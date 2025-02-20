---
title: "Identify and interrupt downloads of potentially dangerous files"
ms.author: kvice
author: dan-wesley
manager: likuba
ms.date: 07/18/2024
audience: ITPro
ms.topic: conceptual
ms.service: microsoft-edge
ms.localizationpriority: medium
ms.collection: M365-modern-desktop
description: "Understand how Microsoft Edge identifies and interrupts downloads of potentially dangerous files"
---

# Identify and interrupt downloads of potentially dangerous files

Microsoft Edge's File Type Policies component classifies files by their level of "dangerousness" to manage file downloads. A harmless file (for example, a `.txt` file) can be downloaded freely, while a potentially dangerous file like a `.dll` is subjected to a higher degree of vetting. This scrutiny provides a more security-conscious user experience.

## How Microsoft Edge determines the danger level of a file type

Microsoft Edge inherits most of its file type policies from the upstream Chromium browser, with a few changes for security or compatibility reasons. You can view Chromium's policies for file types and their classification in the [download_file_types.asciipb](https://source.chromium.org/chromium/chromium/src/+/main:components/safe_browsing/core/resources/download_file_types.asciipb;drc=af17ad3f07c1d8a24381eb7669bec0c2ffb86521) file. In this file, you'll see that each type has a **danger_level**, which is one of three values: `DANGEROUS`, `NOT_DANGEROUS`, or `ALLOW_ON_USER_GESTURE`.

The following two classifications are simple:

- **NOT_DANGEROUS** means that the file is safe to download, even if the download request was accidental.
- **DANGEROUS** means that the browser should always warn the user that the download may harm their device.

The third setting, **ALLOW_ON_USER_GESTURE** is more subtle. These files are potentially dangerous, but most likely harmless if the user requests the download. Microsoft Edge will allow these downloads to continue automatically if **two** conditions are **both** met:

- There's a [user gesture](https://textslashplain.com/2020/05/18/browser-basics-user-gestures/) associated with the network request that started the download. For example, the user clicked a link to the download.
- There's a recorded prior visit to the referring origin (the page that links to the download) before the most recent midnight (that is, yesterday or earlier). This recorded visit implies that the user has a history of visiting the site.

The download will also continue automatically if the user explicitly starts it by using the **Save link as** context menu command, enters the download's URL directly into the browser's address bar, or if Microsoft Defender SmartScreen indicates that the file is safe.

> [!NOTE]
> Starting in version 91, Microsoft Edge will interrupt downloads that lack the required gesture.

## User experience for downloads that lack a gesture

If a download for a potentially dangerous type starts without the required gesture, Microsoft Edge states that the download "was blocked". Commands named `Keep` and `Delete` are available from the **…** (ellipsis) option on the download item to let the user continue or cancel the download.

:::image type="content" source="media/microsoft-edge-security-Download-interruptions/Dowload-was-blocked.png" alt-text="Download is blocked, user can keep or delete the download.":::

On the `edge://downloads` page, the user will see the same options. The next screenshot shows an example of these options.

:::image type="content" source="media/microsoft-edge-security-Download-interruptions/msg-keep-delete-option.png" alt-text="Download is blocked but user can keep or delete the download.":::

## Enterprise controls for downloads

While users are unlikely to encounter download interruptions for sites they use every day, they might encounter them for legitimate downloads on sites that they use rarely. To help streamline the user-experience for Enterprises, a Group Policy is available.

Enterprises can use [ExemptFileTypeDownloadWarnings](/deployedge/microsoft-edge-policies#exemptfiletypedownloadwarnings) to specify the filetypes that are allowed to download from specific sites without interruption. For example, the following policy allows `XML` files to download from `contoso.com` and `woodgrovebank.com` without interruption, and allows `MSG` files to download from any site.

`[{"file_extension":"xml","domains":["contoso.com", "woodgrovebank.com"]},
{"file_extension":"msg", "domains": ["*"]}]`

### Update for Edge Version 132

With the release of Edge Version 132.0.2915.0, a change was introduced that affects the handling of `.crx` files (Chrome extension files). The `DownloadRestrictions` policy now blocks the download of `.crx` files if configured to block dangerous file types (options 1, 2, or 3). This change was introduced through Chromium and is documented in the Chromium code review.

To address this issue, enterprises should update their policies to include the `ExemptFileTypeDownloadWarnings` policy to allow `.crx` files to be downloaded without interruption. For example:

`[{"file_extension": "crx", "domains": ["*"]},
{"file_extension":"xml","domains":["contoso.com", "woodgrovebank.com"]},
{"file_extension":"msg", "domains": ["*"]}]`

## File types requiring a gesture

Chromium's latest [file types policies](https://source.chromium.org/chromium/chromium/src/+/main:components/safe_browsing/core/resources/download_file_types.asciipb;drc=af17ad3f07c1d8a24381eb7669bec0c2ffb86521) are published in the Chromium source code, and Microsoft Edge inherits most of these, with a few changes for security or compatibility reasons. As of May 2021, file types with a `danger_level` of `ALLOW_ON_USER_GESTURE` on at least one OS platform include:
`crx, pl, py, pyc, pyo, pyw, rb, efi, oxt, msi, msp, mst, ade, adp, mad, maf, mag, mam, maq, mar, mas, mat, mav, maw, mda, mdb, mde, mdt, mdw, mdz, accdb, accde, accdr, accda, ocx, ops, paf, pcd, pif, plg, prf, prg, pst, cpi, partial, xrm-ms, rels, svg, xml, xsl, xsd, ps1, ps1xml, ps2, ps2xml, psc1, psc2, js, jse, vb, vbe, vbs, vbscript, ws, wsc, wsf, wsh, msh, msh1, msh2, mshxml, msh1xml, msh2xml, ad, app, application, appref-ms, asp, asx, bas, bat, chi, chm, cmd, com, cpl, crt, cer, der, eml, exe, fon, fxp, hlp, htt, inf, ins, inx, isu, isp, job, lnk, mau, mht, mhtml, mmc, msc, msg, reg, rgs, scr, sct, search-ms, settingcontent-ms, shb, shs, slk, u3p, vdx, vsx, vtx, vsdx, vssx, vstx, vsdm, vssm, vstm, vsd, vsmacros, vss, vst, vsw, xnk, cdr, dart, dc42, diskcopy42, dmg, dmgpart, dvdr, dylib, img, imgpart, ndif, service, smi, sparsebundle, sparseimage, toast, udif, action, definition, wflow, caction, as, cpgz, command, mpkg, pax, workflow, xip, mobileconfig, configprofile, internetconnect, networkconnect, pkg, deb, pet, pup, rpm, slp, out, run, bash, csh, ksh, sh, shar, tcsh, desktop, dex, apk, rdp`

## The file type danger level may vary by operating system

File type settings sometimes vary depending on the client OS platform. For instance, an `.exe` file isn't dangerous on a Mac, while an `.applescript` file is harmless on Windows.
