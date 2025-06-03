---
title: "Microsoft Edge release notes for Mobile Stable Channel"
ms.author: chfen
author: vmliramichael
manager: alexyuan
ms.date: 06/3/2025
audience: ITPro
ms.topic: release-notes
ms.service: microsoft-edge
ms.localizationpriority: high
ms.collection: M365-modern-desktop
description: "Microsoft Edge release notes for Mobile Stable Channel"
---

# Release notes for Microsoft Edge Mobile Stable Channel

These release notes provide information about new features that are available to work or school accounts, and nonsecurity updates that are included in the Microsoft Edge for Mobile Stable Channel.

To understand Microsoft Edge channels, see the [Overview of the Microsoft Edge channels](./microsoft-edge-channels.md).

All the Stable channel security updates are listed in [Release notes for Microsoft Edge Security Updates](./microsoft-edge-relnotes-security.md).

> [!NOTE]
> For the Stable Channel, updates roll out progressively over one or more days. To learn more, see [Progressive rollouts for Microsoft Edge updates](./microsoft-edge-update-progressive-rollout.md). There might be a delay before the new release is populated to the App Store (iOS) and Google Play (Android). 

## Version 137.0.3296.53 (Android and iOS): June 3, 2025

Fixed various bugs and performance issues, general updates, and enhancements.

### General Updates

- **[iOS]** Upgrade Intune MAM SDK to version `20.5.1`
- **[iOS]** Upgrade MAM Tunnel SDK to version `1.3.3`
- **[iOS & Android]** Upgrade OneAuth SDK to version `6.1.0`

### New Policies

- **[iOS]** Support new App Proxy pre-authentication strict mode policy that ensures URL access must wait until pre-authentication is completed.  
  - MAM Key: `com.microsoft.intune.mam.managedbrowser.AppProxyPreAuthStrictModeEnabled`  
  - Value: `true` = enable, `false` = disable (default)

### Bug Fixes

- **[Android]** Fixed an issue where the Custom URL policy does not work on tablet devices
- **[Android]** Fixed an issue where the Custom Brand Logo and Brand Color do not appear
- **[iOS]** Fixed a blank page issue after configuring the `openInPrivateIfBlocked` policy

### New Enhancements

- **[iOS]** Improved the user experience for web single sign-on
- **[iOS]** Improved the user experience for shared device mode

## Version 136.0.3240.91 (Android and iOS): May 27, 2025

Fixed various bugs and performance issues.

## Version 136.0.3240.77 (iOS): May 19, 2025

Fixed various bugs and performance issues.

## Version 136.0.3240.76 (Android): May 19, 2025

Fixed various bugs and performance issues.

## Version 136.0.3240.71 (iOS): May 12, 2025

Fixed various bugs and performance issues.

## Version 136.0.3240.64 (Android): May 11, 2025

Fixed various bugs and performance issues.

## Version 136.0.3240.61 (iOS): May 8, 2025

Fixed various bugs, general updates, new enhancements.

## General Updates

- [iOS] Upgraded Intune MAM SDK to version `20.4.1`  
- [iOS] Upgraded MAM Tunnel SDK to version `1.3.1`

## Bug Fixes

- [iOS] Fixed an issue where PacProxy redirected incorrectly  
- [iOS] Fixed a memory leak under InPrivate Mode when setting `InPrivateModeAvailability`  
- [iOS] Fixed an issue where the `EdgeRestoreBrowsingOption` MDM Policy had no effect

## New Enhancements

- [iOS] Improved user experience of Guided Switch 
- [iOS] Added support for Strict Mode in Proactive Auth
- [iOS] Improve the user experience of APP Proxy
- [iOS] Improve the user experience of shared device mode

## Version 136.0.3240.50 (Android): May 6, 2025

Fixed various bugs, new enhancements and performance issues.

### Bug fixes

- [Android] Fix the issue about unintentional uploading of data from the personal profile are allowed
- [Android] Fix the issue about inPrivate tabs still can be added in landscape mode after been disabled by policy
- [Android] Fix the issue about the EdgeShowBottomBarInKioskMode may not work on some device
- [Android] Fix the issue of the EdgeRestoreBrowsingOption MDM Policy taking no effect

### New enhancements

- [Android] Improve the user experience when disable Print feature
- [Android] Improve the user experience of shared device mode

## Version 135.0.3179.98 (Android and iOS): April 28, 2025

Fixed various bugs and performance issues.

## Version 135.0.3179.85 (Android and iOS): April 21, 2025

Fixed various bugs and performance issues.

## Version 135.0.3179.72 (Android and iOS): April 14, 2025

Fixed various bugs and performance issues.

## Version 135.0.3179.54 (Android and iOS): April 8, 2025 

Fixed various bugs and performance issues, general updates, new policies, and enhancements.

### General updates

- [iOS & Android] Upgrade OneAuth SDK to version 5.5.0
 
### New Policies

- [iOS & Android] Support new policy that can support to configure “Continue browsing where I left off” or "Always Start with a Fresh New Tab" when Edge launches
(MAM Key: `com.microsoft.intune.mam.managedbrowser.RestoreBrowsingOption`; MDM Key: `EdgeRestoreBrowsingOption`; Value: 0=no config, 1=“Continue browsing where I left off”, 2= "Always Start with a Fresh New Tab")

- [iOS & Android] Support Managed Browser Token Interactive Mode
(MAM Key: `com.microsoft.intune.mam.managedbrowser.EnableInteractiveModeForWebSSO`; Value: true)

- [iOS & Android] Support Managed Desktop View in Mobile
(MDM Key: `DefaultDesktopSiteSetting`; Value: 1=Open all websites with Desktop view, 2=Open all websites with Mobile view

  MDM Key: `DesktopSiteForceForUrls`; Value: a list of site URL patterns that will always open in desktop view

  MDM Key: `MobileSiteForceForUrls`; Value: a list of site URL patterns that will always open in mobile view)

### Bug fixes

- [Android] Fix the issue about OverlayPermissionDetectionEnabled Policy does not work
- [iOS] Fix the issue about 'Open in Microsoft Edge' trigger displays a blocked message
- [iOS] Fix the issue about disabledFeatures=inPrivate does not show toast message
- [iOS & Android] Fix the issue where Policy related with Brand Color does not take effect

### New enhancements

- [Android] Improve the user experience of guide switch
- [iOS] Improve the user experience of single device mode
- [iOS] Improve the user experience of APP Proxy
- [iOS & Android] Improve the user experience of B2W Single sign-on


## Version 134.0.3124.105 (Android): April 2, 2025

Fixed various bugs and performance issues.

## Version 134.0.3124.95 (iOS): March 31, 2025

Fixed various bugs and performance issues.

## Version 134.0.3124.77 (Android and iOS): March 24, 2025

Fixed various bugs and performance issues.

## Version 134.0.3124.68 (Android and iOS): March 17, 2025

Fixed various bugs and performance issues.

## Version 134.0.3124.57 (Android): March 11, 2025

Fixed various bugs and performance issues and new policies.

### New Policies

- [Android] Support manages web sub resource blocking policy By default, AllowListURLs and BlockListURLs apply only at the navigation level. When you embed blocked URLs (either URLs configured in BlockListURLs or URLs not configured in AllowListURLs) as subresources within a web page, those subresource URLs aren't blocked. To further restrict these subresources, you can configure the new policy to block them. For example, if you set `com.microsoft.intune.mam.managedbrowser.ManageRestrictedSubresourceEnabled=true`, subresource URLs are blocked if they're listed as blocked.

### Bug fixes

- [Android] Fix managed bookmark does not show issue in first launch.

## Version 134.0.3124.51 (iOS): March 10, 2025

Fixed various bugs and performance issues, general updates, and enhancements.

### General updates

- [iOS] Upgrade MAM Tunnel SDK to version 1.2.4
- [iOS] Upgrade Intune MAM SDK to version 20.3.0

### Bug fixes

- [iOS] Fix the issue about APP Proxy fails to function properly due to CA Remediation Cache
- [iOS] Fix the issue about sign-in page crash under InPrivate mode when launching
- [iOS] Fix the issue about displaying a blocked message when clicking 'Open in Microsoft Edge'

### New enhancements

- [iOS] Improve the user experience of single device mode
- [iOS] Improve the user experience about InPrivate mode

## Version 133.0.3065.92 (Android): March 1, 2025

Fixed various bugs and performance issues.

## Version 133.0.3065.92 (iOS): February 28, 2025

Fixed various bugs and performance issues.

## Version 133.0.3065.80 (Android): February 24, 2025

Fixed various bugs and performance issues.

## Version 133.0.3065.80 (iOS): February 21, 2025

Fixed various bugs and performance issues.

## Version 133.0.3065.67 (Android): February 18, 2025

Fixed various bugs and performance issues.

### General updates

- [Android] Microsoft 365 Copilot Chat in Edge mobile has re-enable page summarization features, allowing users to summarize open webpages or PDFs.  This feature is available for non-EU regions.  Administrators can control the availability of Copilot Chat in Edge Mobile using the following policy  [com.microsoft.intune.mam.managedbrowser.ChatPageContext](/mem/intune/apps/manage-microsoft-edge#copilot). For more information, see [Microsoft Edge Mobile Policy Documentation | Microsoft Learn](/deployedge/microsoft-edge-mobile-policies#edgecopilotenabled)


## Version 133.0.3065.65 (iOS): February 18, 2025

Fixed various bugs and performance issues.

### General updates

- [iOS] Microsoft 365 Copilot Chat in Edge mobile has re-enable page summarization features, allowing users to summarize open webpages or PDFs.  This feature is available for non-EU regions.  Administrators can control the availability of Copilot Chat in Edge Mobile using the following policy [com.microsoft.intune.mam.managedbrowser.ChatPageContext](/mem/intune/apps/manage-microsoft-edge#copilot). For more information, see [Microsoft Edge Mobile Policy Documentation | Microsoft Learn](/deployedge/microsoft-edge-mobile-policies#edgecopilotenabled)


## Version 133.0.3065.54 (Android and iOS): February 10, 2025

Fixed various bugs and performance issues, general updates, new policies, and enhancements.

### General updates

- [iOS] Upgrade MAM Tunnel SDK to version 1.2.3
- [Android] Upgrade Intune MAM SDK to version 11.1.0
- [iOS & Android] Upgrade MS OneAuth SDK version 5.0.0
- [iOS & Android] Support Page Summary via Copilot for Commercial users
 

### New Policies

- [iOS] Support new policy to ignore the post requests when URL blocked auto switches to private mode or MSA mode
(Set `com.microsoft.intune.mam.managedbrowser.IgnorePostRequestOnAutoTransition=true`)


### Bug fixes

- [iOS] Fix the issue about App Proxy doesn't take effect after signing out and then signing back in without exiting the app
- [iOS] Fix the issue about canceling in Guided Switch doesn't return to the homepage when URL Block is active
 

### New enhancements

- [iOS] Improve IdleTimeoutActions policy and support sign out action
- [iOS] Improve the feature experience for DisableFeature policy about settings and feedback
- [iOS] Improve the user experience about InPrivate mode on iPad
- [iOS & Android] Add manage account entry in account settings page

## Version 132.0.2957.129 (Android): January 27, 2025

Fixed various bugs and performance issues.

## Version 132.0.2957.122 (iOS): January 23, 2025

Fixed various bugs and performance issues.

## Version 132.0.2957.118 (Android and iOS): January 22, 2025

Fixed various bugs and performance issues, general updates, new policies, and enhancements.

### General Updates

- [iOS] Upgrade Intune MAM SDK to version 19.7.8
- [iOS] Upgrade MAM Tunnel SDK to version 1.2.1
- [Android] Support workspaces feature on Android (Need to enable feature under edge://flags)

### New Policies

- [iOS] Support manages web sub resource blocking policy (By default, AllowListURLs and BlockListURLs apply only at the navigation level. When you embed blocked URLs (either URLs configured in BlockListURLs or URLs not configured in AllowListURLs) as sub resources within a web page, those sub resource URLs aren't blocked. To further restrict these sub resources, you can configure the new policy to block the sub resource URLs. For example, set `com.microsoft.intune.mam.managedbrowser.ManageRestrictedSubresourceEnabled=true`, subresource URLs are blocked if they're listed as blocked.)

### Bug Fixes

- [iOS] Fix the issue with open PDF file with special characters in the file name
- [iOS] Fix bookmark MDM Policy not taking effect
- [iOS] Fix download bypasses Intune share policy under InPrivate mode
- [iOS] Fix InPrivate policy wasn't fully effective in the context menu
- [Android] Fix brand logo may not show at sometimes

### New Enhancements

- [iOS] Improve the sign-in experience for single device mode
- [iOS] Improve the feature experience for DisableFeature policy about settings and feedback
- [iOS] Enhancements the experience of bookmark icon under App Proxy
- [Android] Support remove certain account from sign in account list

## Version 131.0.2903.145 (Android and iOS): January 13, 2025

Fixed various bugs and performance issues.

## Version 131.0.2903.134 (Android and iOS): January 02, 2025

Fixed various bugs and performance issues.

## Version 131.0.2903.125 (iOS): December 30, 2024

Fixed various bugs and performance issues.


## Version 131.0.2903.125 (Android): December 27, 2024

Fixed various bugs and performance issues.

## Version 131.0.2903.113 (Android): December 23, 2024

Fixed various bugs and performance issues.

## Version 131.0.2903.112 (iOS): December 19, 2024

Fixed various bugs and performance issues.

## Version 131.0.2903.107 (Android and iOS): December 17, 2024

Fixed various bugs and performance issues.

## Version 131.0.2903.101 (Android and iOS): December 13, 2024

Fixed various bugs and performance issues.

## Version 131.0.2903.87 (Android): December 9, 2024

Fixed various bugs and performance issues.


## Version 131.0.2903.77 (Android and iOS): December 2, 2024

Fixed various bugs and performance issues.

## Version 131.0.2903.68 (Android and iOS): November 25, 2024

Fixed various bugs and performance issues.

## Version 131.0.2903.54 (iOS): November 19, 2024

Fixed various bugs and performance issues, general updates, new policies, and enhancements.

### General updates

- [iOS] Upgrade Intune MAM SDK to version 19.7.2
- [iOS] Upgrade MAM Tunnel SDK to version 1.2.1
- [iOS] Upgrade MS OneAuth SDK version 4.0.2

### Bug fixes

- [iOS] Fix the issue with saving Word/Excel/PowerPoint files locally.
- [iOS] Fix unresponsive sign-in panel in "Send to device".
- [iOS] Fix the issue where the [IdleTimeout](/deployedge/microsoft-edge-mobile-policies#idletimeout) policy did not resume normal operation after the action was completed.
- [iOS] Fix Tooltip cannot auto-dismiss when VoiceOver is turned on.

### New Policies

- [iOS] Support to disable settings and feedback features via DisableFeature policy
(`com.microsoft.intune.mam.managedbrowser.disabledFeatures` in MAM and `EdgeDisabledFeatures` in MDM now supports configuring disable settings and feedback features on the NTP using the values "settings" and "feedback")
- [iOS] Support Microsoft Entra ID File advanced encryption by Intune auto file encryption capability. (Implement comprehensive encryption of sandbox files under Microsoft Entra ID accounts using Intune MAM SDK's File Transparent Encryption. File encryption is enabled when the `com.microsoft.intune.IntuneMAMOnly.AdvancedEncryption` policy is set to Enabled.)

### Enhancements

- [iOS] Improve the feature experience for the App Proxy policy by preventing it from not functioning correctly until the next cold start.
- [iOS] Improve the feature experience for switching profile.
- [iOS] General enhancements to [NewTabPageLayout](/deployedge/microsoft-edge-mobile-policies#edgenewtabpagelayout) policy (Policy auto correct NewTabPageLayout to custom if `NewTabPageLayout.Custom` has value).
- [iOS] Support sign-out action in [IdleTimeoutActions](/deployedge/microsoft-edge-mobile-policies#idletimeoutactions) policy.

## Version 131.0.2903.48 (Android): November 18, 2024

Fixed various bugs and performance issues, general updates, new policies, and enhancements.

### General updates

- [Android] Upgrade MS OneAuth SDK version 4.0.2

### New Policies

- [Android] Support to disable settings and feedback features via DisableFeature policy
(`com.microsoft.intune.mam.managedbrowser.disabledFeatures` in MAM and `EdgeDisabledFeatures` in MDM now supports configuring disable settings and feedback features on the NTP using the values "settings" and "feedback")

### Enhancements

- [Android] Enhancements the display size of brandLogo (Related policy `com.microsoft.intune.mam.managedbrowser.NewTabPage.BrandLogo`).
- [Android] Improve the sign-in experience for single device mode (Remove SDM needed restart on first startup).
- [Android] General enhancements to NewTabPageLayout policy (Policy auto correct NewTabPageLayout to custom if NewTabPageLayout.Custom has value).

## Version 130.0.2849.80 (Android and iOS): November 11, 2024

Fixed various bugs and performance issues.

## Version 130.0.2849.68 (Android and iOS): November 4, 2024

Fixed various bugs and performance issues.

## Version 130.0.2849.57 (Android and iOS): October 28, 2024

Fixed various bugs and performance issues.

## Version 130.0.2849.52 (iOS): October 23, 2024

Fixed various bugs and performance issues.

### General update

- [iOS] Upgrade Intune MAM SDK to version 19.7.2 which contains support for blocking of Apple Intelligence.

## Version 130.0.2849.46 (Android and iOS): October 20, 2024

Fixed various bugs and performance issues, general updates, new policies, and enhancements.

### General updates

- [iOS] Upgrade Intune MAM SDK to version 19.7.0
- [iOS] Upgrade MAM Tunnel SDK to version 1.1.12
- [iOS & Android] Enable wallpaper on NTP for Commercial user by default. A user can configure `com.microsoft.intune.mam.managedbrowser.NewTabPageLayout.Custom` to exclude the wallpaper.
- [iOS & Android] Enable weather widget on NTP for Commercial user by default. A user can add weather token to **DisableFeature** policy to disable it the widget.

### Bug fixes

- [iOS] Fix issue about single device mode force sign-in interrupted by external intent.
- [iOS] Fix **disableImportPasswords** policy not working as expected.

### New policies

- [iOS & Android] Support to disable weather widget on NTP via **DisableFeature** policy
(`com.microsoft.intune.mam.managedbrowser.disabledFeatures` in MAM) and **EdgeDisabledFeatures** in MDM, now supports disabling weather widget on NTP by using "weather" as value.

### Enhancements

- [iOS] Support removing specified account from sign in account list.
- [Android] Change default value of `recommendsCustomUi` to support passkey in Edge. Before these changes, the user can only use Google Password Manager and can't select Microsoft Authenticator to save passkey. After these changes, a user can select a third party passkey app, including Microsoft Authenticator.
- [Android] Improves the feature experience for App proxy.
- [iOS & Android] Improves the occurrence of re-sign in prompts on NTP.
- [iOS & Android] General enhancements to NTLMSSO policies to make it more useful.
- [iOS & Android] Enable Managed Browser revamp feature by default with silent mode as the managed browser. This change helps customers remediate from non-compliant cases, such as no device registration.

<!-- Version 129.0.2792.58 (Android and iOS): September 24, 2024 to Version 129.0.2792.92 (Android and iOS): October 15, 2024 --->
<!-- Version 128.0.2739.82 (iOS): September 18, 2024 to Version 128.0.2739.42 (iOS): August 27, 2024 --->
<!-- Version 127.0.2651.111 (Android and iOS): August 20, 2024 to Version 127.0.2651.81 (iOS): July 31, 2024 --->
<!-- Version 126.2592.120 (iOS): July 24, 2024 to Version 126.0.2592.56 (Android and iOS): June 17, 2024 -->
<!-- Version 125.0.2535.96 (Android and iOS): June 11, 2024 to Version 125.0.2535.51 (Android): May 21, 2024 --->
<!-- Version 124.0.2478.105 (iOS): May 17, 2024 to Version 124.0.2478.50 (Android and iOS): April 22, 2024 -->
<!-- Version 123.0.2420.108 (iOS): April 19, 2024 to Version 123.0.2420.56 (iOS): March 25, 2024 -->
<!-- Version 122.0.2365.99 (Android and iOS): March 18, to 2024 Version 121.0.2277.84 (Android): January 29, 2024 -->
<!-- Version 120.0.2210.150: January 21, 2024 to Version 120.0.2210.59: December 12, 2023 -->
<!-- Version 119.0.2151.107: December 6, 2023 to Version 119.0.2151.46: November 7, 2023  -->
<!-- Version 118.0.2088.81: November 1, 2023 to Version 117.0.2045.53: October 6, 2023  -->
<!-- Version 117.0.2045.33: September 15, 2023 to Version 116.0.1938.64: August 30, 2023  -->
<!-- Version 116.0.1938.56: August 21, 2023, to Version 115.0.1901.183: July 22, 2023 -->
<!-- Version 114.0.1823.37: June 2, 2023 to Version 113.0.1774.50: May 18, 2023 -->
<!-- Version 113.1774.36: May 8, 2023 to Version 112.0.1722.36: April 7, 2023 -->
<!-- Version 111.0.1661.43: March 18, 2023 to Version 109.0.1518.70: January 26, 2023 -->
<!-- Version Version 109.0.1518.58: January 18, 2023 to Version 108.0.1462.45: December 8, 2022  -->
<!-- Version 108.0.1462.43: December 7, 2022 to Version 106.0.1370.47: October 17, 2022 -->
<!-- Version 105.0.1343.38: September 13, 2022 to Version 101.0.1210.32: April 29, 2022 -->

## See also

- [Microsoft Edge Enterprise landing page](https://aka.ms/EdgeEnterprise)
