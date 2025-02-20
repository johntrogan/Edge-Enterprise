---
title: "Deploy Microsoft Edge with Windows 10 updates"
ms.author: archandr
author: dan-wesley
manager: likuba
ms.date: 07/18/2024
audience: ITPro
ms.topic: conceptual
ms.service: microsoft-edge
ms.localizationpriority: medium
ms.collection: M365-modern-desktop
description: "Deploy Microsoft Edge with Windows 10 updates"
---

# Deploy Microsoft Edge with Windows 10 updates

The article provides information for users who are deploying Microsoft Edge by using Windows 10 updates.

## For Windows 10 October 2020 Update

Windows 10 October 2020 Update and later include Microsoft Edge pre-installed as the default browser. However, version 84 of Microsoft Edge that shipped with Windows 10 October 2020 Update, and version 92 of Microsoft Edge that shipped with Windows 10 November 2021 Update, are now outdated. While Microsoft Edge will automatically update itself to a newer version after a user has logged on, since the timing of the update is dependant upon various factors, this can be unpredictable. For organizations that desire greater control and want to ensure that Microsoft Edge (Stable channel) is updated to the latest version before user sign-in, the following PowerShell command can be used to force a Microsoft Edge update during Windows OOBE.

`Start-Process -FilePath "C:\Program Files (x86)\Microsoft\EdgeUpdate\MicrosoftEdgeUpdate.exe" -argumentlist "/silent /install appguid={56EB18F8-B008-4CBD-B6D2-8C97FE7E9062}&appname=Microsoft%20Edge&needsadmin=True"`

If using Windows Autopilot, it's possible to wrap this script as an \.intunewin file using the [Microsoft Win32 content prep tool](/mem/intune/apps/apps-win32-prepare). It can then be set as a required app for the Enrollment Status Page (ESP) if desired.

> [!NOTE]
> If you currently leverage policies such as [Target Channel override](/deployedge/microsoft-edge-update-policies#target-channel-override) or [Target Version override](/deployedge/microsoft-edge-update-policies#targetversionprefix) to remain on an older version of Microsoft Edge, be aware that the above script will not take any policies into account, and will simply update to the latest version. By default, Microsoft Edge does not downgrade itself, including once such policies are later received.

## For Windows 10 releases Windows 10 April 2018 Update through Windows 10 April 2020 Update

Windows Server Update Services (WSUS) has updates for each version of Windows 10 from Windows 10 April 2018 Update through Windows 10 April 2020 Update that will remove the Microsoft Edge Legacy desktop app and replace it with Microsoft Edge. For more information, see [this support article](https://support.microsoft.com/topic/update-in-wsus-for-the-new-microsoft-edge-for-windows-10-version-1809-1903-1909-and-2004-october-29-2020-b4980418-4ec4-dee7-3b17-1c6499bd127c) to find out which WSUS update is right for your Windows version.

## For Windows 10 releases prior to Windows 10 April 2018 Update (and Windows 7, 8.1, and earlier)

Windows updates to install Microsoft Edge aren't available for these versions. Consider other options for deploying Microsoft Edge to these devices such as [Configuration Manager](/configmgr/apps/deploy-use/deploy-edge?bc=%2fDeployEdge%2fbreadcrumb%2ftoc.json&toc=%2fDeployEdge%2ftoc.json) or [Intune](/mem/intune/apps/apps-windows-edge/?bc=%2fDeployEdge%2fbreadcrumb%2ftoc.json&toc=%2fDeployEdge%2ftoc.json).

## See also

- [Microsoft Edge Enterprise landing page](https://aka.ms/EdgeEnterprise)
- [Plan your deployment of Microsoft Edge](deploy-edge-plan-deployment.md)