---
title: "Archived - release notes for Microsoft Edge Mobile Stable Channel"
ms.author: archandr
author: dan-wesley
manager: likuba
ms.date: 01/29/2024
audience: ITPro
ms.topic: conceptual
ms.service: microsoft-edge
ms.localizationpriority: medium
ms.collection: M365-modern-desktop
description: "Archived release notes for Microsoft Edge Mobile Stable Channel"
---

# Archived - release notes for Microsoft Edge Mobile Stable Channel

These release notes provide information about new features and non-security updates that are included in the Microsoft Mobile Edge Stable Channel. All the security updates are listed [here](microsoft-edge-relnotes-security.md).

<!-- Version 129.0.2792.58 (Android and iOS): September 24, 2024 to Version 129.0.2792.92 (Android and iOS): October 15, 2024 --->

## Version 129.0.2792.92 (Android and iOS): October 15, 2024

Fixed various bugs and performance issues.

## Version 129.0.2792.84 (Android and iOS): October 9, 2024

Fixed various bugs and performance issues, enhancements.  

### Enhancements

- [Android and iOS] The page layout of the New Tab Page (NTP) defaults to Inspirational for Microsoft Entra ID accounts.

## Version 129.0.2792.65 (Android): September 27, 2024

Fixed various bugs and performance issues.

## Version 129.0.2792.58 (Android and iOS): September 24, 2024

Fixed various bugs and performance issues, general updates, bug fixes, enhancements, and new policies.

### General updates

- [iOS] Upgrade Intune MAM SDK to version 19.6.0
- [Android] Upgrade Intune MAM SDK to version 10.4.0
- [Android and iOS] Upgrade MS OneAuth SDK version 3.3.0 
- [Android and iOS] Remove native AAD Copilot support

### Bug fixes

- [iOS] Fix managed bookmarks dismiss under AAD account (without "XXX's Favorites" folder under favorites)
- [iOS] Fix downloaded files not properly moved in work profile
- [iOS] Fix a bug related to MAM Tunnel can't be disconnected automatically when change to personal account
- [iOS] Fix disableFeatures policy - InPrivate mode disablement bug & support policy auto change
(The problem is when set `com.microsoft.intune.mam.managedbrowser.disabledFeatures='inprivate'`, the InPrivate mode can still be accessed, and the corresponding toolbar button remains functional. Expects the policy to support dynamic switching without needing to restart Microsoft Edge. When the policy disables InPrivate mode, the application should automatically exit InPrivate mode and close all open InPrivate tabs)

### Enhancements

- [iOS] Improve the transition user experience for account switcher in iPad
- [iOS] Improve Web SSO for CMC (copilot.microsoft.com) sign in in MSA
- [Android and iOS] Improve the occurrence of re-sign-in prompts by disallow user interaction for proactive-auth
- [Android and iOS] Improve account verification by consider sync and news feed status
- [Android and iOS] General enhancements to NTLMSSO policies to make it more useful

### New Policies

- [Android and iOS] Support to disable Share and SendtoDevices via **DisableFeature** policy
(`com.microsoft.intune.mam.managedbrowser.disabledFeatures` in MAM and `EdgeDisabledFeatures` in MDM now support to config to disable Share and Sendtodevices in overflow menu by value share|sendtodevices)


<!-- Version 128.0.2739.82 (iOS): September 18, 2024 to Version 128.0.2739.42 (iOS): August 27, 2024 --->

## Version 128.0.2739.82 (iOS): September 18, 2024

Fixed various bugs and performance issues.

## Version 128.0.2739.82 (Android): September 16, 2024

Fixed various bugs and performance issues.

## Version 128.0.2739.72 (Android and iOS): September 10, 2024

Fixed various bugs and performance issues.

## Version 128.0.2739.64 (Android): September 5,2024

Fixed various bugs and performance issues.

## Version 128.0.2739.60 (iOS): September 4, 2024

Fixed various bugs and performance issues.

## Version 128.0.2739.60 (Android): September 3, 2024

Fixed various bugs and performance issues, general updates, enhancements, and feature updates.

### General updates

- [Android] Upgrade Intune MAM SDK to version 10.3.1
- [Android] Upgrade OneAuth SDK to version 3.0.0

### Bug fixes

- [Android] Fix AppProxy translation worked in InPrivate context unexpectedly
- [Android] Fix a bug related to policy of single device mode

### Enhancements

- [Android] General enhancements to NTLMSSO policies to make it more useful, and added support for 407 proxy auth challenges.
- [Android] Re-sign-in prompts and banners are reworded as "re-verify account" for clarity. These prompts and banners remind the user to verify their account by reinputting a password and refresh underlying tokens to keep account state healthy.
- [Android] Clear opened tabs data when signing out of Microsoft Entra ID if clear data is chosen.

### Feature updates

- **Deprecation of Copilot on Edge mobile.** Microsoft Copilot and the corresponding settings are removed from the Edge mobile application.  

  Copilot for work and web chat will be available to Entra ID users through the Microsoft 365 mobile application.

## Version 128.0.2739.42 (iOS): August 27, 2024

Fixed various bugs and performance issues, general updates, enhancements, feature updates, and new policies.

### General updates

- [iOS] Upgrade MS Tunnel SDK version 1.1.7
- [iOS] Upgrade Intune MAM SDK to version 19.5.1
- [iOS] Upgrade OneAuth SDK to version 3.0.0

### Bug fixes

- [iOS] Fix a bug related to the [DefaultBrowserSettingEnabled](/deployedge/microsoft-edge-mobile-policies#defaultbrowsersettingenabled) policy.

### Enhancements

- [iOS] General enhancements to NTLMSSO policies to make it more useful, added support for 407 proxy auth challenges.
- [iOS] Re-sign-in prompts and banners are changed to "re-verify account" for clarity. These prompts and banners remind a user to verify their account by reinputting a password and refresh underlying tokens to keep account state healthy.
- [iOS] Clear opened tabs data when signing out of Microsoft Entra ID if clear data is chosen.

### Feature updates

- **Deprecation of Copilot on Edge mobile.** Microsoft Copilot and the corresponding settings are removed from the Edge mobile application.  

  Copilot for work and web chat will be available to Entra ID users through the Microsoft 365 mobile application.

### New Policies

- [iOS] Enable Web Inspector and add a new token (`webinspector`) of disabled features policy to disable it. Previously Web Inspector was disabled in Stable versions, but it's now enabled for general web site debugging and troubleshooting purposes.

<!-- Version 129.0.2792.52: September 19, 2024 to Version 129.0.2792.12: August 29, 2024 -->

## Version 129.0.2792.52: September 19, 2024

Fixed various bugs and performance issues.

## Version 129.0.2792.50: September 18, 2024

Fixed various bugs and performance issues.

## Version 129.0.2792.41: September 13, 2024

Fixed various bugs and performance issues.

## Version 129.0.2792.31: September 9, 2024

Fixed various bugs and performance issues.

## Version 129.0.2792.21: September 3, 2024

Fixed various bugs and performance issues.

## Version 129.0.2792.12: August 29, 2024

Fixed various bugs and performance issues, feature updates.

### Dev Channel updates

The following Dev channel updates preceded this Beta channel release. These notes provide detailed information about the changes in each release.

- [Dev Channel update to 129.0.2752.4 is live. - Microsoft Community Hub](https://techcommunity.microsoft.com/t5/articles/dev-channel-update-to-129-0-2752-4-is-live/m-p/4215208)
- [Dev Channel update to 129.0.2766.0 is live. - Microsoft Community Hub](https://techcommunity.microsoft.com/t5/articles/dev-channel-update-to-129-0-2766-0-is-live/m-p/4218361)
- [Dev Channel update to 129.0.2779.0 is live. - Microsoft Community Hub](https://techcommunity.microsoft.com/t5/articles/dev-channel-update-to-129-0-2779-0-is-live/m-p/4226574)

### Fixes

- **Policy updates to allow wildcards.** The documentation for the following policies were inaccurate and were corrected. These policies support wildcards (*) in URL patterns when being configured: [ImagesAllowedForUrls](/deployedge/microsoft-edge-policies#imagesallowedforurls), [ImagesBlockedForUrls](/deployedge/microsoft-edge-policies#imagesblockedforurls), [InsecureContentAllowedForUrls](/deployedge/microsoft-edge-policies#insecurecontentallowedforurls), [InsecureContentBlockedForUrls](/deployedge/microsoft-edge-policies#insecurecontentblockedforurls), [PopupsAllowedForUrls](/deployedge/microsoft-edge-policies#popupsallowedforurls), [PopupsBlockedForUrls](/deployedge/microsoft-edge-policies#popupsblockedforurls).

### Feature updates

- **Update to Microsoft Edge supported operating systems.** The minimum supported macOS version is increased to macOS 11. Users on older versions of macOS will no longer receive Microsoft Edge updates. For more information, see [Microsoft Edge Supported Operating Systems](/DeployEdge/microsoft-edge-supported-operating-systems).

- **Deprecation of the CryptoWallet feature.** To improve end user experience, the CryptoWallet feature and the [CryptoWalletEnabled](/deployedge/microsoft-edge-policies#cryptowalletenabled) policy is deprecated. The [CryptoWalletEnabled](/deployedge/microsoft-edge-policies#cryptowalletenabled) policy will be obsolete in an upcoming release.

- **Microsoft Edge sidebar updates.** For inactive sidebar users and new Microsoft Edge users, the sidebar is turned OFF. Users can always return to the **Settings** > **Sidebar** and turn the sidebar ON again at any time. For active sidebar users, the current sidebar state remains the same.
  
  Administrators can control the availability of the sidebar using the [HubsSidebarEnabled](/deployedge/microsoft-edge-policies#hubssidebarenabled) policy. **Note:** This feature is a controlled feature rollout. If you don't see this feature, check back as we continue our rollout.

### Policy updates

#### Deprecated policies

- [CryptoWalletEnabled](/deployedge/microsoft-edge-policies#cryptowalletenabled)  - Enable CryptoWallet feature (deprecated)
- [EnhanceSecurityModeOptOutUXEnabled](/deployedge/microsoft-edge-policies#enhancesecuritymodeoptoutuxenabled)  - Manage opt-out user experience for Enhanced Security Mode (ESM) in Microsoft Edge (deprecated)

<!-- Version 127.0.2651.111 (Android and iOS): August 20, 2024 to Version 127.0.2651.81 (iOS): July 31, 2024 --->

## Version 127.0.2651.111 (Android and iOS): August 20, 2024

Fixed various bugs and performance issues.

## Version 127.0.2651.102 (Android and iOS): August 13, 2024

Fixed various bugs and performance issues.

## Version 127.0.2651.96 (iOS): August 8, 2024

Fixed various bugs and performance issues.

## Version 127.0.2651.90 (Android): August 6, 2024

Fixed various bugs and performance issues.

## Version 127.0.2651.82 (Android): August 1, 2024

Fixed various bugs and performance issues, general updates, and new policies.

### General updates

- [Android] Exclude Microsoft Entra ID Copilot from NTP's voice and camera search

### Bug fixes

- [Android] Fix a bug related to policy InPrivateModeAvailability
- [Android] Fix SSO bug when a blocked link is opened from Outlook

### New policies

- [Android] Disable UIR prompt pop-up via `com.microsoft.intune.mam.managedbrowser.disabledFeatures` or [EdgeDisabledFeatures](/deployedge/microsoft-edge-mobile-policies#edgedisabledfeatures) policy
- [Android] Add CIDR (Classless Inter-domain Routing) support in AllowListURLs/BlockListURLs feature
- [Android] New `com.microsoft.intune.mam.managedbrowser.InternalPagesBlockList` policy to allow IT admin disable edge internal pages

## Version 127.0.2651.81 (iOS): July 31, 2024

Fixed various bugs and performance issues, general updates, new policies, and enhancements.

### Bug fixes

- [iOS] Fix [DefaultBrowserSettingEnabled](/deployedge/microsoft-edge-mobile-policies#defaultbrowsersettingenabled) policy that didn't work
- [iOS] Fix the UI layout issue caused by changes in UIWindow safeAreaInsets leading to Webview content offset shift in certain situations

### General updates

- [iOS] Upgrade MS Tunnel SDK version 1.0.18
- [iOS] Upgrade Intune MAM SDK to version 19.4.1

### New policies

- [iOS] Disable UIR prompt pop-up via `com.microsoft.intune.mam.managedbrowser.disabledFeatures` or [EdgeDisabledFeatures](/deployedge/microsoft-edge-mobile-policies#edgedisabledfeatures) policy
- [iOS] Add CIDR (Classless Inter-domain Routing) support in AllowListURLs/BlockListURLs feature
- [iOS] New `com.microsoft.intune.mam.managedbrowser.InternalPagesBlockList` policy to allow IT admin disable edge internal pages

### Enhancements

- [iOS] Shared device mode support is generally available.

<!-- Version 126.2592.120 (iOS): July 24, 2024 to Version 126.0.2592.56 (Android and iOS): June 17, 2024 -->

## Version 126.2592.120 (iOS): July 24, 2024

Fixed various bugs and performance issues.

## Version 126.0.2592.117 (Android): July 23, 2024

Fixed various bugs and performance issues.

## Version 126.0.2592.106 (Android and iOS): July 16, 2024

Fixed various bugs and performance issues.

## Version 126.0.2592.100 (Android and iOS): July 11, 2024

Fixed various bugs and performance issues.

## Version 126.0.2592.86 (Android and iOS): July 2, 2024

Fixed various bugs and performance issues.

## Version 126.0.2592.80 (Android): June 27, 2024

Fixed various bugs and performance issues.

## Version 126.0.2592.74 (Android): June 25, 2024

Fixed various bugs and performance issues.

## Version 126.0.2592.56 (Android and iOS): June 17, 2024

Fixed various bugs and performance issues, made general updates, added policies and enhancements.

### General updates

- [iOS] Upgrade MS Tunnel SDK version 1.1.0
- [Android and iOS] Update OneAuth SDK to 2.3.1

### Bug fixes

- [Android] Scrolling screenshot will be disabled if Intune APP (App Protection Policy) is configured to block screenshot.

### New policies

- [Android and iOS] Manage contextual search via policy `com.microsoft.intune.mam.managedbrowser.disabledFeatures=contextualsearch`
- [iOS] Introduce MDM policy **EdgeSharedDeviceSupportEnabled** to disable shared device mode.

### Enhancements

- [Android and iOS] Remove [Copilot](https://copilot.microsoft.com/#/) from default allowlist so that you can manage access to [Copilot](https://copilot.microsoft.com/#/) via URLs blocklist.
- [iOS] Support Passkey on iOS. This feature is disabled by default. It can be enabled by turning on the `flag edge-iOS-enable-passkey-signin` from *Edge://flags*.

<!-- Version 125.0.2535.96 (Android and iOS): June 11, 2024 to Version 125.0.2535.51 (Android): May 21, 2024 --->

## Version 125.0.2535.96 (Android and iOS): June 11, 2024

Fixed various bugs and performance issues.

## Version 125.0.2535.87 (Android and iOS): June 5, 2024

Fixed various bugs and performance issues.

## Version 125.0.2535.72 (Android and iOS): May 27, 2024

Fixed various bugs and performance issues.

## Version 125.0.2535.60 (iOS): May 23, 2024

Fixed various bugs and performance issues, provide general updates, add new features and policies.

### General updates

- MS Tunnel SDK updated to 1.0.17.
- Upgrade Intune iOS SDK to 19.3.1, with working time support.

### New features

- Shared links feature appears in overflow menu in work account. 
- PAC policy now supports fail-close.
- Support certificate pinning via Intune, currently only supports limited number of Microsoft domains. Pending on Intune's improvements to support customizable cert-domain pair.
- Support of new iOS 17 relay proxy via policy `com.microsoft.intune.mam.managedbrowser.ProxyRelayUrl`.

### New Policies

- `com.microsoft.intune.mam.managedbrowser.ProfileAutoSwitchToWork` to resolve the conflict between Intune auto identity switch and Edge allow/block URL policies.
- Introduce MDM policy [EdgeCopilotEnabled](/deployedge/microsoft-edge-mobile-policies#edgecopilotenabled), to globally disable Copilot in Edge mobile, including the personal context.

## Version 125.0.2535.51 (Android): May 21, 2024

Fixed various bugs and performance issues, provide a general update, add new features and policies.

### General updates

- Upgrade the Intune Android SDK to 10.3.0, with working time support.

### New features

- Edge Android now supports kerberos/negotiate authentication on Android via an [external SPNEGO authenticator app](https://github.com/google/android-kerberos-authenticator) integrated with Android account management framework.
- Shared links feature appears in overflow menu in work account.

### New Policies

- Introduce the MDM policy [EdgeCopilotEnabled](/deployedge/microsoft-edge-mobile-policies#edgecopilotenabled), to globally disable Copilot in Edge mobile, including the personal context.

<!-- Version 124.0.2478.105 (iOS): May 17, 2024 to Version 124.0.2478.50 (Android and iOS): April 22, 2024 -->

## Version 124.0.2478.105 (iOS): May 17, 2024

Fixed various bugs and performance issues.

## Version 124.0.2478.104 (Android): May 15, 2024

Fixed various bugs and performance issues.

## Version 124.0.2478.89 (iOS): May 8, 2024

Fixed various bugs and performance issues.

## Version 124.0.2478.87 (Android): May 7, 2024

Fixed various bugs and performance issues.

## Version 124.0.2478.71 (iOS): April 30, 2024

Fixed various bugs and performance issues.

## Version 124.0.2478.71 (Android): April 29, 2024

### Policy updates

- MDM policy  [edgenewtabpagelayout](/deployedge/microsoft-edge-mobile-policies#edgenewtabpagelayout) to manage New Tab Page layout settings.
- MDM policy [edgenewtabpagelayoutcustom](/deployedge/microsoft-edge-mobile-policies#edgenewtabpagelayoutcustom) to manage New Tab Page custom setting.
- MDM policy [edgenewtabpagelayoutuserselectable](/deployedge/microsoft-edge-mobile-policies#edgenewtabpagelayoutuserselectable) to manage whether the New Tab Page layout is selectable by users.

Fixed various bugs and performance issues.

## Version 124.0.2478.62 (Android): April 25, 2024

Fixed various bugs and performance issues.

### Bug fixes

- [Android] Fixed a bug where setting Edge as the default browser caused repetition, and the button became unresponsive.
- [Android] Fixed a bug in shared device mode where the sign-in process was getting hung on the loading screen.

## Version 124.0.2478.50 (Android and iOS): April 22, 2024

Made general updates, fixed various bugs and performance issues, added new features and policies.

### General updates

- [iOS] MS Tunnel updated to 1.0.15, added privacy manifest file to comply with Apple App Store requirements.
- [iOS] updated Citrix mVPN iOS SDK to 24.2.1
- [iOS] added 'protApp' parameter to Microsoft Bing Search resource token fetch request, so it is not blocked by the CA "requiring app protection" policy. This token is needed for Copilot in Edge
- [iOS] Intune SDK updated to 19.2.0

### Bug fixes

- [iOS] Fix disableFeatures policy bug for inPrivate mode, handle corner cases where inPrivate not disabled
- [Android] Fixed a bug in Guided switch

### New features

- [Android] Re-enable Kerberos authentication support on Android with an external Negotiate Authenticator app.
- [Android and iOS] Copilot in Edge mobile now properly supports school scenarios.
- [iOS] Shared Device Mode support
- [Android and iOS] In-flight, the "Shared Links" feature can be opened from the Edge overflow menu.

### Policy updates

- [Android and iOS] Introduce MDM policy [EdgeCopilotEnabled](/deployedge/microsoft-edge-mobile-policies#edgecopilotenabled), to globally disable Copilot in Edge mobile, including the personal context.
- [Android and iOS] MDM policy [HideFirstRunExperience](/deployedge/microsoft-edge-mobile-policies#hidefirstrunexperience), to hide first run experience.
- [Android and iOS] MDM policy [DefaultBrowserSettingEnabled](/deployedge/microsoft-edge-mobile-policies#defaultbrowsersettingenabled), to disable default browser settings pop-up.
- [Android] MDM policy [PreventTyposquattingPromptOverride](/deployedge/microsoft-edge-mobile-policies#preventtyposquattingpromptoverride), to prevent bypassing Edge Website Typo Protection prompts for sites.
- [Android] MDM policy [TyposquattingAllowListDomains](/deployedge/microsoft-edge-mobile-policies#typosquattingallowlistdomains), to configure the list of domains for which Edge Website Typo Protection won't trigger warnings.

<!-- Version 123.0.2420.108 (iOS): April 19, 2024 to Version 123.0.2420.56 (iOS): March 25, 2024 -->

## Version 123.0.2420.108 (iOS): April 19, 2024

Fixed various bugs and performance issues.

### Bug fixes

- Fixed a bug that pkpass files in binary data mime type were not handled correctly.

## Version 123.0.2420.102 (iOS): April 16, 2024

Fixed various bugs and performance issues.

## Version 123.0.2420.102 (Android): April 16, 2024

Fixed various bugs and performance issues.

## Version 123.0.2420.90 (iOS): April 11, 2024

Fixed various bugs and performance issues.

## Version 123.0.2420.90 (Android): April 10, 2024

Fixed various bugs and performance issues.

## Version 123.0.2420.74 (Android and iOS): April 2, 2024

Fixed various bugs and performance issues.

### General updates

- [iOS] Update Citrix mVPN SDK to version 24.2.1

### New features

- Start a flight to show Shared links entry point on the overflow menu

## Version 123.0.2420.61 (Android): March 25, 2024

Fixed various bugs and performance issues. This release includes general updates, and new policies.

### General updates

- [Android] Remove "https" scheme check for managed bookmarks to support URLs such as `edge://…`.

### Bug fixes

- [Android] Fix a bug that NLTM SSO policy doesn't work in some conditions.
- [Android] Fix issues for brand logo policy.

### Policy updates

- Introduce a policy to control the behavior of opening Intune unmanaged URL in work profile. Current behavior is "stay" and open the unmanaged URL in work profile. This policy allows admin to change behavior to switch to personal context and open the unmanaged URL.

  `com.microsoft.intune.mam.managedbrowser.ProfileAutoSwitch`
  - 0 (Default) - The URLs are opened in normal tabs with work profile
  - 1 - Edge respects Intune's protection policy, the behavior is based on the configuration of Receive data from other apps in Intune protection policy.
    - All apps - fall back to behavior for policy value 0
    - None or Policy managed apps
      - If personal profile is signed-in, the URLs are opened in normal tabs with personal profile
      - If personal profile isn't signed-in, the URLs are opened in InPrivate
      - If InPrivate is disabled, the URLs won't be opened
  - 2 (Android only) - Microsoft Edge checks **URLAllowlist** or **URLBlocklist**. Microsoft Edge opens allowed URLs in normal tabs with work profile. As for URLs in blocklist, they might or might not be opened in InPrivate or normal tabs with personal profile, it depends on how **openInPrivateIfBlocked** is configured.

## Version 123.0.2420.56 (iOS): March 25, 2024

Fixed various bugs and performance issues. This release includes general updates, new features, and new policies.

### General updates

- [iOS] Update MS Tunnel MAM SDK to 1.0.12
- [iOS] Update MS Intune MAM SDK to 19.1.0
- [iOS] "Save to OneDrive" option in Edge now has upload progress indicator.

### Bug fixes

- [iOS] URL Block policy also shows "Site blocked" alert for http POST requests.
- [iOS] Fix issues for new File upload block policy and idle timer policy.

### New features

- [iOS] Shared device mode public preview

### Policy updates

- [iOS] Introduces MAM policy to control the behavior the "Site Blocked" popup. This policy would let admins choose preferences between InPrivate and MSA if options are available.
`com.microsoft.intune.mam.managedbrowser.AutoTransitionModeOnBlock`
  - 0 (Default) - Always show choose popup windows
  - 1 - Only MSA account login, auto transition to MSA
  - 2 - When the MSA account login and InPrivate are enabled at the same time, auto transition to MSA
  - 3 - When the MSA account login and InPrivate are enabled at the same time, auto transition to InPrivate.

- [iOS] Introduce a policy to control the behavior of opening Intune unmanaged URL in work profile. Current behavior is "stay" and open the unmanaged URL in work profile. This policy allows admin to change behavior to switch to personal context and open the unmanaged URL.

  `com.microsoft.intune.mam.managedbrowser.ProfileAutoSwitch`
  - 0 (Default) - The URLs are opened in normal tabs with work profile
  - 1 - Edge respects Intune's protection policy, the behavior is based on the configuration of Receive data from other apps in Intune protection policy.
    - All apps - fall back to behavior for policy value 0
    - None or Policy managed apps
      - If personal profile is signed-in, the URLs are opened in normal tabs with personal profile
      - If personal profile isn't signed-in, the URLs are opened in InPrivate
      - If InPrivate is disabled, the URLs won't be opened

<!-- Version 122.0.2365.99 (Android and iOS): March 18, to 2024 Version 121.0.2277.84 (Android): January 29, 2024 -->

## Version 122.0.2365.99 (Android and iOS): March 18, 2024

Fixed various bugs and performance issues.

## Version 122.0.2365.86 (Android and iOS): March 12, 2024

Fixed various bugs and performance issues.

## Version 122.2365.78 (iOS): March 8, 2024

Fixed various bugs and performance issues.

### Fixes

- fixed a crash issue

## Version 122.0.2365.76 (Android): March 7, 2024

Fixed various bugs and performance issues.

### Feature update

- Extensions in Edge for Android can be disabled by MAM policy.
  - `com.microsoft.intune.mam.managedbrowser.disabledFeatures=extensions`

  Note: The Extensions feature is still in flight. It can be turned on by the Android Extension flag from *Edge://flags*.

## Version 122.2365.71 (iOS): March 6, 2024

Fixed various bugs and performance issues.

## Version 122.0.2365.56 (Android and iOS): February 26, 2024

Made general updates, fixed various bugs, and added new policy support.

### General updates

- Updated the Intune Mobile Application Management (MAM) SDK to version 19.1.0.
- With the release of iOS 17, multiple persistent stores are now supported. Work and personal accounts have their own designated persistent store. The MAM policy [`com.microsoft.intune.mam.managedbrowser.PersistentWebsiteDataStore`](/mem/intune/apps/manage-microsoft-edge#ios-website-data-store) is no longer applicable.

### Bug fixes

- Fixed crash with Microsoft MAM Tunnel
- Fixed bug for MDM policy EdgeBlockSignInEnabled
- Addressed accessibility and UI issues related to implicit sign-in.
- Resolved several policy-related crashes and performance issues.
- [iOS] Fixed a bug preventing deep links from opening via `window.open()`.
- [iOS] Resolved an issue where the Intune SDK unexpectedly blocked "Open in Microsoft Edge".
- [iOS] Resolved an issue with closing tabs in InPrivate mode.

### Policy updates

- [iOS] Mobile Application Management (MDM) policy IdleTimeoutActions to specify actions to run when the timeout from the IdleTimeout policy is reached. Only close_tabs is supported.
- [iOS] MDM policy IdleTimeout to specify the length of time without user input (in minutes) before the browser runs actions configured via the IdleTimeoutActions policy.
- MAM policy to allow or block file uploads to specified domains.
  - `com.microsoft.intune.mam.managedbrowser.FileUploadBlockedForUrls`
  - `com.microsoft.intune.mam.managedbrowser.FileUploadAllowedForUrls`

## Version 121.0.2277.133: February 20, 2024

Fixed various bugs and performance issues for Android and iOS.

## Version 121.0.2277.107 (iOS): February 7, 2024

Fixed various bugs and performance issues.

## Version 121.0.2277.99 (iOS): February 6, 2024

Fixed various bugs and performance issues.

## Version 121.0.2277.105 (Android): February 5, 2024

Fixed various bugs and performance issues.

## Version 121.0.2277.86 (iOS): February 1, 2024

Fixed various bugs, added new policy support, and enhanced users' experience.

### Fixes

**iOS:**

- Resolved the issue with the "Open in Microsoft Edge" option not functioning due to Intune SDK problem.
- Upgraded Microsoft Tunnel MAM SDK to version 1.0.11.
- Fixed a background crash related to the policy manager.
- Upgraded Intune MAM SDK for iOS to version 19.0.0.

### Policy updates

#### New policies

- [EdgeBlockSignInEnabled](/deployedge/microsoft-edge-mobile-policies#edgeblocksigninenabled) to block Edge sign-in
- [ExperimentationAndConfigurationServiceControl](/deployedge/microsoft-edge-mobile-policies#experimentationandconfigurationservicecontrol), allowing customers to opt-in for experiments and gain early access to Microsoft Edge experimenting features.

### Enhancements

- News feeds is enabled for work or school accounts.

<!-- =================================================== -->
## Version 121.0.2277.84 (Android): January 29, 2024

Fixed various bugs, added new policy support, and enhanced users' experience.

### Fixes

**Android:**

- Fixed bugs related to bookmarks.
- Upgraded Intune MAM SDK to version 10.1.0.
 
### Policy updates

#### New policies

- [EdgeBlockSignInEnabled](/deployedge/microsoft-edge-mobile-policies#edgeblocksigninenabled) to block Edge sign-in
- [ExperimentationAndConfigurationServiceControl](/deployedge/microsoft-edge-mobile-policies#experimentationandconfigurationservicecontrol), allowing customers to opt-in for experiments and gain early access to Microsoft Edge experimenting features.
- [EdgeOneAuthProxy](/deployedge/microsoft-edge-mobile-policies#edgeoneauthproxy) to specify a dedicated proxy to sign in to Edge in Android

### Enhancements

- News feeds is enabled for work or school accounts.

<!-- Version 120.0.2210.150: January 21, 2024 to Version 120.0.2210.59: December 12, 2023 -->
## Version 120.0.2210.150: January 21, 2024

Fixed various bugs and performance issues for Android and iOS.

## Version 120.0.2210.141: January 17, 2024

Fixed various bugs and performance issues for Android and iOS.

## Version 120.0.2210.126: January 9, 2024

Fixed various bugs and performance issues for Android and iOS.

## Version 120.0.2210.115: January 5, 2024

Fixed various bugs and performance issues for Android.

## Version 120.0.2210.116: January 2, 2024

Fixed various bugs and performance issues for iOS.

## Version 120.0.2210.105: December 29, 2023

Fixed various bugs and performance issues for iOS.

## Version 120.0.2210.99: December 27, 2023

Fixed various bugs and performance issues.

**Note:** The app jump blocker feature is removed from Android and iOS.

## Version 120.0.2210.86: December 19, 2023

Fixed various bugs and performance issues for iOS.

## Version 120.0.2210.84: December 19, 2023

Fixed various bugs and performance issues for Android.

## Version 120.0.2210.78: December 15, 2023

Fixed various bugs and performance issues for iOS.

 **Note:** The default key value for [iOS Website data store](/mem/intune/apps/manage-microsoft-edge#ios-website-data-store) is changed to "2".

## Version 120.0.2210.64: December 12, 2023

Fixed various bugs and performance issues for Android.

### Policy support

For more information, see [Manage Microsoft Edge on iOS and Android with Intune](/mem/intune/apps/manage-microsoft-edge).

MAM Policy to configure search engine:

- `com.microsoft.intune.mam.managedbrowser.DefaultSearchProviderEnabled`
- `com.microsoft.intune.mam.managedbrowser.DefaultSearchProviderName`
- `com.microsoft.intune.mam.managedbrowser.DefaultSearchProviderSearchURL`

MAM Policy to configure pop-up behavior:

- `com.microsoft.intune.mam.managedbrowser.DefaultPopupsSetting`
- `com.microsoft.intune.mam.managedbrowser.PopupsAllowedForUrls`
- `com.microsoft.intune.mam.managedbrowser.PopupsBlockedForUrls`

### Policy update

#### New policies

- [EdgeBrandLogo](/deployedge/microsoft-edge-mobile-policies#edgebrandlogo) - Configure Brand logo in New Tab Page
- [EdgeBrandColor](/deployedge/microsoft-edge-mobile-policies#edgebrandcolor) - Configure Brand color in New Tab Page
- [EdgeProxyPacUrl](/deployedge/microsoft-edge-mobile-policies#edgeproxypacurl) - Specify a URL to a proxy auto-config (PAC) file
- [PopupsAllowedForUrls](/deployedge/microsoft-edge-mobile-policies#popupsallowedforurls) - Allow pop-up windows on specific sites
- [PopupsBlockedForUrls](/deployedge/microsoft-edge-mobile-policies#popupsblockedforurls) - Block pop-up windows on specific sites

## Version 120.0.2210.59: December 12, 2023

Fixed various bugs and performance issues for iOS.

### Policy support

For more information, see [Manage Microsoft Edge on iOS and Android with Intune](/mem/intune/apps/manage-microsoft-edge).

MAM Policy to configure search engine:

- `com.microsoft.intune.mam.managedbrowser.DefaultSearchProviderEnabled`
- `com.microsoft.intune.mam.managedbrowser.DefaultSearchProviderName`
- `com.microsoft.intune.mam.managedbrowser.DefaultSearchProviderSearchURL`

MAM Policy to configure pop-up behavior:

- `com.microsoft.intune.mam.managedbrowser.DefaultPopupsSetting`
- `com.microsoft.intune.mam.managedbrowser.PopupsAllowedForUrls`
- `com.microsoft.intune.mam.managedbrowser.PopupsBlockedForUrls`

### Policy update

#### New policies

- [EdgeBrandLogo](/deployedge/microsoft-edge-mobile-policies#edgebrandlogo) - Configure Brand logo in New Tab Page
- [EdgeBrandColor](/deployedge/microsoft-edge-mobile-policies#edgebrandcolor) - Configure Brand color in New Tab Page
- [EdgeProxyPacUrl](/deployedge/microsoft-edge-mobile-policies#edgeproxypacurl) - Specify a URL to a proxy auto-config (PAC) file
- [PopupsAllowedForUrls](/deployedge/microsoft-edge-mobile-policies#popupsallowedforurls) - Allow pop-up windows on specific sites
- [PopupsBlockedForUrls](/deployedge/microsoft-edge-mobile-policies#popupsblockedforurls) - Block pop-up windows on specific sites

<!-- Version 119.0.2151.107: December 6, 2023 to Version 119.0.2151.46: November 7, 2023  -->
## Version 119.0.2151.107: December 6, 2023

Fixed various bugs and performance issues for Android.

## Version 119.0.2151.105: December 5, 2023

Fixed various bugs and performance issues for iOS.

## Version 119.0.2151.96: November 30, 2023

Fixed various bugs and performance issues for iOS.

## Version 119.0.2151.92: November 28, 2023

Fixed various bugs and performance issues for Android and iOS.

## Version 119.0.2151.78: November 21, 2023

Fixed various bugs and performance issues for Android and iOS.

## Version 119.0.2151.65: November 13, 2023

Fixed various bugs and performance issues for Android and iOS.

## Version 119.0.2151.56: November 9, 2023

Fixed various bugs and performance issues for iOS.

## Version 119.0.2151.46: November 7, 2023

Fixed various bugs and performance issues for Android.

### Policy support (Android and iOS)

Configure to turn on Microsoft Defender SmartScreen:

- MAM: [com.microsoft.intune.mam.managedbrowser.SmartScreenEnabled](/mem/intune/apps/manage-microsoft-edge#microsoft-defender-smartscreen)
- MDM: [SmartScreenEnabled](/deployedge/microsoft-edge-mobile-policies#smartscreenenabled)

Configure to turn on ManagedFavorites (bookmarks):

- MDM: [ManagedFavorites](/deployedge/microsoft-edge-mobile-policies#managedfavorites)

<!-- Version 118.0.2088.81: November 1, 2023 to Version 117.0.2045.53: October 6, 2023  -->
## Version 118.0.2088.81: November 1, 2023

Fixed various bugs and performance issues for iOS.

## Version 118.0.2088.68: October 25, 2023

Fixed various bugs and performance issues for iOS.

## Version 118.0.2088.66: October 24, 2023

Fixed various bugs and performance issues for Android.

## Version 118.0.2088.60: October 21, 2023

Fixed various bugs and performance issues for iOS.

## Version 118.0.2088.52: October 18, 2023

Fixed various bugs and performance issues.

### Feature update

- **Microsoft Tunnel for MAM strict mode.** When strict mode is turned on by MAM policy `com.microsoft.intune.mam.managedbrowser.StrictTunnelMode`, the network will be blocked until the tunnel is connected.

- **Overflow menu enablement for locked view mode.** Originally, overflow menu is disabled when Edge locked view mode is turned on by MDM policy `EdgeLockedViewMode=true`. Now, the overflow menu is enabled when Edge locked view mode is turned on.

- **Support for saving logs to local devices.** For more information, see [Diagnostic logs](/mem/intune/apps/manage-microsoft-edge#diagnostic-logs)

### Policy support

Allow proceeding from the SSL warning page:

- MAM: com.microsoft.intune.mam.managedbrowser.SSLErrorOverrideAllowed (Android only)
- MDM: [SSLErrorOverrideAllowed](/deployedge/microsoft-edge-mobile-policies#sslerroroverrideallowed)

Control the behavior of opening external apps:

- MAM: [com.microsoft.intune.mam.managedbrowser.OpeningExternalApps](/mem/intune/apps/manage-microsoft-edge#block-opening-external-apps)

## Version 117.0.2045.65: October 11, 2023

Fixed various bugs and performance issues.

## Version 117.0.2045.53: October 6, 2023

Fixed various bugs and performance issues for Android.

<!-- Version 117.0.2045.33: September 15, 2023 to Version 116.0.1938.64: August 30, 2023  -->
## Version 117.0.2045.33: September 15, 2023

Fixed various bugs and performance issues for iOS.

### Feature update

- **Support for iOS 17.** Microsoft Edge for iOS supports iOS 17.

- **Shared Links feature.** This feature is released in Edge for Android as a public preview. By default, the shared links feature is turned off. It can be turned on by enabling the shared links flag in `Edge://flags`.

- **Edge shopping/coupons can be managed by MAM policy.** For example, to enable coupons: `com.microsoft.intune.mam.managedbrowser.disabledFeatures=coupons`.

- **New policy to manage the "import password" feature in MAM and MDM.** The following settings are available to manage this feature:

  - MAM: `com.microsoft.intune.mam.managedbrowser.disableImportPasswords`
  - MDM: `EdgeImportPasswordsDisabled`

- **Improvements to Bing Chat Enterprise for iOS and Android** For example, Bing Image Creator and Bing Visual Search.

## Version 116.0.1938.72: September 5, 2023

Fixed various bugs and performance issues for iOS.

### Feature update

This iOS version introduces a new MAM policy. This MAM policy controls whether Bing Chat Enterprise (BCE) can access content protected by an Intune App protection policy. When the policy is set to true, users can copy text from a protected web page and paste it into BCE. BCE can also access the page if users ask a question like "Summarize the current web page". The policy and its settings are as follows:<br>
`com.microsoft.intune.mam.managedbrowser.ChatAllowManagedContent=true (default)/false`.

## Version 116.0.1938.64: August 30, 2023

Fixed various bugs and performance issues.

### Feature update

- **Bing Chat Enterprise (BCE)** is available on Edge mobile for iOS and Android. By default, Bing Chat Enterprise is turned on. For detailed information about how to manage BCE, see [Bing Chat Enterprise](/mem/intune/apps/manage-microsoft-edge#bing-chat-enterprise).

<!-- Version 116.0.1938.56: August 21, 2023, to Version 115.0.1901.183: July 22, 2023 -->
## Version 116.0.1938.56: August 21, 2023

Fixed various bugs and performance issues for iOS.

### Feature updates

- Bing Chat Enterprise (BCE) is available on Edge mobile. By default, Bing Chat Enterprise is turned off. It can be turned on via Intune MAM policy `com.microsoft.intune.mam.managedbrowser.Chat=true`.

- The **Open in Microsoft Edge** option is available for saving files to OneDrive (Android).

- Brand info (logo) of New Tab Page (NTP) is now pulled from MS Graph. If you only configure brand logo in the Intune portal, you must also configure it in the Azure portal. For more information, see [Add company branding - Basics](/azure/active-directory/fundamentals/how-to-customize-branding#basics).

- InPrivate mode can be managed by Mobile Device Management (MDM) Policy setting for [InPrivateModeAvailability](/deployedge/microsoft-edge-mobile-policies#inprivatemodeavailability).

## Version 116.0.1938.53: August 21, 2023

Fixed various bugs and performance issues for Android.

## Version 115.0.1901.187: July 27, 2023

Fixed various bugs and performance issues for iOS.

## Version 115.0.1901.183: July 22, 2023

Fixed various bugs and performance issues for Android.

This release contains several security fixes for Android. For more information, see the [Security Update Guide](https://msrc.microsoft.com/update-guide).


<!-- Version 114.0.1823.37: June 2, 2023 to Version 113.0.1774.50: May 18, 2023 -->
## Version 114.0.1823.37: June 2, 2023

Fixed various bugs and performance issues.

### Policy update

- **iOS Website data store access.** Currently, the persistent data store is only statically used by personal accounts. Because work or school accounts can't use this data store, browsing data rather than cookies are lost when their sessions end. This new policy lets organizations access the data store dynamically, which persists browsing data for work or school accounts, giving users a better browsing experience. For more information, see this policy in [Manage Microsoft Edge on iOS and Android with Intune](/mem/intune/apps/manage-microsoft-edge#ios-website-data-store).

## Version 113.0.1774.50: May 18, 2023

Fixed various bugs and performance issues.

This release contains several security fixes for Android. For more information, see the [Security Update Guide](https://msrc.microsoft.com/update-guide).

<!-- Version 113.1774.36: May 8, 2023 to Version 112.0.1722.36: April 7, 2023 -->
## Version 113.1774.36: May 8, 2023

Fixed various bugs and performance issues.

### Feature updates

- **Open in Microsoft Edge option (iOS only).** This option is available for saving files to OneDrive.

- **Net-export supports open-in (iOS only).** This option now supports open-in instead of using the native mail app.

- **Shared Device Mode (SDM) for Edge mobile.** Generally available for Android.

## Version 112.0.1722.54: April 19, 2023

Fixed various bugs and performance issues.

This release contains several security fixes for Android. For more information, see the [Security Update Guide](https://msrc.microsoft.com/update-guide).

## Version 112.0.1722.44: April 12, 2023

Fixed various bugs and performance issues for iOS.

## Version 112.0.1722.36: April 7, 2023

Fixed various bugs and performance issues for Android.

### Feature updates

- **Translator, Read Aloud, Drop and developer tools (Android only).** These tools can be managed by Mobile Application Management (MAM) [disabledFeatures](/mem/intune/apps/manage-microsoft-edge#disable-specific-features) and the Mobile Device Management (MDM) policy, [EdgeDisabledFeatures](/deployedge/microsoft-edge-mobile-policies#edgedisabledfeatures).


<!-- Version 111.0.1661.43: March 18, 2023 to Version 109.0.1518.70: January 26, 2023 -->
## Version 111.0.1661.43: March 18, 2023

Fixed various bugs and performance issues.

### Feature updates

- **Support saving files to OneDrive for Business.** Save files securely with the Intune App Protection Policy. For more information, see [App protection policies overview](/mem/intune/apps/app-protection-policy).

- **Edge-specific policies are supported in the MDM channel.** These policies are now supported in version 111. For more information, see [Edge Specific](/deployedge/microsoft-edge-mobile-policies#edge-specific).

## Version 110.0.1587.61: March 1, 2023

Fixed various bugs and performance issues for Android.

## Version 110.0.1587.54: February 21, 2023

Fixed various bugs and performance issues.

### Feature updates

- **Microsoft Edge for iOS supports Microsoft Tunnel for MAM solution.** For more information, see [Learn about using Microsoft Tunnel with Mobile Application Management](/mem/intune/protect/microsoft-tunnel-mam).

## Version 109.0.1518.70: January 26, 2023

Fixed various bugs and performance issues.

This release contains several security fixes for iOS and Android. For more information, see the [Security Update Guide](https://msrc.microsoft.com/update-guide).

<!-- Version 109.0.1518.58: January 18, 2023 to Version 108.0.1462.45: December 8, 2022  -->
## Version 109.0.1518.58: January 18, 2023

Fixed various bugs and performance issues for Android.

> [!NOTE]
> Release version 109 supports more than 30 policies. For more information, see [Microsoft Edge Mobile - Policies](/deployedge/microsoft-edge-mobile-policies).

## Version 108.0.1462.77: January 6, 2023

Fixed various bugs and performance issues for iOS.

## Version 108.0.1462.62: December 21, 2022

Fixed various bugs and performance issues.

## Version 108.0.1462.48: December 12, 2022

Fixed various bugs and performance issues for Android.

## Version 108.0.1462.45: December 8, 2022

Fixed various bugs for Android.

### Feature updates

- **Support Shared Device Mode (Android only).** Starting with Microsoft Edge 108 for Android, shared device mode will be supported as public preview. For more information, see [Microsoft applications that support shared device mode](/azure/active-directory/develop/msal-android-shared-devices#microsoft-applications-that-support-shared-device-mode).

## Version 108.0.1462.43: December 7, 2022

Fixed various bugs and performance issues for iOS.

## Version 107.0.1418.52: November 17, 2022

Fixed various bugs and performance issues.

## Version 107.0.1418.42: November 14, 2022

Fixed various bugs and performance issues.

## Version 107.0.1418.36: November 4, 2022

Fixed various bugs and performance issues.

## Version 107.0.1418.33: November 2, 2022

Fixed various bugs and performance issues.

## Version 107.0.1418.28: November 2, 2022

Fixed various bugs and performance issues.

## Version 106.0.1370.52: October 20, 2022

Fixed various bugs and performance issues.

## Version 106.0.1370.47: October 17, 2022

Fixed various bugs and performance issues.

## Version 105.0.1343.38: September 13, 2022

Fixed various bugs.

## Version 104.0.1293.60: August 17, 2022

> [!IMPORTANT]
> This update contains a fix for [CVE-2022-2856](https://msrc.microsoft.com/update-guide/vulnerability/CVE-2022-2856), which has been reported by the Chromium team as having an exploit in the wild. For more information, see the [Security Update Guide](https://msrc.microsoft.com/update-guide).

Stable channel security updates are listed [here](/deployedge/microsoft-edge-relnotes-security#august-17-2022).

## Version 104.0.1293.58: August 16, 2022

Fixed various bugs.

### Feature updates

- **Support for disabling of inPrivate browsing and Password feature (iOS and Android).**  Before Microsoft Edge 104, Edge for iOS and Android disabled InPrivate browsing and Password (prompts to save passwords for the user) by default when only allow Work or School Accounts is configured.<br><br>
Starting with Microsoft Edge 104, you have more flexibility because InPrivate and Password won't be disabled by default when only allow Work or School Accounts is configured. Instead, you can decide whether to disable InPrivate browsing or Password by configuring the **com.microsoft.intune.mam.managedbrowser.disabledFeatures** key. For more information, see [Disable specific features](/mem/intune/apps/manage-microsoft-edge#disable-specific-features).

## Version 103.1264.53: July 1, 2022

Fixed various bugs.

## Version 103.0.1264.38: June 30, 2022

Fixed various bugs.

## Version 102.0.1245.30: May 31, 2022

Fixed various bugs.

### Feature updates

- **Support switching network stack between Chromium and iOS (iOS only).** The [NetworkStackPref](/mem/intune/apps/manage-microsoft-edge#switch-network-stack-between-chromium-and-ios) policy lets you choose the network preference for Microsoft Edge for iOS.

### Policy updates

#### New policies

- [NetworkStackPref](/mem/intune/apps/manage-microsoft-edge#switch-network-stack-between-chromium-and-ios) - Choose the network preference for Microsoft Edge for iOS

## Version 101.0.1210.43: May 9, 2022

Fixed various bugs.

## Version 101.0.1210.32: April 29, 2022

Fixed various bugs.

### Feature updates

- **Read Aloud: background play and play in silent mode (iOS and Android)**
  - When playing in the background, users can control Read Aloud (pause, resume, play forwards, or play backwards) via the notification panel and lock screen.
  - When a user switches tabs in Microsoft Edge while using Read Aloud, they can use a floating control bar to pause, resume, or close Read Aloud.
  - When a device's silent toggle is on, it doesn't affect Read Aloud playback as long as media volume is turned up.
  
