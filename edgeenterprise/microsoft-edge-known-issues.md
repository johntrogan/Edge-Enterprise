---
title: "Microsoft Edge known issues"
ms.author: archandr
author: vmliramichael
manager: likuba
ms.date: 03/13/2025
audience: ITPro
ms.topic: troubleshooting-known-issue
ms.service: microsoft-edge
ms.localizationpriority: high
ms.collection: M365-modern-desktop
description: "Microsoft Edge known issues, workarounds, and fixes"
---

# Microsoft Edge known issues

This article tracks the known issues, workarounds, and fixes for Microsoft Edge.

## High impact issues

These issues are high impact as identified by Customer Service & Support. Check this article often as the Microsoft Edge team provides workarounds and fixes.

The following table lists the issues that the Microsoft Edge team is tracking closely, working on, or resolved.

<!--------------------------------->
<!------ TAB 1 OPEN --------------->
<!--------------------------------->

## [**Open issues**](#tab/Open)

| Version | Symptom | Workaround | Comment |
| --- | --- | --- | --- |
| 135 | Customers may see an issue where the first-run experience (FRE) page edge://welcome-new-device opens and fails with an error message page that doesn't close. This occurs when FRE is disabled and might be triggered suddenly after upgrade.  | Roll back Microsoft Edge to version 134.0.3124.95 or modify the HideFirstRunExperience policy to “0”. | This issue is fixed in Microsoft Edge stable release 135.0.3179.85. |
| 134 | Some customers may unexpectedly start seeing the sidepane open with context for their Teams and Outlook links. In Edge 134, a bug fix introduced a regression where if the sidebar was turned off (not visible), Edge would auto-open Teams or Outlook context in the sidepane. | Users can manually toggle off the auto-open context experience in Edge settings (Copilot and sidebar/App and notification settings/Teams + Outlook). | We're working to release a fix for Microsoft Edge as soon as possible. This ensures that the side pane doesn't appear for users who don't have the sidebar visible. |
| 134 | Enterprise users with Multifactor Authentication (MFA) and Conditional Access (CA) may see popups when they start the Microsoft Edge browser. |  | Recognizing the broad impact this issue is having, Microsoft is working to temporarily mitigate this issue through the [Experimentation and Configuration Service (ECS)](/deployedge/edge-configuration-and-experiments). To receive the mitigation, admins should either **not** configure the [ExperimentationAndConfigurationServiceControl](/deployedge/microsoft-edge-policies#experimentationandconfigurationservicecontrol) policy or set the policy to "FullMode" or "ConfigurationsOnlyMode". |
| 134 | Enterprise users with MFA and CA may not have Single Sign-on (SSO) with Microsoft 365 Copilot Chat. The user may see a "sign in" button. |  | The user may see a "sign in" button when they try to use Copilot. |
| 134 | Customers may not be able to start the Microsoft Edge browser programmatically using `--inprivate` and `--app` (application mode) via the command line because the browser crashes. | Customers can start the browser using `"C:\Program Files (x86)\Microsoft\Edge\Application\msedge.exe" https://www.contoso.com --inprivate`. Alternatively, they can roll back to Microsoft Edge version 133.0.3065.92. | This issue is fixed in Microsoft Edge stable release 134.0.3124.83. |
| 133 | Customers may not be able to start the sync functionality or open AIP-protected PDF files in Microsoft Edge. A bug in version 133 caused excessive traffic to the MIP service. | For sync: "sign out (keeping locally saved data)" then "sign in" again. For AIP-protected PDFs, use Azure Information Protection Viewer. | This issue is fixed in Microsoft Edge stable release 133.0.3065.69. Note: For some users, it may still be necessary to sign out and sign in again. |
| 130 | In version 130.0.2849.46, nonspecial scheme URL handling was updated to align with the [URL Standard](https://url.spec.whatwg.org/), which may affect site compatibility. | Don't configure or set [ExperimentationAndConfigurationServiceControl](/deployedge/microsoft-edge-policies#experimentationandconfigurationservicecontrol) to "FullMode" or "ConfigurationsOnlyMode". Alternatively, roll back to version 129.0.2792.89. | Microsoft temporarily disabled this feature via [ECS](/deployedge/edge-configuration-and-experiments). A browser restart is needed. A code change in version 130.0.2849.80 also disables it if ECS is blocked by policy. **Note:** Re-enabled in version 133.0.3065.10+. |
| 124 | Specific HTTPS websites may show `ERR_CONNECTION_ABORTED` or `ERR_SSL_PROTOCOL_ERROR`. Linked to the "TLS 1.3 hybridized Kyber support" feature. | Disable Kyber via `edge://flags/#enable-tls13-kyber`. Enterprises can use the **PostQuantumKeyAgreementEnabled** policy. Registry: `[HKEY_LOCAL_MACHINE\Software\Policies\Microsoft\Edge] (DWORD) "PostQuantumKeyAgreementEnabled"=0` | This workaround is temporary and will be removed in future versions. Disabling weakens TLS security. |
| 121 | Specific HTTPS websites may show `ERR_SSL_KEY_USAGE_INCOMPATIBLE`, caused by enforcing X.509 key usage extensions. | Set the **RSAKeyUsageForLocalAnchorsEnabled** policy. Registry: `[HKEY_LOCAL_MACHINE\Software\Policies\Microsoft\Edge] (DWORD) "RSAKeyUsageForLocalAnchorsEnabled"=0` | This policy isn't effective in Microsoft Edge version 124 and later. |
| 120 | Microsoft Edge opens HTTP URLs as HTTPS when the server supports HTTPS. This is due to the "HttpsDefault" feature. | Use the **HttpsUpgradesEnabled** policy to disable automatic HTTPS.  Previously, the **AutomaticHttpsDefault** policy was used, but it has been deprecated in Microsoft Edge version 136.  Registry: `[HKEY_LOCAL_MACHINE\Software\Policies\Microsoft\Edge] (DWORD) "HttpsUpgradesEnabled"=0`. To disable per-site, use **InsecureContentAllowedForUrls**. |  |
| 119 | Specific HTTPS websites may show `ERR_SSL_PROTOCOL_ERROR` due to removal of SHA-1 in TLS handshakes. | Set **InsecureHashesInTLSHandshakesEnabled** policy. Registry: `[HKEY_LOCAL_MACHINE\Software\Policies\Microsoft\Edge] (DWORD) "InsecureHashesInTLSHandshakesEnabled"=1` | This policy was removed in version 124+. Enabling this increases impersonation risk. |


<!--------------------------------->
<!--------- TAB 2 FIXED ----------->
<!--------------------------------->

## [**Fixed issues**](#tab/Fixed)

|  Version  | Symptom | Workaround | Comment |
| --- | --- | --- | --- |
| 131 | With Microsoft Edge Stable version 131.0.2903.48, some text isn't displayed, and rendering is broken when viewing certain PDF files containing Japanese fonts. | This issue doesn't occur with the new Adobe Acrobat powered built-in PDF reader. Enterprise administrators can avoid the issue by enabling the [NewPDFReaderEnabled](/deployedge/microsoft-edge-policies#newpdfreaderenabled) policy. Each user can also avoid the issue by enabling the New PDF Viewer in *edge://flags/#edge-new-pdf-viewer*.<br><br>**Note:**<br>When you set NewPDFReaderEnabled to 1, the PDF is displayed correctly in Edge. However, the same issue occurs in the print preview. Some text doesn't display correctly in the print preview, but the actual printout is correct.  | This issue on Windows is fixed in Microsoft Edge stable release 131.0.2903.70.<br><br>This issue on macOS is fixed in Microsoft Edge stable release 132.0.2957.115. |
| 130 | With Microsoft Edge Stable version 130.0.2849.46, some browser extensions are no longer working if they're using the chrome.storage.managed API. | Roll back Microsoft Edge to version 129.0.2792.89. | This issue is fixed in Microsoft Edge stable release 130.0.2849.56. |
| 128    | Starting with Microsoft Edge Stable version 128.0.2739.42, pages may fail to fully load when retrieving resources from the HTTP cache. When the issue is encountered, DevTools shows the requests failing with net::ERR_FAILED.| Roll back Microsoft Edge to version 127.0.2651.105 for Edge Stable or version 126.0.2592.137 for Edge Extended Stable.<br><br>A force reload (Ctrl+Reload button) can mitigate individual page loads.<br><br>Site owners may also consider reducing the use of HTTP caching for impacted resources until the issue is addressed. |Microsoft is collaborating with the Chromium project via [Chromium bug 362788339]( https://issues.chromium.org/issues/362788339) to address the issue. This issue is fixed in Microsoft Edge stable release 128.0.2739.63. |
| 128    | Starting with Microsoft Edge Stable version 128.0.2739.42, customs configured start pages appear to be stuck in the loading state. | Roll back Microsoft Edge to version 127.0.2651.105 for Edge Stable or version 126.0.2592.137 for Edge Extended Stable.<br><br>Use the command line argument: `"C:\Program Files (x86)\Microsoft\Edge\Application\msedge.exe" --disable-features="msIrm, msIrmv2, msEndpointDLp"`<br>**Note:** Command line args are case sensitive. | The fix is included in Stable version 128.0.2739.54.  |


## See also

- [Microsoft Edge Enterprise landing page](https://aka.ms/EdgeEnterprise)
