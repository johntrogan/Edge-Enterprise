---
title: "Microsoft Edge Browser Policy Documentation"
ms.author: jalam
author: vmliramichael
manager: nuyunzhang
ms.date: 04/22/2025
audience: ITPro
ms.topic: reference
ms.service: microsoft-edge
ms.localizationpriority: high
ms.collection: M365-modern-desktop
ms.custom:
description: "Windows and Mac documentation for all policies supported by the Microsoft Edge Browser"
---

# Microsoft Edge - Policies

The latest version of Microsoft Edge includes the following policies. You can use these policies to configure how Microsoft Edge runs in your organization. For information about an additional set of policies used to control how and when Microsoft Edge is updated, check out [Microsoft Edge update policy reference](microsoft-edge-update-policies.md).

You can download the [Microsoft Security Compliance Toolkit](https://www.microsoft.com/download/details.aspx?id=55319) for the recommended security configuration baseline settings for Microsoft Edge. For more information see the [Microsoft Security Baselines Blog](https://techcommunity.microsoft.com/t5/microsoft-security-baselines/bg-p/Microsoft-Security-Baselines).

Starting in Microsoft Edge version 116, certain policies will not be applied to a profile that is signed in with a Microsoft account. For more information, please check an individual policy for details on whether it applies to a profile that is signed in with a Microsoft account.

> [!Note]
> This article applies to Microsoft Edge version 77 or later.

## New policies

There are no new policies in Microsoft Edge version 137.

The following table lists the new policies for Microsoft Edge version 136.

|Policy Name|Caption|
|-|-|
|[PasswordExportEnabled](microsoft-edge-browser-policies/PasswordExportEnabled.md)|Enable exporting saved passwords from Password Manager|
|[ProfileTypeInProfileButtonEnabled](microsoft-edge-browser-policies/ProfileTypeInProfileButtonEnabled.md)|Controls the display of the profile button label for the work or school profile|
|[HttpsUpgradesEnabled](microsoft-edge-browser-policies/HttpsUpgradesEnabled.md)|Enable automatic HTTPS upgrades|

## Deprecated policies

The following table lists all deprecated policies.

|Policy Name|Caption|
|-|-|
|[ProxyBypassList](microsoft-edge-browser-policies/ProxyBypassList.md)|Configure proxy bypass rules (deprecated)|
|[ProxyMode](microsoft-edge-browser-policies/ProxyMode.md)|Configure proxy server settings (deprecated)|
|[ProxyPacUrl](microsoft-edge-browser-policies/ProxyPacUrl.md)|Set the proxy .pac file URL (deprecated)|
|[ProxyServer](microsoft-edge-browser-policies/ProxyServer.md)|Configure address or URL of proxy server (deprecated)|
|[AddressBarMicrosoftSearchInBingProviderEnabled](microsoft-edge-browser-policies/AddressBarMicrosoftSearchInBingProviderEnabled.md)|Enable Microsoft Search in Bing suggestions in the address bar (deprecated)|
|[AllowGamesMenu](microsoft-edge-browser-policies/AllowGamesMenu.md)|Allow users to access the games menu (deprecated)|
|[AutomaticHttpsDefault](microsoft-edge-browser-policies/AutomaticHttpsDefault.md)|Configure Automatic HTTPS (deprecated)|
|[BackgroundTemplateListUpdatesEnabled](microsoft-edge-browser-policies/BackgroundTemplateListUpdatesEnabled.md)|Enables background updates to the list of available templates for Collections and other features that use templates (deprecated)|
|[ForceCertificatePromptsOnMultipleMatches](microsoft-edge-browser-policies/ForceCertificatePromptsOnMultipleMatches.md)|Configure whether Microsoft Edge should automatically select a certificate when there are multiple certificate matches for a site configured with "AutoSelectCertificateForUrls" (deprecated)|
|[InsecureFormsWarningsEnabled](microsoft-edge-browser-policies/InsecureFormsWarningsEnabled.md)|Enable warnings for insecure forms (deprecated)|
|[MicrosoftOfficeMenuEnabled](microsoft-edge-browser-policies/MicrosoftOfficeMenuEnabled.md)|Allow users to access the Microsoft Office menu (deprecated)|
|[NativeWindowOcclusionEnabled](microsoft-edge-browser-policies/NativeWindowOcclusionEnabled.md)|Enable Native Window Occlusion (deprecated)|
|[PromotionalTabsEnabled](microsoft-edge-browser-policies/PromotionalTabsEnabled.md)|Enable full-tab promotional content (deprecated)|
|[RendererCodeIntegrityEnabled](microsoft-edge-browser-policies/RendererCodeIntegrityEnabled.md)|Enable renderer code integrity (deprecated)|
|[ShowOfficeShortcutInFavoritesBar](microsoft-edge-browser-policies/ShowOfficeShortcutInFavoritesBar.md)|Show Microsoft Office shortcut in favorites bar (deprecated)|
|[UnthrottledNestedTimeoutEnabled](microsoft-edge-browser-policies/UnthrottledNestedTimeoutEnabled.md)|JavaScript setTimeout will not be clamped until a higher nesting threshold is set (deprecated)|
|[WebWidgetAllowed](microsoft-edge-browser-policies/WebWidgetAllowed.md)|Enable the Search bar (deprecated)|

## Obsolete policies

The following table lists the obsoleted policies for Microsoft Edge version 137.

|Policy Name|Caption|
|-|-|
|[MutationEventsEnabled](microsoft-edge-browser-policies/MutationEventsEnabled.md)|Enable deprecated/removed Mutation Events (obsolete)|

The following table lists the obsoleted policies for Microsoft Edge version 136.

|Policy Name|Caption|
|-|-|
|[EnhanceSecurityModeOptOutUXEnabled](microsoft-edge-browser-policies/EnhanceSecurityModeOptOutUXEnabled.md)|Manage opt-out user experience for Enhanced Security Mode (ESM) in Microsoft Edge (obsolete)|
|[NewBaseUrlInheritanceBehaviorAllowed](microsoft-edge-browser-policies/NewBaseUrlInheritanceBehaviorAllowed.md)|Allows enabling the feature NewBaseUrlInheritanceBehavior (obsolete)|
|[RSAKeyUsageForLocalAnchorsEnabled](microsoft-edge-browser-policies/RSAKeyUsageForLocalAnchorsEnabled.md)|Check RSA key usage for server certificates issued by local trust anchors (obsolete)|

## Available policies

These tables list all of the browser-related group policies available in this release of Microsoft Edge. Use the links in the table to get more details about specific policies.

- [Application Guard settings](#application-guard-settings)
- [Cast](#cast)
- [Certificate management settings](#certificate-management-settings)
- [Content settings](#content-settings)
- [Default search provider](#default-search-provider)
- [Downloads](#downloads)
- [Edge Website Typo Protection settings](#edge-website-typo-protection-settings)
- [Edge Workspaces settings](#edge-workspaces-settings)
- [Experimentation](#experimentation)
- [Extensions](#extensions)
- [Games settings](#games-settings)
- [Generative AI](#generative-ai)
- [HTTP authentication](#http-authentication)
- [Identity and sign-in](#identity-and-sign-in)
- [Idle Browser Actions](#idle-browser-actions)
- [Immersive Reader settings](#immersive-reader-settings)
- [Kiosk Mode settings](#kiosk-mode-settings)
- [Manageability](#manageability)
- [Native Messaging](#native-messaging)
- [Network settings](#network-settings)
- [PDF Reader](#pdf-reader)
- [Password manager and protection](#password-manager-and-protection)
- [Performance](#performance)
- [Permit or deny screen capture](#permit-or-deny-screen-capture)
- [Printing](#printing)
- [Private Network Request Settings](#private-network-request-settings)
- [Profile settings](#profile-settings)
- [Proxy server](#proxy-server)
- [Related Website Sets Settings](#related-website-sets-settings)
- [Scareware Blocker settings](#scareware-blocker-settings)
- [Sleeping tabs settings](#sleeping-tabs-settings)
- [SmartScreen settings](#smartscreen-settings)
- [Startup, home page and new tab page](#startup-home-page-and-new-tab-page)
- [WebRtc settings](#webrtc-settings)
- [Additional](#additional)

<a id="application-guard-settings-policies"></a>
### Application Guard settings

|Policy Name|Caption|
|-|-|
|<a id="applicationguardcontainerproxy"></a><a id="application-guard-container-proxy"></a>[ApplicationGuardContainerProxy](microsoft-edge-browser-policies/ApplicationGuardContainerProxy.md)|Application Guard Container Proxy|
|<a id="applicationguardfavoritessyncenabled"></a><a id="application-guard-favorites-sync-enabled"></a>[ApplicationGuardFavoritesSyncEnabled](microsoft-edge-browser-policies/ApplicationGuardFavoritesSyncEnabled.md)|Application Guard Favorites Sync Enabled|
|<a id="applicationguardpassivemodeenabled"></a><a id="ignore-application-guard-site-list-configuration-and-browse-edge-normally"></a>[ApplicationGuardPassiveModeEnabled](microsoft-edge-browser-policies/ApplicationGuardPassiveModeEnabled.md)|Ignore Application Guard site list configuration and browse Edge normally|
|<a id="applicationguardtrafficidentificationenabled"></a><a id="application-guard-traffic-identification"></a>[ApplicationGuardTrafficIdentificationEnabled](microsoft-edge-browser-policies/ApplicationGuardTrafficIdentificationEnabled.md)|Application Guard Traffic Identification|
|<a id="applicationguarduploadblockingenabled"></a><a id="prevents-files-from-being-uploaded-while-in-application-guard"></a>[ApplicationGuardUploadBlockingEnabled](microsoft-edge-browser-policies/ApplicationGuardUploadBlockingEnabled.md)|Prevents files from being uploaded while in Application Guard|

<a id="cast-policies"></a>
### Cast

|Policy Name|Caption|
|-|-|
|<a id="edgedisabledialprotocolforcastdiscovery"></a><a id="disable-dial-protocol-for-cast-device-discovery"></a>[EdgeDisableDialProtocolForCastDiscovery](microsoft-edge-browser-policies/EdgeDisableDialProtocolForCastDiscovery.md)|Disable DIAL protocol for cast device discovery|
|<a id="enablemediarouter"></a><a id="enable-google-cast"></a>[EnableMediaRouter](microsoft-edge-browser-policies/EnableMediaRouter.md)|Enable Google Cast|
|<a id="showcasticonintoolbar"></a><a id="show-the-cast-icon-in-the-toolbar"></a>[ShowCastIconInToolbar](microsoft-edge-browser-policies/ShowCastIconInToolbar.md)|Show the cast icon in the toolbar|

<a id="certificate-management-settings-policies"></a>
### Certificate management settings

|Policy Name|Caption|
|-|-|
|<a id="cacertificatemanagementallowed"></a><a id="allow-users-to-manage-installed-ca-certificates"></a>[CACertificateManagementAllowed](microsoft-edge-browser-policies/CACertificateManagementAllowed.md)|Allow users to manage installed CA certificates.|
|<a id="cacertificates"></a><a id="tls-server-certificates-that-should-be-trusted-by-microsoft-edge"></a>[CACertificates](microsoft-edge-browser-policies/CACertificates.md)|TLS server certificates that should be trusted by Microsoft Edge|
|<a id="cacertificateswithconstraints"></a><a id="tls-certificates-that-should-be-trusted-by-microsoft-edge-for-server-authentication-with-constraints"></a>[CACertificatesWithConstraints](microsoft-edge-browser-policies/CACertificatesWithConstraints.md)|TLS certificates that should be trusted by Microsoft Edge for server authentication with constraints|
|<a id="cadistrustedcertificates"></a><a id="tls-certificates-that-should-be-distrusted-by-microsoft-edge-for-server-authentication"></a>[CADistrustedCertificates](microsoft-edge-browser-policies/CADistrustedCertificates.md)|TLS certificates that should be distrusted by Microsoft Edge for server authentication|
|<a id="cahintcertificates"></a><a id="tls-certificates-that-are-not-trusted-or-distrusted-but-can-be-used-in-path-building-for-server-authentication"></a>[CAHintCertificates](microsoft-edge-browser-policies/CAHintCertificates.md)|TLS certificates that are not trusted or distrusted but can be used in path-building for server authentication|
|<a id="caplatformintegrationenabled"></a><a id="use-user-added-tls-certificates-from-platform-trust-stores-for-server-authentication"></a>[CAPlatformIntegrationEnabled](microsoft-edge-browser-policies/CAPlatformIntegrationEnabled.md)|Use user-added TLS certificates from platform trust stores for server authentication|

<a id="content-settings-policies"></a>
### Content settings

|Policy Name|Caption|
|-|-|
|<a id="autoselectcertificateforurls"></a><a id="automatically-select-client-certificates-for-these-sites"></a>[AutoSelectCertificateForUrls](microsoft-edge-browser-policies/AutoSelectCertificateForUrls.md)|Automatically select client certificates for these sites|
|<a id="automaticdownloadsallowedforurls"></a><a id="allow-multiple-automatic-downloads-in-quick-succession-on-specific-sites"></a>[AutomaticDownloadsAllowedForUrls](microsoft-edge-browser-policies/AutomaticDownloadsAllowedForUrls.md)|Allow multiple automatic downloads in quick succession on specific sites|
|<a id="automaticdownloadsblockedforurls"></a><a id="block-multiple-automatic-downloads-in-quick-succession-on-specific-sites"></a>[AutomaticDownloadsBlockedForUrls](microsoft-edge-browser-policies/AutomaticDownloadsBlockedForUrls.md)|Block multiple automatic downloads in quick succession on specific sites|
|<a id="automaticfullscreenallowedforurls"></a><a id="allow-automatic-full-screen-on-specified-sites"></a>[AutomaticFullscreenAllowedForUrls](microsoft-edge-browser-policies/AutomaticFullscreenAllowedForUrls.md)|Allow automatic full screen on specified sites|
|<a id="automaticfullscreenblockedforurls"></a><a id="block-automatic-full-screen-on-specified-sites"></a>[AutomaticFullscreenBlockedForUrls](microsoft-edge-browser-policies/AutomaticFullscreenBlockedForUrls.md)|Block automatic full screen on specified sites|
|<a id="cookiesallowedforurls"></a><a id="allow-cookies-on-specific-sites"></a>[CookiesAllowedForUrls](microsoft-edge-browser-policies/CookiesAllowedForUrls.md)|Allow cookies on specific sites|
|<a id="cookiesblockedforurls"></a><a id="block-cookies-on-specific-sites"></a>[CookiesBlockedForUrls](microsoft-edge-browser-policies/CookiesBlockedForUrls.md)|Block cookies on specific sites|
|<a id="cookiessessiononlyforurls"></a><a id="limit-cookies-from-specific-websites-to-the-current-session"></a>[CookiesSessionOnlyForUrls](microsoft-edge-browser-policies/CookiesSessionOnlyForUrls.md)|Limit cookies from specific websites to the current session|
|<a id="dataurlinsvguseenabled"></a><a id="data-url-support-for-svguseelement"></a>[DataUrlInSvgUseEnabled](microsoft-edge-browser-policies/DataUrlInSvgUseEnabled.md)|Data URL support for SVGUseElement|
|<a id="defaultautomaticdownloadssetting"></a><a id="default-automatic-downloads-setting"></a>[DefaultAutomaticDownloadsSetting](microsoft-edge-browser-policies/DefaultAutomaticDownloadsSetting.md)|Default automatic downloads setting|
|<a id="defaultcookiessetting"></a><a id="configure-cookies"></a>[DefaultCookiesSetting](microsoft-edge-browser-policies/DefaultCookiesSetting.md)|Configure cookies|
|<a id="defaultfilesystemreadguardsetting"></a><a id="control-use-of-the-file-system-api-for-reading"></a>[DefaultFileSystemReadGuardSetting](microsoft-edge-browser-policies/DefaultFileSystemReadGuardSetting.md)|Control use of the File System API for reading|
|<a id="defaultfilesystemwriteguardsetting"></a><a id="control-use-of-the-file-system-api-for-writing"></a>[DefaultFileSystemWriteGuardSetting](microsoft-edge-browser-policies/DefaultFileSystemWriteGuardSetting.md)|Control use of the File System API for writing|
|<a id="defaultgeolocationsetting"></a><a id="default-geolocation-setting"></a>[DefaultGeolocationSetting](microsoft-edge-browser-policies/DefaultGeolocationSetting.md)|Default geolocation setting|
|<a id="defaultimagessetting"></a><a id="default-images-setting"></a>[DefaultImagesSetting](microsoft-edge-browser-policies/DefaultImagesSetting.md)|Default images setting|
|<a id="defaultinsecurecontentsetting"></a><a id="control-use-of-insecure-content-exceptions"></a>[DefaultInsecureContentSetting](microsoft-edge-browser-policies/DefaultInsecureContentSetting.md)|Control use of insecure content exceptions|
|<a id="defaultjavascriptjitsetting"></a><a id="control-use-of-javascript-jit"></a>[DefaultJavaScriptJitSetting](microsoft-edge-browser-policies/DefaultJavaScriptJitSetting.md)|Control use of JavaScript JIT|
|<a id="defaultjavascriptoptimizersetting"></a><a id="control-use-of-javascript-optimizers"></a>[DefaultJavaScriptOptimizerSetting](microsoft-edge-browser-policies/DefaultJavaScriptOptimizerSetting.md)|Control use of JavaScript optimizers|
|<a id="defaultjavascriptsetting"></a><a id="default-javascript-setting"></a>[DefaultJavaScriptSetting](microsoft-edge-browser-policies/DefaultJavaScriptSetting.md)|Default JavaScript setting|
|<a id="defaultnotificationssetting"></a><a id="default-notification-setting"></a>[DefaultNotificationsSetting](microsoft-edge-browser-policies/DefaultNotificationsSetting.md)|Default notification setting|
|<a id="defaultpluginssetting"></a><a id="default-adobe-flash-setting-obsolete"></a>[DefaultPluginsSetting](microsoft-edge-browser-policies/DefaultPluginsSetting.md)|Default Adobe Flash setting (obsolete)|
|<a id="defaultpopupssetting"></a><a id="default-pop-up-window-setting"></a>[DefaultPopupsSetting](microsoft-edge-browser-policies/DefaultPopupsSetting.md)|Default pop-up window setting|
|<a id="defaultthirdpartystoragepartitioningsetting"></a><a id="default-setting-for-third-party-storage-partitioning"></a>[DefaultThirdPartyStoragePartitioningSetting](microsoft-edge-browser-policies/DefaultThirdPartyStoragePartitioningSetting.md)|Default setting for third-party storage partitioning|
|<a id="defaultwebbluetoothguardsetting"></a><a id="control-use-of-the-web-bluetooth-api"></a>[DefaultWebBluetoothGuardSetting](microsoft-edge-browser-policies/DefaultWebBluetoothGuardSetting.md)|Control use of the Web Bluetooth API|
|<a id="defaultwebhidguardsetting"></a><a id="control-use-of-the-webhid-api"></a>[DefaultWebHidGuardSetting](microsoft-edge-browser-policies/DefaultWebHidGuardSetting.md)|Control use of the WebHID API|
|<a id="defaultwebusbguardsetting"></a><a id="control-use-of-the-webusb-api"></a>[DefaultWebUsbGuardSetting](microsoft-edge-browser-policies/DefaultWebUsbGuardSetting.md)|Control use of the WebUSB API|
|<a id="defaultwindowmanagementsetting"></a><a id="default-window-management-permission-setting"></a>[DefaultWindowManagementSetting](microsoft-edge-browser-policies/DefaultWindowManagementSetting.md)|Default Window Management permission setting|
|<a id="filesystemreadaskforurls"></a><a id="allow-read-access-via-the-file-system-api-on-these-sites"></a>[FileSystemReadAskForUrls](microsoft-edge-browser-policies/FileSystemReadAskForUrls.md)|Allow read access via the File System API on these sites|
|<a id="filesystemreadblockedforurls"></a><a id="block-read-access-via-the-file-system-api-on-these-sites"></a>[FileSystemReadBlockedForUrls](microsoft-edge-browser-policies/FileSystemReadBlockedForUrls.md)|Block read access via the File System API on these sites|
|<a id="filesystemwriteaskforurls"></a><a id="allow-write-access-to-files-and-directories-on-these-sites"></a>[FileSystemWriteAskForUrls](microsoft-edge-browser-policies/FileSystemWriteAskForUrls.md)|Allow write access to files and directories on these sites|
|<a id="filesystemwriteblockedforurls"></a><a id="block-write-access-to-files-and-directories-on-these-sites"></a>[FileSystemWriteBlockedForUrls](microsoft-edge-browser-policies/FileSystemWriteBlockedForUrls.md)|Block write access to files and directories on these sites|
|<a id="imagesallowedforurls"></a><a id="allow-images-on-these-sites"></a>[ImagesAllowedForUrls](microsoft-edge-browser-policies/ImagesAllowedForUrls.md)|Allow images on these sites|
|<a id="imagesblockedforurls"></a><a id="block-images-on-specific-sites"></a>[ImagesBlockedForUrls](microsoft-edge-browser-policies/ImagesBlockedForUrls.md)|Block images on specific sites|
|<a id="insecurecontentallowedforurls"></a><a id="allow-insecure-content-on-specified-sites"></a>[InsecureContentAllowedForUrls](microsoft-edge-browser-policies/InsecureContentAllowedForUrls.md)|Allow insecure content on specified sites|
|<a id="insecurecontentblockedforurls"></a><a id="block-insecure-content-on-specified-sites"></a>[InsecureContentBlockedForUrls](microsoft-edge-browser-policies/InsecureContentBlockedForUrls.md)|Block insecure content on specified sites|
|<a id="intranetfilelinksenabled"></a><a id="allow-intranet-zone-file-url-links-from-microsoft-edge-to-open-in-windows-file-explorer"></a>[IntranetFileLinksEnabled](microsoft-edge-browser-policies/IntranetFileLinksEnabled.md)|Allow intranet zone file URL links from Microsoft Edge to open in Windows File Explorer|
|<a id="javascriptallowedforurls"></a><a id="allow-javascript-on-specific-sites"></a>[JavaScriptAllowedForUrls](microsoft-edge-browser-policies/JavaScriptAllowedForUrls.md)|Allow JavaScript on specific sites|
|<a id="javascriptblockedforurls"></a><a id="block-javascript-on-specific-sites"></a>[JavaScriptBlockedForUrls](microsoft-edge-browser-policies/JavaScriptBlockedForUrls.md)|Block JavaScript on specific sites|
|<a id="javascriptjitallowedforsites"></a><a id="allow-javascript-to-use-jit-on-these-sites"></a>[JavaScriptJitAllowedForSites](microsoft-edge-browser-policies/JavaScriptJitAllowedForSites.md)|Allow JavaScript to use JIT on these sites|
|<a id="javascriptjitblockedforsites"></a><a id="block-javascript-from-using-jit-on-these-sites"></a>[JavaScriptJitBlockedForSites](microsoft-edge-browser-policies/JavaScriptJitBlockedForSites.md)|Block JavaScript from using JIT on these sites|
|<a id="javascriptoptimizerallowedforsites"></a><a id="allow-javascript-optimization-on-these-sites"></a>[JavaScriptOptimizerAllowedForSites](microsoft-edge-browser-policies/JavaScriptOptimizerAllowedForSites.md)|Allow JavaScript optimization on these sites|
|<a id="javascriptoptimizerblockedforsites"></a><a id="block-javascript-optimizations-on-these-sites"></a>[JavaScriptOptimizerBlockedForSites](microsoft-edge-browser-policies/JavaScriptOptimizerBlockedForSites.md)|Block JavaScript optimizations on these sites|
|<a id="legacysamesitecookiebehaviorenabled"></a><a id="enable-default-legacy-samesite-cookie-behavior-setting-obsolete"></a>[LegacySameSiteCookieBehaviorEnabled](microsoft-edge-browser-policies/LegacySameSiteCookieBehaviorEnabled.md)|Enable default legacy SameSite cookie behavior setting (obsolete)|
|<a id="legacysamesitecookiebehaviorenabledfordomainlist"></a><a id="revert-to-legacy-samesite-behavior-for-cookies-on-specified-sites-obsolete"></a>[LegacySameSiteCookieBehaviorEnabledForDomainList](microsoft-edge-browser-policies/LegacySameSiteCookieBehaviorEnabledForDomainList.md)|Revert to legacy SameSite behavior for cookies on specified sites (obsolete)|
|<a id="notificationsallowedforurls"></a><a id="allow-notifications-on-specific-sites"></a>[NotificationsAllowedForUrls](microsoft-edge-browser-policies/NotificationsAllowedForUrls.md)|Allow notifications on specific sites|
|<a id="notificationsblockedforurls"></a><a id="block-notifications-on-specific-sites"></a>[NotificationsBlockedForUrls](microsoft-edge-browser-policies/NotificationsBlockedForUrls.md)|Block notifications on specific sites|
|<a id="partitionedbloburlusage"></a><a id="manage-blob-url-partitioning-during-fetching-and-navigation"></a>[PartitionedBlobUrlUsage](microsoft-edge-browser-policies/PartitionedBlobUrlUsage.md)|Manage Blob URL Partitioning During Fetching and Navigation|
|<a id="pluginsallowedforurls"></a><a id="allow-the-adobe-flash-plug-in-on-specific-sites-obsolete"></a>[PluginsAllowedForUrls](microsoft-edge-browser-policies/PluginsAllowedForUrls.md)|Allow the Adobe Flash plug-in on specific sites (obsolete)|
|<a id="pluginsblockedforurls"></a><a id="block-the-adobe-flash-plug-in-on-specific-sites-obsolete"></a>[PluginsBlockedForUrls](microsoft-edge-browser-policies/PluginsBlockedForUrls.md)|Block the Adobe Flash plug-in on specific sites (obsolete)|
|<a id="popupsallowedforurls"></a><a id="allow-pop-up-windows-on-specific-sites"></a>[PopupsAllowedForUrls](microsoft-edge-browser-policies/PopupsAllowedForUrls.md)|Allow pop-up windows on specific sites|
|<a id="popupsblockedforurls"></a><a id="block-pop-up-windows-on-specific-sites"></a>[PopupsBlockedForUrls](microsoft-edge-browser-policies/PopupsBlockedForUrls.md)|Block pop-up windows on specific sites|
|<a id="registeredprotocolhandlers"></a><a id="register-protocol-handlers"></a>[RegisteredProtocolHandlers](microsoft-edge-browser-policies/RegisteredProtocolHandlers.md)|Register protocol handlers|
|<a id="serialallowallportsforurls"></a><a id="automatically-grant-sites-permission-to-connect-all-serial-ports"></a>[SerialAllowAllPortsForUrls](microsoft-edge-browser-policies/SerialAllowAllPortsForUrls.md)|Automatically grant sites permission to connect all serial ports|
|<a id="serialallowusbdevicesforurls"></a><a id="automatically-grant-sites-permission-to-connect-to-usb-serial-devices"></a>[SerialAllowUsbDevicesForUrls](microsoft-edge-browser-policies/SerialAllowUsbDevicesForUrls.md)|Automatically grant sites permission to connect to USB serial devices|
|<a id="showpdfdefaultrecommendationsenabled"></a><a id="allow-notifications-to-set-microsoft-edge-as-default-pdf-reader"></a>[ShowPDFDefaultRecommendationsEnabled](microsoft-edge-browser-policies/ShowPDFDefaultRecommendationsEnabled.md)|Allow notifications to set Microsoft Edge as default PDF reader|
|<a id="spotlightexperiencesandrecommendationsenabled"></a><a id="choose-whether-users-can-receive-customized-background-images-and-text-suggestions-notifications-and-tips-for-microsoft-services"></a>[SpotlightExperiencesAndRecommendationsEnabled](microsoft-edge-browser-policies/SpotlightExperiencesAndRecommendationsEnabled.md)|Choose whether users can receive customized background images and text, suggestions, notifications, and tips for Microsoft services|
|<a id="thirdpartystoragepartitioningblockedfororigins"></a><a id="disable-third-party-storage-partitioning-for-specific-top-level-origins"></a>[ThirdPartyStoragePartitioningBlockedForOrigins](microsoft-edge-browser-policies/ThirdPartyStoragePartitioningBlockedForOrigins.md)|Disable third-party storage partitioning for specific top-level origins|
|<a id="webhidallowalldevicesforurls"></a><a id="allow-listed-sites-to-connect-to-any-hid-device"></a>[WebHidAllowAllDevicesForUrls](microsoft-edge-browser-policies/WebHidAllowAllDevicesForUrls.md)|Allow listed sites to connect to any HID device|
|<a id="webhidallowdevicesforurls"></a><a id="allow-listed-sites-connect-to-specific-hid-devices"></a>[WebHidAllowDevicesForUrls](microsoft-edge-browser-policies/WebHidAllowDevicesForUrls.md)|Allow listed sites connect to specific HID devices|
|<a id="webhidallowdeviceswithhidusagesforurls"></a><a id="automatically-grant-permission-to-these-sites-to-connect-to-hid-devices-containing-top-level-collections-with-the-given-hid-usage"></a>[WebHidAllowDevicesWithHidUsagesForUrls](microsoft-edge-browser-policies/WebHidAllowDevicesWithHidUsagesForUrls.md)|Automatically grant permission to these sites to connect to HID devices containing top-level collections with the given HID usage|
|<a id="webhidaskforurls"></a><a id="allow-the-webhid-api-on-these-sites"></a>[WebHidAskForUrls](microsoft-edge-browser-policies/WebHidAskForUrls.md)|Allow the WebHID API on these sites|
|<a id="webhidblockedforurls"></a><a id="block-the-webhid-api-on-these-sites"></a>[WebHidBlockedForUrls](microsoft-edge-browser-policies/WebHidBlockedForUrls.md)|Block the WebHID API on these sites|
|<a id="webusballowdevicesforurls"></a><a id="grant-access-to-specific-sites-to-connect-to-specific-usb-devices"></a>[WebUsbAllowDevicesForUrls](microsoft-edge-browser-policies/WebUsbAllowDevicesForUrls.md)|Grant access to specific sites to connect to specific USB devices|
|<a id="webusbaskforurls"></a><a id="allow-webusb-on-specific-sites"></a>[WebUsbAskForUrls](microsoft-edge-browser-policies/WebUsbAskForUrls.md)|Allow WebUSB on specific sites|
|<a id="webusbblockedforurls"></a><a id="block-webusb-on-specific-sites"></a>[WebUsbBlockedForUrls](microsoft-edge-browser-policies/WebUsbBlockedForUrls.md)|Block WebUSB on specific sites|
|<a id="windowmanagementallowedforurls"></a><a id="allow-window-management-permission-on-specified-sites"></a>[WindowManagementAllowedForUrls](microsoft-edge-browser-policies/WindowManagementAllowedForUrls.md)|Allow Window Management permission on specified sites|
|<a id="windowmanagementblockedforurls"></a><a id="block-window-management-permission-on-specified-sites"></a>[WindowManagementBlockedForUrls](microsoft-edge-browser-policies/WindowManagementBlockedForUrls.md)|Block Window Management permission on specified sites|

<a id="default-search-provider-policies"></a>
### Default search provider

|Policy Name|Caption|
|-|-|
|<a id="defaultsearchproviderenabled"></a><a id="enable-the-default-search-provider"></a>[DefaultSearchProviderEnabled](microsoft-edge-browser-policies/DefaultSearchProviderEnabled.md)|Enable the default search provider|
|<a id="defaultsearchproviderencodings"></a><a id="default-search-provider-encodings"></a>[DefaultSearchProviderEncodings](microsoft-edge-browser-policies/DefaultSearchProviderEncodings.md)|Default search provider encodings|
|<a id="defaultsearchproviderimageurl"></a><a id="specifies-the-search-by-image-feature-for-the-default-search-provider"></a>[DefaultSearchProviderImageURL](microsoft-edge-browser-policies/DefaultSearchProviderImageURL.md)|Specifies the search-by-image feature for the default search provider|
|<a id="defaultsearchproviderimageurlpostparams"></a><a id="parameters-for-an-image-url-that-uses-post"></a>[DefaultSearchProviderImageURLPostParams](microsoft-edge-browser-policies/DefaultSearchProviderImageURLPostParams.md)|Parameters for an image URL that uses POST|
|<a id="defaultsearchproviderkeyword"></a><a id="default-search-provider-keyword"></a>[DefaultSearchProviderKeyword](microsoft-edge-browser-policies/DefaultSearchProviderKeyword.md)|Default search provider keyword|
|<a id="defaultsearchprovidername"></a><a id="default-search-provider-name"></a>[DefaultSearchProviderName](microsoft-edge-browser-policies/DefaultSearchProviderName.md)|Default search provider name|
|<a id="defaultsearchprovidersearchurl"></a><a id="default-search-provider-search-url"></a>[DefaultSearchProviderSearchURL](microsoft-edge-browser-policies/DefaultSearchProviderSearchURL.md)|Default search provider search URL|
|<a id="defaultsearchprovidersuggesturl"></a><a id="default-search-provider-url-for-suggestions"></a>[DefaultSearchProviderSuggestURL](microsoft-edge-browser-policies/DefaultSearchProviderSuggestURL.md)|Default search provider URL for suggestions|
|<a id="newtabpagesearchbox"></a><a id="configure-the-new-tab-page-search-box-experience"></a>[NewTabPageSearchBox](microsoft-edge-browser-policies/NewTabPageSearchBox.md)|Configure the new tab page search box experience|

<a id="downloads-policies"></a>
### Downloads

|Policy Name|Caption|
|-|-|
|<a id="showdownloadsinsecurewarningsenabled"></a><a id="enable-insecure-download-warnings"></a>[ShowDownloadsInsecureWarningsEnabled](microsoft-edge-browser-policies/ShowDownloadsInsecureWarningsEnabled.md)|Enable insecure download warnings|

<a id="edge-website-typo-protection-settings-policies"></a>
### Edge Website Typo Protection settings

|Policy Name|Caption|
|-|-|
|<a id="preventtyposquattingpromptoverride"></a><a id="prevent-bypassing-edge-website-typo-protection-prompts-for-sites"></a>[PreventTyposquattingPromptOverride](microsoft-edge-browser-policies/PreventTyposquattingPromptOverride.md)|Prevent bypassing Edge Website Typo Protection prompts for sites|
|<a id="typosquattingallowlistdomains"></a><a id="configure-the-list-of-domains-for-which-edge-website-typo-protection-wont-trigger-warnings"></a>[TyposquattingAllowListDomains](microsoft-edge-browser-policies/TyposquattingAllowListDomains.md)|Configure the list of domains for which Edge Website Typo Protection won't trigger warnings|
|<a id="typosquattingcheckerenabled"></a><a id="configure-edge-website-typo-protection"></a>[TyposquattingCheckerEnabled](microsoft-edge-browser-policies/TyposquattingCheckerEnabled.md)|Configure Edge Website Typo Protection|

<a id="edge-workspaces-settings-policies"></a>
### Edge Workspaces settings

|Policy Name|Caption|
|-|-|
|<a id="edgeworkspacesenabled"></a><a id="enable-workspaces"></a>[EdgeWorkspacesEnabled](microsoft-edge-browser-policies/EdgeWorkspacesEnabled.md)|Enable Workspaces|
|<a id="workspacesnavigationsettings"></a><a id="configure-navigation-settings-per-groups-of-urls-in-microsoft-edge-workspaces"></a>[WorkspacesNavigationSettings](microsoft-edge-browser-policies/WorkspacesNavigationSettings.md)|Configure navigation settings per groups of URLs in Microsoft Edge Workspaces|

<a id="experimentation-policies"></a>
### Experimentation

|Policy Name|Caption|
|-|-|
|<a id="featureflagoverridescontrol"></a><a id="configure-users-ability-to-override-feature-flags"></a>[FeatureFlagOverridesControl](microsoft-edge-browser-policies/FeatureFlagOverridesControl.md)|Configure users ability to override feature flags|

<a id="extensions-policies"></a>
### Extensions

|Policy Name|Caption|
|-|-|
|<a id="blockexternalextensions"></a><a id="blocks-external-extensions-from-being-installed"></a>[BlockExternalExtensions](microsoft-edge-browser-policies/BlockExternalExtensions.md)|Blocks external extensions from being installed|
|<a id="controldefaultstateofallowextensionfromotherstoressettingenabled"></a><a id="configure-default-state-of-allow-extensions-from-other-stores-setting"></a>[ControlDefaultStateOfAllowExtensionFromOtherStoresSettingEnabled](microsoft-edge-browser-policies/ControlDefaultStateOfAllowExtensionFromOtherStoresSettingEnabled.md)|Configure default state of Allow extensions from other stores setting|
|<a id="extensionallowedtypes"></a><a id="configure-allowed-extension-types"></a>[ExtensionAllowedTypes](microsoft-edge-browser-policies/ExtensionAllowedTypes.md)|Configure allowed extension types|
|<a id="extensiondevelopermodesettings"></a><a id="control-the-availability-of-developer-mode-on-extensions-page"></a>[ExtensionDeveloperModeSettings](microsoft-edge-browser-policies/ExtensionDeveloperModeSettings.md)|Control the availability of developer mode on extensions page|
|<a id="extensionextendedbackgroundlifetimeforportconnectionstourls"></a><a id="configure-a-list-of-origins-that-grant-an-extended-background-lifetime-to-connecting-extensions"></a>[ExtensionExtendedBackgroundLifetimeForPortConnectionsToUrls](microsoft-edge-browser-policies/ExtensionExtendedBackgroundLifetimeForPortConnectionsToUrls.md)|Configure a list of origins that grant an extended background lifetime to connecting extensions.|
|<a id="extensioninstallallowlist"></a><a id="allow-specific-extensions-to-be-installed"></a>[ExtensionInstallAllowlist](microsoft-edge-browser-policies/ExtensionInstallAllowlist.md)|Allow specific extensions to be installed|
|<a id="extensioninstallblocklist"></a><a id="control-which-extensions-cannot-be-installed"></a>[ExtensionInstallBlocklist](microsoft-edge-browser-policies/ExtensionInstallBlocklist.md)|Control which extensions cannot be installed|
|<a id="extensioninstallforcelist"></a><a id="control-which-extensions-are-installed-silently"></a>[ExtensionInstallForcelist](microsoft-edge-browser-policies/ExtensionInstallForcelist.md)|Control which extensions are installed silently|
|<a id="extensioninstallsources"></a><a id="configure-extension-and-user-script-install-sources"></a>[ExtensionInstallSources](microsoft-edge-browser-policies/ExtensionInstallSources.md)|Configure extension and user script install sources|
|<a id="extensioninstalltypeblocklist"></a><a id="blocklist-for-extension-install-types"></a>[ExtensionInstallTypeBlocklist](microsoft-edge-browser-policies/ExtensionInstallTypeBlocklist.md)|Blocklist for extension install types|
|<a id="extensionmanifestv2availability"></a><a id="control-manifest-v2-extension-availability"></a>[ExtensionManifestV2Availability](microsoft-edge-browser-policies/ExtensionManifestV2Availability.md)|Control Manifest v2 extension availability|
|<a id="extensionsettings"></a><a id="configure-extension-management-settings"></a>[ExtensionSettings](microsoft-edge-browser-policies/ExtensionSettings.md)|Configure extension management settings|

<a id="games-settings-policies"></a>
### Games settings

|Policy Name|Caption|
|-|-|
|<a id="gamermodeenabled"></a><a id="enable-gamer-mode"></a>[GamerModeEnabled](microsoft-edge-browser-policies/GamerModeEnabled.md)|Enable Gamer Mode|

<a id="generative-ai-policies"></a>
### Generative AI

|Policy Name|Caption|
|-|-|
|<a id="genailocalfoundationalmodelsettings"></a><a id="settings-for-genai-local-foundational-model"></a>[GenAILocalFoundationalModelSettings](microsoft-edge-browser-policies/GenAILocalFoundationalModelSettings.md)|Settings for GenAI local foundational model|

<a id="http-authentication-policies"></a>
### HTTP authentication

|Policy Name|Caption|
|-|-|
|<a id="allhttpauthschemesallowedfororigins"></a><a id="list-of-origins-that-allow-all-http-authentication"></a>[AllHttpAuthSchemesAllowedForOrigins](microsoft-edge-browser-policies/AllHttpAuthSchemesAllowedForOrigins.md)|List of origins that allow all HTTP authentication|
|<a id="allowcrossoriginauthprompt"></a><a id="allow-cross-origin-http-authentication-prompts"></a>[AllowCrossOriginAuthPrompt](microsoft-edge-browser-policies/AllowCrossOriginAuthPrompt.md)|Allow cross-origin HTTP Authentication prompts|
|<a id="authnegotiatedelegateallowlist"></a><a id="specifies-a-list-of-servers-that-microsoft-edge-can-delegate-user-credentials-to"></a>[AuthNegotiateDelegateAllowlist](microsoft-edge-browser-policies/AuthNegotiateDelegateAllowlist.md)|Specifies a list of servers that Microsoft Edge can delegate user credentials to|
|<a id="authschemes"></a><a id="supported-authentication-schemes"></a>[AuthSchemes](microsoft-edge-browser-policies/AuthSchemes.md)|Supported authentication schemes|
|<a id="authserverallowlist"></a><a id="configure-list-of-allowed-authentication-servers"></a>[AuthServerAllowlist](microsoft-edge-browser-policies/AuthServerAllowlist.md)|Configure list of allowed authentication servers|
|<a id="basicauthoverhttpenabled"></a><a id="allow-basic-authentication-for-http"></a>[BasicAuthOverHttpEnabled](microsoft-edge-browser-policies/BasicAuthOverHttpEnabled.md)|Allow Basic authentication for HTTP|
|<a id="disableauthnegotiatecnamelookup"></a><a id="disable-cname-lookup-when-negotiating-kerberos-authentication"></a>[DisableAuthNegotiateCnameLookup](microsoft-edge-browser-policies/DisableAuthNegotiateCnameLookup.md)|Disable CNAME lookup when negotiating Kerberos authentication|
|<a id="enableauthnegotiateport"></a><a id="include-non-standard-port-in-kerberos-spn"></a>[EnableAuthNegotiatePort](microsoft-edge-browser-policies/EnableAuthNegotiatePort.md)|Include non-standard port in Kerberos SPN|
|<a id="ntlmv2enabled"></a><a id="control-whether-ntlmv2-authentication-is-enabled"></a>[NtlmV2Enabled](microsoft-edge-browser-policies/NtlmV2Enabled.md)|Control whether NTLMv2 authentication is enabled|
|<a id="windowshelloforhttpauthenabled"></a><a id="windows-hello-for-http-auth-enabled"></a>[WindowsHelloForHTTPAuthEnabled](microsoft-edge-browser-policies/WindowsHelloForHTTPAuthEnabled.md)|Windows Hello For HTTP Auth Enabled|

<a id="identity-and-sign-in-policies"></a>
### Identity and sign-in

|Policy Name|Caption|
|-|-|
|<a id="automaticprofileswitchingsitelist"></a><a id="configure-the-automatic-profile-switching-site-list"></a>[AutomaticProfileSwitchingSiteList](microsoft-edge-browser-policies/AutomaticProfileSwitchingSiteList.md)|Configure the automatic profile switching site list|
|<a id="edgedefaultprofileenabled"></a><a id="default-profile-setting-enabled"></a>[EdgeDefaultProfileEnabled](microsoft-edge-browser-policies/EdgeDefaultProfileEnabled.md)|Default Profile Setting Enabled|
|<a id="guidedswitchenabled"></a><a id="guided-switch-enabled"></a>[GuidedSwitchEnabled](microsoft-edge-browser-policies/GuidedSwitchEnabled.md)|Guided Switch Enabled|
|<a id="implicitsigninenabled"></a><a id="enable-implicit-sign-in"></a>[ImplicitSignInEnabled](microsoft-edge-browser-policies/ImplicitSignInEnabled.md)|Enable implicit sign-in|
|<a id="linkedaccountenabled"></a><a id="enable-the-linked-account-feature-obsolete"></a>[LinkedAccountEnabled](microsoft-edge-browser-policies/LinkedAccountEnabled.md)|Enable the linked account feature (obsolete)|
|<a id="oneauthauthenticationenforced"></a><a id="oneauth-authentication-flow-enforced-for-signin"></a>[OneAuthAuthenticationEnforced](microsoft-edge-browser-policies/OneAuthAuthenticationEnforced.md)|OneAuth Authentication Flow Enforced for signin|
|<a id="onlyonpremisesimplicitsigninenabled"></a><a id="only-on-premises-account-enabled-for-implicit-sign-in"></a>[OnlyOnPremisesImplicitSigninEnabled](microsoft-edge-browser-policies/OnlyOnPremisesImplicitSigninEnabled.md)|Only on-premises account enabled for implicit sign-in|
|<a id="proactiveauthworkflowenabled"></a><a id="enable-proactive-authentication"></a>[ProactiveAuthWorkflowEnabled](microsoft-edge-browser-policies/ProactiveAuthWorkflowEnabled.md)|Enable proactive authentication|
|<a id="seamlesswebtobrowsersigninenabled"></a><a id="seamless-web-to-browser-sign-in-enabled"></a>[SeamlessWebToBrowserSignInEnabled](microsoft-edge-browser-policies/SeamlessWebToBrowserSignInEnabled.md)|Seamless Web To Browser Sign-in Enabled|
|<a id="signinctaonntpenabled"></a><a id="enable-sign-in-click-to-action-dialog-obsolete"></a>[SignInCtaOnNtpEnabled](microsoft-edge-browser-policies/SignInCtaOnNtpEnabled.md)|Enable sign in click to action dialog (obsolete)|
|<a id="switchintranetsitestoworkprofile"></a><a id="switch-intranet-sites-to-a-work-or-school-profile"></a>[SwitchIntranetSitesToWorkProfile](microsoft-edge-browser-policies/SwitchIntranetSitesToWorkProfile.md)|Switch intranet sites to a work or school profile|
|<a id="switchsitesoniemodesitelisttoworkprofile"></a><a id="switch-sites-on-the-ie-mode-site-list-to-a-work-or-school-profile"></a>[SwitchSitesOnIEModeSiteListToWorkProfile](microsoft-edge-browser-policies/SwitchSitesOnIEModeSiteListToWorkProfile.md)|Switch sites on the IE mode site list to a work or school profile|
|<a id="wamauthbelowwin10rs3enabled"></a><a id="wam-for-authentication-below-windows-10-rs3-enabled"></a>[WAMAuthBelowWin10RS3Enabled](microsoft-edge-browser-policies/WAMAuthBelowWin10RS3Enabled.md)|WAM for authentication below Windows 10 RS3 enabled|
|<a id="webtobrowsersigninenabled"></a><a id="web-to-browser-sign-in-enabled"></a>[WebToBrowserSignInEnabled](microsoft-edge-browser-policies/WebToBrowserSignInEnabled.md)|Web To Browser Sign-in Enabled|

<a id="idle-browser-actions-policies"></a>
### Idle Browser Actions

|Policy Name|Caption|
|-|-|
|<a id="idletimeout"></a><a id="delay-before-running-idle-actions"></a>[IdleTimeout](microsoft-edge-browser-policies/IdleTimeout.md)|Delay before running idle actions|
|<a id="idletimeoutactions"></a><a id="actions-to-run-when-the-computer-is-idle"></a>[IdleTimeoutActions](microsoft-edge-browser-policies/IdleTimeoutActions.md)|Actions to run when the computer is idle|

<a id="immersive-reader-settings-policies"></a>
### Immersive Reader settings

|Policy Name|Caption|
|-|-|
|<a id="immersivereadergrammartoolsenabled"></a><a id="enable-grammar-tools-feature-within-immersive-reader-in-microsoft-edge-obsolete"></a>[ImmersiveReaderGrammarToolsEnabled](microsoft-edge-browser-policies/ImmersiveReaderGrammarToolsEnabled.md)|Enable Grammar Tools feature within Immersive Reader in Microsoft Edge (obsolete)|
|<a id="immersivereaderpicturedictionaryenabled"></a><a id="enable-picture-dictionary-feature-within-immersive-reader-in-microsoft-edge-obsolete"></a>[ImmersiveReaderPictureDictionaryEnabled](microsoft-edge-browser-policies/ImmersiveReaderPictureDictionaryEnabled.md)|Enable Picture Dictionary feature within Immersive Reader in Microsoft Edge (obsolete)|

<a id="kiosk-mode-settings-policies"></a>
### Kiosk Mode settings

|Policy Name|Caption|
|-|-|
|<a id="kioskaddressbareditingenabled"></a><a id="configure-address-bar-editing-for-kiosk-mode-public-browsing-experience"></a>[KioskAddressBarEditingEnabled](microsoft-edge-browser-policies/KioskAddressBarEditingEnabled.md)|Configure address bar editing for kiosk mode public browsing experience|
|<a id="kioskdeletedownloadsonexit"></a><a id="delete-files-downloaded-as-part-of-kiosk-session-when-microsoft-edge-closes"></a>[KioskDeleteDownloadsOnExit](microsoft-edge-browser-policies/KioskDeleteDownloadsOnExit.md)|Delete files downloaded as part of kiosk session when Microsoft Edge closes|
|<a id="kioskswipegesturesenabled"></a><a id="swipe-gestures-in-microsoft-edge-kiosk-mode-enabled"></a>[KioskSwipeGesturesEnabled](microsoft-edge-browser-policies/KioskSwipeGesturesEnabled.md)|Swipe gestures in Microsoft Edge kiosk mode enabled|

<a id="manageability-policies"></a>
### Manageability

|Policy Name|Caption|
|-|-|
|<a id="edgemanagementenabled"></a><a id="microsoft-edge-management-enabled"></a>[EdgeManagementEnabled](microsoft-edge-browser-policies/EdgeManagementEnabled.md)|Microsoft Edge management enabled|
|<a id="edgemanagementenrollmenttoken"></a><a id="microsoft-edge-management-enrollment-token"></a>[EdgeManagementEnrollmentToken](microsoft-edge-browser-policies/EdgeManagementEnrollmentToken.md)|Microsoft Edge management enrollment token|
|<a id="edgemanagementextensionsfeedbackenabled"></a><a id="microsoft-edge-management-extensions-feedback-enabled"></a>[EdgeManagementExtensionsFeedbackEnabled](microsoft-edge-browser-policies/EdgeManagementExtensionsFeedbackEnabled.md)|Microsoft Edge management extensions feedback enabled|
|<a id="edgemanagementpolicyoverridesplatformpolicy"></a><a id="microsoft-edge-management-service-policy-overrides-platform-policy"></a>[EdgeManagementPolicyOverridesPlatformPolicy](microsoft-edge-browser-policies/EdgeManagementPolicyOverridesPlatformPolicy.md)|Microsoft Edge management service policy overrides platform policy.|
|<a id="edgemanagementuserpolicyoverridescloudmachinepolicy"></a><a id="allow-cloud-based-microsoft-edge-management-service-user-policies-to-override-local-user-policies"></a>[EdgeManagementUserPolicyOverridesCloudMachinePolicy](microsoft-edge-browser-policies/EdgeManagementUserPolicyOverridesCloudMachinePolicy.md)|Allow cloud-based Microsoft Edge management service user policies to override local user policies.|
|<a id="mamenabled"></a><a id="mobile-app-management-enabled"></a>[MAMEnabled](microsoft-edge-browser-policies/MAMEnabled.md)|Mobile App Management Enabled|

<a id="native-messaging-policies"></a>
### Native Messaging

|Policy Name|Caption|
|-|-|
|<a id="nativemessagingallowlist"></a><a id="control-which-native-messaging-hosts-users-can-use"></a>[NativeMessagingAllowlist](microsoft-edge-browser-policies/NativeMessagingAllowlist.md)|Control which native messaging hosts users can use|
|<a id="nativemessagingblocklist"></a><a id="configure-native-messaging-block-list"></a>[NativeMessagingBlocklist](microsoft-edge-browser-policies/NativeMessagingBlocklist.md)|Configure native messaging block list|
|<a id="nativemessaginguserlevelhosts"></a><a id="allow-user-level-native-messaging-hosts-installed-without-admin-permissions"></a>[NativeMessagingUserLevelHosts](microsoft-edge-browser-policies/NativeMessagingUserLevelHosts.md)|Allow user-level native messaging hosts (installed without admin permissions)|

<a id="network-settings-policies"></a>
### Network settings

|Policy Name|Caption|
|-|-|
|<a id="accesscontrolallowmethodsincorspreflightspecconformant"></a><a id="make-access-control-allow-methods-matching-in-cors-preflight-spec-conformant"></a>[AccessControlAllowMethodsInCORSPreflightSpecConformant](microsoft-edge-browser-policies/AccessControlAllowMethodsInCORSPreflightSpecConformant.md)|Make Access-Control-Allow-Methods matching in CORS preflight spec conformant|
|<a id="blocktruncatedcookies"></a><a id="block-truncated-cookies-obsolete"></a>[BlockTruncatedCookies](microsoft-edge-browser-policies/BlockTruncatedCookies.md)|Block truncated cookies (obsolete)|
|<a id="compressiondictionarytransportenabled"></a><a id="enable-compression-dictionary-transport-support"></a>[CompressionDictionaryTransportEnabled](microsoft-edge-browser-policies/CompressionDictionaryTransportEnabled.md)|Enable compression dictionary transport support|
|<a id="dataurlwhitespacepreservationenabled"></a><a id="dataurl-whitespace-preservation-for-all-media-types"></a>[DataURLWhitespacePreservationEnabled](microsoft-edge-browser-policies/DataURLWhitespacePreservationEnabled.md)|DataURL Whitespace Preservation for all media types|
|<a id="ipv6reachabilityoverrideenabled"></a><a id="enable-ipv6-reachability-check-override"></a>[IPv6ReachabilityOverrideEnabled](microsoft-edge-browser-policies/IPv6ReachabilityOverrideEnabled.md)|Enable IPv6 reachability check override|
|<a id="zstdcontentencodingenabled"></a><a id="enable-zstd-content-encoding-support"></a>[ZstdContentEncodingEnabled](microsoft-edge-browser-policies/ZstdContentEncodingEnabled.md)|Enable zstd content encoding support|

<a id="pdf-reader-policies"></a>
### PDF Reader

|Policy Name|Caption|
|-|-|
|<a id="viewxfapdfiniemodeallowedfilehash"></a><a id="view-xfa-based-pdf-files-using-ie-mode-for-allowed-file-hash"></a>[ViewXFAPDFInIEModeAllowedFileHash](microsoft-edge-browser-policies/ViewXFAPDFInIEModeAllowedFileHash.md)|View XFA-based PDF files using IE Mode for allowed file hash.|
|<a id="viewxfapdfiniemodeallowedorigins"></a><a id="view-xfa-based-pdf-files-using-ie-mode-for-allowed-file-origin"></a>[ViewXFAPDFInIEModeAllowedOrigins](microsoft-edge-browser-policies/ViewXFAPDFInIEModeAllowedOrigins.md)|View XFA-based PDF files using IE Mode for allowed file origin.|

<a id="password-manager-and-protection-policies"></a>
### Password manager and protection

|Policy Name|Caption|
|-|-|
|<a id="deletingundecryptablepasswordsenabled"></a><a id="enable-deleting-undecryptable-passwords"></a>[DeletingUndecryptablePasswordsEnabled](microsoft-edge-browser-policies/DeletingUndecryptablePasswordsEnabled.md)|Enable deleting undecryptable passwords|
|<a id="passworddeleteonbrowsercloseenabled"></a><a id="prevent-passwords-from-being-deleted-if-any-edge-settings-is-enabled-to-delete-browsing-data-when-microsoft-edge-closes"></a>[PasswordDeleteOnBrowserCloseEnabled](microsoft-edge-browser-policies/PasswordDeleteOnBrowserCloseEnabled.md)|Prevent passwords from being deleted if any Edge settings is enabled to delete browsing data when Microsoft Edge closes|
|<a id="passwordexportenabled"></a><a id="enable-exporting-saved-passwords-from-password-manager"></a>[PasswordExportEnabled](microsoft-edge-browser-policies/PasswordExportEnabled.md)|Enable exporting saved passwords from Password Manager|
|<a id="passwordgeneratorenabled"></a><a id="allow-users-to-get-a-strong-password-suggestion-whenever-they-are-creating-an-account-online"></a>[PasswordGeneratorEnabled](microsoft-edge-browser-policies/PasswordGeneratorEnabled.md)|Allow users to get a strong password suggestion whenever they are creating an account online|
|<a id="passwordmanagerblocklist"></a><a id="configure-the-list-of-domains-for-which-the-password-manager-ui-save-and-fill-will-be-disabled"></a>[PasswordManagerBlocklist](microsoft-edge-browser-policies/PasswordManagerBlocklist.md)|Configure the list of domains for which the password manager UI (Save and Fill) will be disabled|
|<a id="passwordmanagerenabled"></a><a id="enable-saving-passwords-to-the-password-manager"></a>[PasswordManagerEnabled](microsoft-edge-browser-policies/PasswordManagerEnabled.md)|Enable saving passwords to the password manager|
|<a id="passwordmanagerrestrictlengthenabled"></a><a id="restrict-the-length-of-passwords-that-can-be-saved-in-the-password-manager"></a>[PasswordManagerRestrictLengthEnabled](microsoft-edge-browser-policies/PasswordManagerRestrictLengthEnabled.md)|Restrict the length of passwords that can be saved in the Password Manager|
|<a id="passwordmonitorallowed"></a><a id="allow-users-to-be-alerted-if-their-passwords-are-found-to-be-unsafe"></a>[PasswordMonitorAllowed](microsoft-edge-browser-policies/PasswordMonitorAllowed.md)|Allow users to be alerted if their passwords are found to be unsafe|
|<a id="passwordprotectionchangepasswordurl"></a><a id="configure-the-change-password-url"></a>[PasswordProtectionChangePasswordURL](microsoft-edge-browser-policies/PasswordProtectionChangePasswordURL.md)|Configure the change password URL|
|<a id="passwordprotectionloginurls"></a><a id="configure-the-list-of-enterprise-login-urls-where-the-password-protection-service-should-capture-salted-hashes-of-a-password"></a>[PasswordProtectionLoginURLs](microsoft-edge-browser-policies/PasswordProtectionLoginURLs.md)|Configure the list of enterprise login URLs where the password protection service should capture salted hashes of a password|
|<a id="passwordprotectionwarningtrigger"></a><a id="configure-password-protection-warning-trigger"></a>[PasswordProtectionWarningTrigger](microsoft-edge-browser-policies/PasswordProtectionWarningTrigger.md)|Configure password protection warning trigger|
|<a id="passwordrevealenabled"></a><a id="enable-password-reveal-button"></a>[PasswordRevealEnabled](microsoft-edge-browser-policies/PasswordRevealEnabled.md)|Enable Password reveal button|
|<a id="primarypasswordsetting"></a><a id="configures-a-setting-that-asks-users-to-enter-their-device-password-while-using-password-autofill"></a>[PrimaryPasswordSetting](microsoft-edge-browser-policies/PrimaryPasswordSetting.md)|Configures a setting that asks users to enter their device password while using password autofill|

<a id="performance-policies"></a>
### Performance

|Policy Name|Caption|
|-|-|
|<a id="efficiencymode"></a><a id="configure-when-efficiency-mode-should-become-active"></a>[EfficiencyMode](microsoft-edge-browser-policies/EfficiencyMode.md)|Configure when efficiency mode should become active|
|<a id="efficiencymodeenabled"></a><a id="efficiency-mode-enabled"></a>[EfficiencyModeEnabled](microsoft-edge-browser-policies/EfficiencyModeEnabled.md)|Efficiency mode enabled|
|<a id="efficiencymodeonpowerenabled"></a><a id="enable-efficiency-mode-when-the-device-is-connected-to-a-power-source"></a>[EfficiencyModeOnPowerEnabled](microsoft-edge-browser-policies/EfficiencyModeOnPowerEnabled.md)|Enable efficiency mode when the device is connected to a power source|
|<a id="extensionsperformancedetectorenabled"></a><a id="extensions-performance-detector-enabled"></a>[ExtensionsPerformanceDetectorEnabled](microsoft-edge-browser-policies/ExtensionsPerformanceDetectorEnabled.md)|Extensions Performance Detector enabled|
|<a id="performancedetectorenabled"></a><a id="performance-detector-enabled"></a>[PerformanceDetectorEnabled](microsoft-edge-browser-policies/PerformanceDetectorEnabled.md)|Performance Detector Enabled|
|<a id="pinbrowseressentialstoolbarbutton"></a><a id="pin-browser-essentials-toolbar-button"></a>[PinBrowserEssentialsToolbarButton](microsoft-edge-browser-policies/PinBrowserEssentialsToolbarButton.md)|Pin browser essentials toolbar button|
|<a id="startupboostenabled"></a><a id="enable-startup-boost"></a>[StartupBoostEnabled](microsoft-edge-browser-policies/StartupBoostEnabled.md)|Enable startup boost|

<a id="permit-or-deny-screen-capture-policies"></a>
### Permit or deny screen capture

|Policy Name|Caption|
|-|-|
|<a id="sameorigintabcaptureallowedbyorigins"></a><a id="allow-same-origin-tab-capture-by-these-origins"></a>[SameOriginTabCaptureAllowedByOrigins](microsoft-edge-browser-policies/SameOriginTabCaptureAllowedByOrigins.md)|Allow Same Origin Tab capture by these origins|
|<a id="screencaptureallowedbyorigins"></a><a id="allow-desktop-window-and-tab-capture-by-these-origins"></a>[ScreenCaptureAllowedByOrigins](microsoft-edge-browser-policies/ScreenCaptureAllowedByOrigins.md)|Allow Desktop, Window, and Tab capture by these origins|
|<a id="tabcaptureallowedbyorigins"></a><a id="allow-tab-capture-by-these-origins"></a>[TabCaptureAllowedByOrigins](microsoft-edge-browser-policies/TabCaptureAllowedByOrigins.md)|Allow Tab capture by these origins|
|<a id="windowcaptureallowedbyorigins"></a><a id="allow-window-and-tab-capture-by-these-origins"></a>[WindowCaptureAllowedByOrigins](microsoft-edge-browser-policies/WindowCaptureAllowedByOrigins.md)|Allow Window and Tab capture by these origins|

<a id="printing-policies"></a>
### Printing

|Policy Name|Caption|
|-|-|
|<a id="defaultprinterselection"></a><a id="default-printer-selection-rules"></a>[DefaultPrinterSelection](microsoft-edge-browser-policies/DefaultPrinterSelection.md)|Default printer selection rules|
|<a id="oopprintdriversallowed"></a><a id="out-of-process-print-drivers-allowed"></a>[OopPrintDriversAllowed](microsoft-edge-browser-policies/OopPrintDriversAllowed.md)|Out-of-process print drivers allowed|
|<a id="printheaderfooter"></a><a id="print-headers-and-footers"></a>[PrintHeaderFooter](microsoft-edge-browser-policies/PrintHeaderFooter.md)|Print headers and footers|
|<a id="printpdfasimagedefault"></a><a id="print-pdf-as-image-default"></a>[PrintPdfAsImageDefault](microsoft-edge-browser-policies/PrintPdfAsImageDefault.md)|Print PDF as Image Default|
|<a id="printpostscriptmode"></a><a id="print-postscript-mode"></a>[PrintPostScriptMode](microsoft-edge-browser-policies/PrintPostScriptMode.md)|Print PostScript Mode|
|<a id="printpreviewstickysettings"></a><a id="configure-the-sticky-print-preview-settings"></a>[PrintPreviewStickySettings](microsoft-edge-browser-policies/PrintPreviewStickySettings.md)|Configure the sticky print preview settings|
|<a id="printpreviewusesystemdefaultprinter"></a><a id="set-the-system-default-printer-as-the-default-printer"></a>[PrintPreviewUseSystemDefaultPrinter](microsoft-edge-browser-policies/PrintPreviewUseSystemDefaultPrinter.md)|Set the system default printer as the default printer|
|<a id="printrasterizationmode"></a><a id="print-rasterization-mode"></a>[PrintRasterizationMode](microsoft-edge-browser-policies/PrintRasterizationMode.md)|Print Rasterization Mode|
|<a id="printrasterizepdfdpi"></a><a id="print-rasterize-pdf-dpi"></a>[PrintRasterizePdfDpi](microsoft-edge-browser-policies/PrintRasterizePdfDpi.md)|Print Rasterize PDF DPI|
|<a id="printstickysettings"></a><a id="print-preview-sticky-settings"></a>[PrintStickySettings](microsoft-edge-browser-policies/PrintStickySettings.md)|Print preview sticky settings|
|<a id="printertypedenylist"></a><a id="disable-printer-types-on-the-deny-list"></a>[PrinterTypeDenyList](microsoft-edge-browser-policies/PrinterTypeDenyList.md)|Disable printer types on the deny list|
|<a id="printingallowedbackgroundgraphicsmodes"></a><a id="restrict-background-graphics-printing-mode"></a>[PrintingAllowedBackgroundGraphicsModes](microsoft-edge-browser-policies/PrintingAllowedBackgroundGraphicsModes.md)|Restrict background graphics printing mode|
|<a id="printingbackgroundgraphicsdefault"></a><a id="default-background-graphics-printing-mode"></a>[PrintingBackgroundGraphicsDefault](microsoft-edge-browser-policies/PrintingBackgroundGraphicsDefault.md)|Default background graphics printing mode|
|<a id="printingenabled"></a><a id="enable-printing"></a>[PrintingEnabled](microsoft-edge-browser-policies/PrintingEnabled.md)|Enable printing|
|<a id="printinglpacsandboxenabled"></a><a id="enable-printing-lpac-sandbox"></a>[PrintingLPACSandboxEnabled](microsoft-edge-browser-policies/PrintingLPACSandboxEnabled.md)|Enable Printing LPAC Sandbox|
|<a id="printingpapersizedefault"></a><a id="default-printing-page-size"></a>[PrintingPaperSizeDefault](microsoft-edge-browser-policies/PrintingPaperSizeDefault.md)|Default printing page size|
|<a id="printingwebpagelayout"></a><a id="sets-layout-for-printing"></a>[PrintingWebpageLayout](microsoft-edge-browser-policies/PrintingWebpageLayout.md)|Sets layout for printing|
|<a id="usesystemprintdialog"></a><a id="print-using-system-print-dialog"></a>[UseSystemPrintDialog](microsoft-edge-browser-policies/UseSystemPrintDialog.md)|Print using system print dialog|

<a id="private-network-request-settings-policies"></a>
### Private Network Request Settings

|Policy Name|Caption|
|-|-|
|<a id="insecureprivatenetworkrequestsallowed"></a><a id="specifies-whether-to-allow-websites-to-make-requests-to-any-network-endpoint-in-an-insecure-manner"></a>[InsecurePrivateNetworkRequestsAllowed](microsoft-edge-browser-policies/InsecurePrivateNetworkRequestsAllowed.md)|Specifies whether to allow websites to make requests to any network endpoint in an insecure manner.|
|<a id="insecureprivatenetworkrequestsallowedforurls"></a><a id="allow-the-listed-sites-to-make-requests-to-more-private-network-endpoints-from-in-an-insecure-manner"></a>[InsecurePrivateNetworkRequestsAllowedForUrls](microsoft-edge-browser-policies/InsecurePrivateNetworkRequestsAllowedForUrls.md)|Allow the listed sites to make requests to more-private network endpoints from in an insecure manner|
|<a id="privatenetworkaccessrestrictionsenabled"></a><a id="specifies-whether-to-apply-restrictions-to-requests-to-more-private-network-endpoints"></a>[PrivateNetworkAccessRestrictionsEnabled](microsoft-edge-browser-policies/PrivateNetworkAccessRestrictionsEnabled.md)|Specifies whether to apply restrictions to requests to more private network endpoints|

<a id="profile-settings-policies"></a>
### Profile settings

|Policy Name|Caption|
|-|-|
|<a id="profiletypeinprofilebuttonenabled"></a><a id="controls-the-display-of-the-profile-button-label-for-the-work-or-school-profile"></a>[ProfileTypeInProfileButtonEnabled](microsoft-edge-browser-policies/ProfileTypeInProfileButtonEnabled.md)|Controls the display of the profile button label for the work or school profile|

<a id="proxy-server-policies"></a>
### Proxy server

|Policy Name|Caption|
|-|-|
|<a id="proxybypasslist"></a><a id="configure-proxy-bypass-rules-deprecated"></a>[ProxyBypassList](microsoft-edge-browser-policies/ProxyBypassList.md)|Configure proxy bypass rules (deprecated)|
|<a id="proxymode"></a><a id="configure-proxy-server-settings-deprecated"></a>[ProxyMode](microsoft-edge-browser-policies/ProxyMode.md)|Configure proxy server settings (deprecated)|
|<a id="proxypacurl"></a><a id="set-the-proxy-pac-file-url-deprecated"></a>[ProxyPacUrl](microsoft-edge-browser-policies/ProxyPacUrl.md)|Set the proxy .pac file URL (deprecated)|
|<a id="proxyserver"></a><a id="configure-address-or-url-of-proxy-server-deprecated"></a>[ProxyServer](microsoft-edge-browser-policies/ProxyServer.md)|Configure address or URL of proxy server (deprecated)|
|<a id="proxysettings"></a><a id="proxy-settings"></a>[ProxySettings](microsoft-edge-browser-policies/ProxySettings.md)|Proxy settings|

<a id="related-website-sets-settings-policies"></a>
### Related Website Sets Settings

|Policy Name|Caption|
|-|-|
|<a id="relatedwebsitesetsenabled"></a><a id="enable-related-website-sets"></a>[RelatedWebsiteSetsEnabled](microsoft-edge-browser-policies/RelatedWebsiteSetsEnabled.md)|Enable Related Website Sets|
|<a id="relatedwebsitesetsoverrides"></a><a id="override-related-website-sets"></a>[RelatedWebsiteSetsOverrides](microsoft-edge-browser-policies/RelatedWebsiteSetsOverrides.md)|Override Related Website Sets.|

<a id="scareware-blocker-settings-policies"></a>
### Scareware Blocker settings

|Policy Name|Caption|
|-|-|
|<a id="scarewareblockerprotectionenabled"></a><a id="configure-edge-scareware-blocker-protection"></a>[ScarewareBlockerProtectionEnabled](microsoft-edge-browser-policies/ScarewareBlockerProtectionEnabled.md)|Configure Edge Scareware Blocker Protection|

<a id="sleeping-tabs-settings-policies"></a>
### Sleeping tabs settings

|Policy Name|Caption|
|-|-|
|<a id="autodiscardsleepingtabsenabled"></a><a id="configure-auto-discard-sleeping-tabs"></a>[AutoDiscardSleepingTabsEnabled](microsoft-edge-browser-policies/AutoDiscardSleepingTabsEnabled.md)|Configure auto discard sleeping tabs|
|<a id="sleepingtabsblockedforurls"></a><a id="block-sleeping-tabs-on-specific-sites"></a>[SleepingTabsBlockedForUrls](microsoft-edge-browser-policies/SleepingTabsBlockedForUrls.md)|Block sleeping tabs on specific sites|
|<a id="sleepingtabsenabled"></a><a id="configure-sleeping-tabs"></a>[SleepingTabsEnabled](microsoft-edge-browser-policies/SleepingTabsEnabled.md)|Configure sleeping tabs|
|<a id="sleepingtabstimeout"></a><a id="set-the-background-tab-inactivity-timeout-for-sleeping-tabs"></a>[SleepingTabsTimeout](microsoft-edge-browser-policies/SleepingTabsTimeout.md)|Set the background tab inactivity timeout for sleeping tabs|

<a id="smartscreen-settings-policies"></a>
### SmartScreen settings

|Policy Name|Caption|
|-|-|
|<a id="exemptsmartscreendownloadwarnings"></a><a id="disable-smartscreen-apprep-based-warnings-for-specified-file-types-on-specified-domains"></a>[ExemptSmartScreenDownloadWarnings](microsoft-edge-browser-policies/ExemptSmartScreenDownloadWarnings.md)|Disable SmartScreen AppRep based warnings for specified file types on specified domains|
|<a id="newsmartscreenlibraryenabled"></a><a id="enable-new-smartscreen-library-obsolete"></a>[NewSmartScreenLibraryEnabled](microsoft-edge-browser-policies/NewSmartScreenLibraryEnabled.md)|Enable new SmartScreen library (obsolete)|
|<a id="preventsmartscreenpromptoverride"></a><a id="prevent-bypassing-microsoft-defender-smartscreen-prompts-for-sites"></a>[PreventSmartScreenPromptOverride](microsoft-edge-browser-policies/PreventSmartScreenPromptOverride.md)|Prevent bypassing Microsoft Defender SmartScreen prompts for sites|
|<a id="preventsmartscreenpromptoverrideforfiles"></a><a id="prevent-bypassing-of-microsoft-defender-smartscreen-warnings-about-downloads"></a>[PreventSmartScreenPromptOverrideForFiles](microsoft-edge-browser-policies/PreventSmartScreenPromptOverrideForFiles.md)|Prevent bypassing of Microsoft Defender SmartScreen warnings about downloads|
|<a id="smartscreenallowlistdomains"></a><a id="configure-the-list-of-domains-for-which-microsoft-defender-smartscreen-wont-trigger-warnings"></a>[SmartScreenAllowListDomains](microsoft-edge-browser-policies/SmartScreenAllowListDomains.md)|Configure the list of domains for which Microsoft Defender SmartScreen won't trigger warnings|
|<a id="smartscreendnsrequestsenabled"></a><a id="enable-microsoft-defender-smartscreen-dns-requests"></a>[SmartScreenDnsRequestsEnabled](microsoft-edge-browser-policies/SmartScreenDnsRequestsEnabled.md)|Enable Microsoft Defender SmartScreen DNS requests|
|<a id="smartscreenenabled"></a><a id="configure-microsoft-defender-smartscreen"></a>[SmartScreenEnabled](microsoft-edge-browser-policies/SmartScreenEnabled.md)|Configure Microsoft Defender SmartScreen|
|<a id="smartscreenfortrusteddownloadsenabled"></a><a id="force-microsoft-defender-smartscreen-checks-on-downloads-from-trusted-sources"></a>[SmartScreenForTrustedDownloadsEnabled](microsoft-edge-browser-policies/SmartScreenForTrustedDownloadsEnabled.md)|Force Microsoft Defender SmartScreen checks on downloads from trusted sources|
|<a id="smartscreenpuaenabled"></a><a id="configure-microsoft-defender-smartscreen-to-block-potentially-unwanted-apps"></a>[SmartScreenPuaEnabled](microsoft-edge-browser-policies/SmartScreenPuaEnabled.md)|Configure Microsoft Defender SmartScreen to block potentially unwanted apps|

<a id="startup-home-page-and-new-tab-page-policies"></a>
### Startup&comma; home page and new tab page

|Policy Name|Caption|
|-|-|
|<a id="homepageisnewtabpage"></a><a id="set-the-new-tab-page-as-the-home-page"></a>[HomepageIsNewTabPage](microsoft-edge-browser-policies/HomepageIsNewTabPage.md)|Set the new tab page as the home page|
|<a id="homepagelocation"></a><a id="configure-the-home-page-url"></a>[HomepageLocation](microsoft-edge-browser-policies/HomepageLocation.md)|Configure the home page URL|
|<a id="newtabpageallowedbackgroundtypes"></a><a id="configure-the-background-types-allowed-for-the-new-tab-page-layout"></a>[NewTabPageAllowedBackgroundTypes](microsoft-edge-browser-policies/NewTabPageAllowedBackgroundTypes.md)|Configure the background types allowed for the new tab page layout|
|<a id="newtabpageapplauncherenabled"></a><a id="hide-app-launcher-on-microsoft-edge-new-tab-page"></a>[NewTabPageAppLauncherEnabled](microsoft-edge-browser-policies/NewTabPageAppLauncherEnabled.md)|Hide App Launcher on Microsoft Edge new tab page|
|<a id="newtabpagebingchatenabled"></a><a id="disable-bing-chat-entry-points-on-microsoft-edge-enterprise-new-tab-page"></a>[NewTabPageBingChatEnabled](microsoft-edge-browser-policies/NewTabPageBingChatEnabled.md)|Disable Bing chat entry-points on Microsoft Edge Enterprise new tab page|
|<a id="newtabpagecompanylogo"></a><a id="set-new-tab-page-company-logo-obsolete"></a>[NewTabPageCompanyLogo](microsoft-edge-browser-policies/NewTabPageCompanyLogo.md)|Set new tab page company logo (obsolete)|
|<a id="newtabpagecompanylogobackplatecolor"></a><a id="set-the-company-logo-backplate-color-on-the-new-tab-page"></a>[NewTabPageCompanyLogoBackplateColor](microsoft-edge-browser-policies/NewTabPageCompanyLogoBackplateColor.md)|Set the company logo backplate color on the new tab page.|
|<a id="newtabpagecompanylogoenabled"></a><a id="hide-the-company-logo-on-the-microsoft-edge-new-tab-page"></a>[NewTabPageCompanyLogoEnabled](microsoft-edge-browser-policies/NewTabPageCompanyLogoEnabled.md)|Hide the company logo on the Microsoft Edge new tab page|
|<a id="newtabpagecontentenabled"></a><a id="allow-microsoft-content-on-the-new-tab-page"></a>[NewTabPageContentEnabled](microsoft-edge-browser-policies/NewTabPageContentEnabled.md)|Allow Microsoft content on the new tab page|
|<a id="newtabpagehidedefaulttopsites"></a><a id="hide-the-default-top-sites-from-the-new-tab-page"></a>[NewTabPageHideDefaultTopSites](microsoft-edge-browser-policies/NewTabPageHideDefaultTopSites.md)|Hide the default top sites from the new tab page|
|<a id="newtabpagelocation"></a><a id="configure-the-new-tab-page-url"></a>[NewTabPageLocation](microsoft-edge-browser-policies/NewTabPageLocation.md)|Configure the new tab page URL|
|<a id="newtabpagemanagedquicklinks"></a><a id="set-new-tab-page-quick-links"></a>[NewTabPageManagedQuickLinks](microsoft-edge-browser-policies/NewTabPageManagedQuickLinks.md)|Set new tab page quick links|
|<a id="newtabpageprerenderenabled"></a><a id="enable-preload-of-the-new-tab-page-for-faster-rendering"></a>[NewTabPagePrerenderEnabled](microsoft-edge-browser-policies/NewTabPagePrerenderEnabled.md)|Enable preload of the new tab page for faster rendering|
|<a id="newtabpagequicklinksenabled"></a><a id="allow-quick-links-on-the-new-tab-page"></a>[NewTabPageQuickLinksEnabled](microsoft-edge-browser-policies/NewTabPageQuickLinksEnabled.md)|Allow quick links on the new tab page|
|<a id="newtabpagesetfeedtype"></a><a id="configure-the-microsoft-edge-new-tab-page-experience-obsolete"></a>[NewTabPageSetFeedType](microsoft-edge-browser-policies/NewTabPageSetFeedType.md)|Configure the Microsoft Edge new tab page experience (obsolete)|
|<a id="restoreonstartup"></a><a id="action-to-take-on-microsoft-edge-startup"></a>[RestoreOnStartup](microsoft-edge-browser-policies/RestoreOnStartup.md)|Action to take on Microsoft Edge startup|
|<a id="restoreonstartupurls"></a><a id="sites-to-open-when-the-browser-starts"></a>[RestoreOnStartupURLs](microsoft-edge-browser-policies/RestoreOnStartupURLs.md)|Sites to open when the browser starts|
|<a id="restoreonstartupuserurlsenabled"></a><a id="allow-users-to-add-and-remove-their-own-sites-during-startup-when-the-restoreonstartupurls-policy-is-configured"></a>[RestoreOnStartupUserURLsEnabled](microsoft-edge-browser-policies/RestoreOnStartupUserURLsEnabled.md)|Allow users to add and remove their own sites during startup when the RestoreOnStartupURLs policy is configured|
|<a id="showhomebutton"></a><a id="show-home-button-on-toolbar"></a>[ShowHomeButton](microsoft-edge-browser-policies/ShowHomeButton.md)|Show Home button on toolbar|

<a id="webrtc-settings-policies"></a>
### WebRtc settings

|Policy Name|Caption|
|-|-|
|<a id="webrtciphandlingurl"></a><a id="webrtc-ip-handling-policy-for-url-patterns"></a>[WebRtcIPHandlingUrl](microsoft-edge-browser-policies/WebRtcIPHandlingUrl.md)|WebRTC IP Handling Policy for URL Patterns|
|<a id="webrtclocalhostiphandling"></a><a id="restrict-exposure-of-local-ip-address-by-webrtc"></a>[WebRtcLocalhostIpHandling](microsoft-edge-browser-policies/WebRtcLocalhostIpHandling.md)|Restrict exposure of local IP address by WebRTC|

<a id="additional-policies"></a>
### Additional

|Policy Name|Caption|
|-|-|
|<a id="aadwebsitessousingthisprofileenabled"></a><a id="single-sign-on-for-work-or-school-sites-using-this-profile-enabled"></a>[AADWebSiteSSOUsingThisProfileEnabled](microsoft-edge-browser-policies/AADWebSiteSSOUsingThisProfileEnabled.md)|Single sign-on for work or school sites using this profile enabled|
|<a id="aigenthemesenabled"></a><a id="enables-dall-e-themes-generation"></a>[AIGenThemesEnabled](microsoft-edge-browser-policies/AIGenThemesEnabled.md)|Enables DALL-E themes generation|
|<a id="accessibilityimagelabelsenabled"></a><a id="let-screen-reader-users-get-image-descriptions-from-microsoft"></a>[AccessibilityImageLabelsEnabled](microsoft-edge-browser-policies/AccessibilityImageLabelsEnabled.md)|Let screen reader users get image descriptions from Microsoft|
|<a id="adhoccodesigningforpwasenabled"></a><a id="native-application-signing-during-progressive-web-application-installation"></a>[AdHocCodeSigningForPWAsEnabled](microsoft-edge-browser-policies/AdHocCodeSigningForPWAsEnabled.md)|Native application signing during Progressive Web Application installation|
|<a id="additionalsearchboxenabled"></a><a id="enable-additional-search-box-in-browser"></a>[AdditionalSearchBoxEnabled](microsoft-edge-browser-policies/AdditionalSearchBoxEnabled.md)|Enable additional search box in browser|
|<a id="addressbareditingenabled"></a><a id="configure-address-bar-editing"></a>[AddressBarEditingEnabled](microsoft-edge-browser-policies/AddressBarEditingEnabled.md)|Configure address bar editing|
|<a id="addressbarmicrosoftsearchinbingproviderenabled"></a><a id="enable-microsoft-search-in-bing-suggestions-in-the-address-bar-deprecated"></a>[AddressBarMicrosoftSearchInBingProviderEnabled](microsoft-edge-browser-policies/AddressBarMicrosoftSearchInBingProviderEnabled.md)|Enable Microsoft Search in Bing suggestions in the address bar (deprecated)|
|<a id="addressbartrendingsuggestenabled"></a><a id="enable-microsoft-bing-trending-suggestions-in-the-address-bar"></a>[AddressBarTrendingSuggestEnabled](microsoft-edge-browser-policies/AddressBarTrendingSuggestEnabled.md)|Enable Microsoft Bing trending suggestions in the address bar|
|<a id="addressbarworksearchresultsenabled"></a><a id="enable-work-search-suggestions-in-the-address-bar"></a>[AddressBarWorkSearchResultsEnabled](microsoft-edge-browser-policies/AddressBarWorkSearchResultsEnabled.md)|Enable Work Search suggestions in the address bar|
|<a id="adssettingforintrusiveadssites"></a><a id="ads-setting-for-sites-with-intrusive-ads"></a>[AdsSettingForIntrusiveAdsSites](microsoft-edge-browser-policies/AdsSettingForIntrusiveAdsSites.md)|Ads setting for sites with intrusive ads|
|<a id="adstransparencyenabled"></a><a id="configure-if-the-ads-transparency-feature-is-enabled"></a>[AdsTransparencyEnabled](microsoft-edge-browser-policies/AdsTransparencyEnabled.md)|Configure if the ads transparency feature is enabled|
|<a id="allowbackforwardcacheforcachecontrolnostorepageenabled"></a><a id="allow-pages-with-cache-control-no-store-header-to-enter-backforward-cache"></a>[AllowBackForwardCacheForCacheControlNoStorePageEnabled](microsoft-edge-browser-policies/AllowBackForwardCacheForCacheControlNoStorePageEnabled.md)|Allow pages with Cache-Control: no-store header to enter back/forward cache|
|<a id="allowdeletingbrowserhistory"></a><a id="enable-deleting-browser-and-download-history"></a>[AllowDeletingBrowserHistory](microsoft-edge-browser-policies/AllowDeletingBrowserHistory.md)|Enable deleting browser and download history|
|<a id="allowfileselectiondialogs"></a><a id="allow-file-selection-dialogs"></a>[AllowFileSelectionDialogs](microsoft-edge-browser-policies/AllowFileSelectionDialogs.md)|Allow file selection dialogs|
|<a id="allowgamesmenu"></a><a id="allow-users-to-access-the-games-menu-deprecated"></a>[AllowGamesMenu](microsoft-edge-browser-policies/AllowGamesMenu.md)|Allow users to access the games menu (deprecated)|
|<a id="allowpopupsduringpageunload"></a><a id="allows-a-page-to-show-popups-during-its-unloading-obsolete"></a>[AllowPopupsDuringPageUnload](microsoft-edge-browser-policies/AllowPopupsDuringPageUnload.md)|Allows a page to show popups during its unloading (obsolete)|
|<a id="allowsurfgame"></a><a id="allow-surf-game"></a>[AllowSurfGame](microsoft-edge-browser-policies/AllowSurfGame.md)|Allow surf game|
|<a id="allowsyncxhrinpagedismissal"></a><a id="allow-pages-to-send-synchronous-xhr-requests-during-page-dismissal-obsolete"></a>[AllowSyncXHRInPageDismissal](microsoft-edge-browser-policies/AllowSyncXHRInPageDismissal.md)|Allow pages to send synchronous XHR requests during page dismissal (obsolete)|
|<a id="allowsystemnotifications"></a><a id="allows-system-notifications"></a>[AllowSystemNotifications](microsoft-edge-browser-policies/AllowSystemNotifications.md)|Allows system notifications|
|<a id="allowtokenbindingforurls"></a><a id="configure-the-list-of-sites-for-which-microsoft-edge-will-attempt-to-establish-a-token-binding-with-obsolete"></a>[AllowTokenBindingForUrls](microsoft-edge-browser-policies/AllowTokenBindingForUrls.md)|Configure the list of sites for which Microsoft Edge will attempt to establish a Token Binding with (obsolete)|
|<a id="allowtrackingforurls"></a><a id="configure-tracking-prevention-exceptions-for-specific-sites"></a>[AllowTrackingForUrls](microsoft-edge-browser-policies/AllowTrackingForUrls.md)|Configure tracking prevention exceptions for specific sites|
|<a id="allowwebauthnwithbrokentlscerts"></a><a id="allow-web-authentication-requests-on-sites-with-broken-tls-certificates"></a>[AllowWebAuthnWithBrokenTlsCerts](microsoft-edge-browser-policies/AllowWebAuthnWithBrokenTlsCerts.md)|Allow Web Authentication requests on sites with broken TLS certificates.|
|<a id="alloweddomainsforapps"></a><a id="define-domains-allowed-to-access-google-workspace"></a>[AllowedDomainsForApps](microsoft-edge-browser-policies/AllowedDomainsForApps.md)|Define domains allowed to access Google Workspace|
|<a id="alternateerrorpagesenabled"></a><a id="suggest-similar-pages-when-a-webpage-cant-be-found"></a>[AlternateErrorPagesEnabled](microsoft-edge-browser-policies/AlternateErrorPagesEnabled.md)|Suggest similar pages when a webpage can't be found|
|<a id="alwaysopenpdfexternally"></a><a id="always-open-pdf-files-externally"></a>[AlwaysOpenPdfExternally](microsoft-edge-browser-policies/AlwaysOpenPdfExternally.md)|Always open PDF files externally|
|<a id="ambientauthenticationinprivatemodesenabled"></a><a id="enable-ambient-authentication-for-inprivate-and-guest-profiles"></a>[AmbientAuthenticationInPrivateModesEnabled](microsoft-edge-browser-policies/AmbientAuthenticationInPrivateModesEnabled.md)|Enable Ambient Authentication for InPrivate and Guest profiles|
|<a id="appcacheforceenabled"></a><a id="allows-the-appcache-feature-to-be-re-enabled-even-if-its-turned-off-by-default-obsolete"></a>[AppCacheForceEnabled](microsoft-edge-browser-policies/AppCacheForceEnabled.md)|Allows the AppCache feature to be re-enabled, even if it's turned off by default (obsolete)|
|<a id="applicationboundencryptionenabled"></a><a id="enable-application-bound-encryption"></a>[ApplicationBoundEncryptionEnabled](microsoft-edge-browser-policies/ApplicationBoundEncryptionEnabled.md)|Enable Application Bound Encryption|
|<a id="applicationlocalevalue"></a><a id="set-application-locale"></a>[ApplicationLocaleValue](microsoft-edge-browser-policies/ApplicationLocaleValue.md)|Set application locale|
|<a id="askbeforecloseenabled"></a><a id="get-user-confirmation-before-closing-a-browser-window-with-multiple-tabs"></a>[AskBeforeCloseEnabled](microsoft-edge-browser-policies/AskBeforeCloseEnabled.md)|Get user confirmation before closing a browser window with multiple tabs|
|<a id="audiocaptureallowed"></a><a id="allow-or-block-audio-capture"></a>[AudioCaptureAllowed](microsoft-edge-browser-policies/AudioCaptureAllowed.md)|Allow or block audio capture|
|<a id="audiocaptureallowedurls"></a><a id="sites-that-can-access-audio-capture-devices-without-requesting-permission"></a>[AudioCaptureAllowedUrls](microsoft-edge-browser-policies/AudioCaptureAllowedUrls.md)|Sites that can access audio capture devices without requesting permission|
|<a id="audioprocesshighpriorityenabled"></a><a id="allow-the-audio-process-to-run-with-priority-above-normal-on-windows"></a>[AudioProcessHighPriorityEnabled](microsoft-edge-browser-policies/AudioProcessHighPriorityEnabled.md)|Allow the audio process to run with priority above normal on Windows|
|<a id="audiosandboxenabled"></a><a id="allow-the-audio-sandbox-to-run"></a>[AudioSandboxEnabled](microsoft-edge-browser-policies/AudioSandboxEnabled.md)|Allow the audio sandbox to run|
|<a id="autoimportatfirstrun"></a><a id="automatically-import-another-browsers-data-and-settings-at-first-run"></a>[AutoImportAtFirstRun](microsoft-edge-browser-policies/AutoImportAtFirstRun.md)|Automatically import another browser's data and settings at first run|
|<a id="autolaunchprotocolscomponentenabled"></a><a id="autolaunch-protocols-component-enabled"></a>[AutoLaunchProtocolsComponentEnabled](microsoft-edge-browser-policies/AutoLaunchProtocolsComponentEnabled.md)|AutoLaunch Protocols Component Enabled|
|<a id="autolaunchprotocolsfromorigins"></a><a id="define-a-list-of-protocols-that-can-launch-an-external-application-from-listed-origins-without-prompting-the-user"></a>[AutoLaunchProtocolsFromOrigins](microsoft-edge-browser-policies/AutoLaunchProtocolsFromOrigins.md)|Define a list of protocols that can launch an external application from listed origins without prompting the user|
|<a id="autoopenallowedforurls"></a><a id="urls-where-autoopenfiletypes-can-apply"></a>[AutoOpenAllowedForURLs](microsoft-edge-browser-policies/AutoOpenAllowedForURLs.md)|URLs where AutoOpenFileTypes can apply|
|<a id="autoopenfiletypes"></a><a id="list-of-file-types-that-should-be-automatically-opened-on-download"></a>[AutoOpenFileTypes](microsoft-edge-browser-policies/AutoOpenFileTypes.md)|List of file types that should be automatically opened on download|
|<a id="autofilladdressenabled"></a><a id="enable-autofill-for-addresses"></a>[AutofillAddressEnabled](microsoft-edge-browser-policies/AutofillAddressEnabled.md)|Enable AutoFill for addresses|
|<a id="autofillcreditcardenabled"></a><a id="enable-autofill-for-payment-instruments"></a>[AutofillCreditCardEnabled](microsoft-edge-browser-policies/AutofillCreditCardEnabled.md)|Enable AutoFill for payment instruments|
|<a id="autofillmembershipsenabled"></a><a id="save-and-fill-memberships"></a>[AutofillMembershipsEnabled](microsoft-edge-browser-policies/AutofillMembershipsEnabled.md)|Save and fill memberships|
|<a id="automatichttpsdefault"></a><a id="configure-automatic-https-deprecated"></a>[AutomaticHttpsDefault](microsoft-edge-browser-policies/AutomaticHttpsDefault.md)|Configure Automatic HTTPS (deprecated)|
|<a id="autoplayallowed"></a><a id="allow-media-autoplay-for-websites"></a>[AutoplayAllowed](microsoft-edge-browser-policies/AutoplayAllowed.md)|Allow media autoplay for websites|
|<a id="autoplayallowlist"></a><a id="allow-media-autoplay-on-specific-sites"></a>[AutoplayAllowlist](microsoft-edge-browser-policies/AutoplayAllowlist.md)|Allow media autoplay on specific sites|
|<a id="backgroundmodeenabled"></a><a id="continue-running-background-apps-after-microsoft-edge-closes"></a>[BackgroundModeEnabled](microsoft-edge-browser-policies/BackgroundModeEnabled.md)|Continue running background apps after Microsoft Edge closes|
|<a id="backgroundtemplatelistupdatesenabled"></a><a id="enables-background-updates-to-the-list-of-available-templates-for-collections-and-other-features-that-use-templates-deprecated"></a>[BackgroundTemplateListUpdatesEnabled](microsoft-edge-browser-policies/BackgroundTemplateListUpdatesEnabled.md)|Enables background updates to the list of available templates for Collections and other features that use templates (deprecated)|
|<a id="beforeunloadeventcancelbypreventdefaultenabled"></a><a id="control-the-behavior-for-the-cancel-dialog-produced-by-the-beforeunload-event-obsolete"></a>[BeforeunloadEventCancelByPreventDefaultEnabled](microsoft-edge-browser-policies/BeforeunloadEventCancelByPreventDefaultEnabled.md)|Control the behavior for the cancel dialog produced by the beforeunload event (obsolete)|
|<a id="bingadssuppression"></a><a id="block-all-ads-on-bing-search-results"></a>[BingAdsSuppression](microsoft-edge-browser-policies/BingAdsSuppression.md)|Block all ads on Bing search results|
|<a id="blockthirdpartycookies"></a><a id="block-third-party-cookies"></a>[BlockThirdPartyCookies](microsoft-edge-browser-policies/BlockThirdPartyCookies.md)|Block third party cookies|
|<a id="browseraddprofileenabled"></a><a id="enable-profile-creation-from-the-identity-flyout-menu-or-the-settings-page"></a>[BrowserAddProfileEnabled](microsoft-edge-browser-policies/BrowserAddProfileEnabled.md)|Enable profile creation from the Identity flyout menu or the Settings page|
|<a id="browsercodeintegritysetting"></a><a id="configure-browser-process-code-integrity-guard-setting"></a>[BrowserCodeIntegritySetting](microsoft-edge-browser-policies/BrowserCodeIntegritySetting.md)|Configure browser process code integrity guard setting|
|<a id="browserguestmodeenabled"></a><a id="enable-guest-mode"></a>[BrowserGuestModeEnabled](microsoft-edge-browser-policies/BrowserGuestModeEnabled.md)|Enable guest mode|
|<a id="browserlegacyextensionpointsblockingenabled"></a><a id="enable-browser-legacy-extension-point-blocking"></a>[BrowserLegacyExtensionPointsBlockingEnabled](microsoft-edge-browser-policies/BrowserLegacyExtensionPointsBlockingEnabled.md)|Enable browser legacy extension point blocking|
|<a id="browsernetworktimequeriesenabled"></a><a id="allow-queries-to-a-browser-network-time-service"></a>[BrowserNetworkTimeQueriesEnabled](microsoft-edge-browser-policies/BrowserNetworkTimeQueriesEnabled.md)|Allow queries to a Browser Network Time service|
|<a id="browsersignin"></a><a id="browser-sign-in-settings"></a>[BrowserSignin](microsoft-edge-browser-policies/BrowserSignin.md)|Browser sign-in settings|
|<a id="browsingdatalifetime"></a><a id="browsing-data-lifetime-settings"></a>[BrowsingDataLifetime](microsoft-edge-browser-policies/BrowsingDataLifetime.md)|Browsing Data Lifetime Settings|
|<a id="builtindnsclientenabled"></a><a id="use-built-in-dns-client"></a>[BuiltInDnsClientEnabled](microsoft-edge-browser-policies/BuiltInDnsClientEnabled.md)|Use built-in DNS client|
|<a id="builtincertificateverifierenabled"></a><a id="determines-whether-the-built-in-certificate-verifier-will-be-used-to-verify-server-certificates-obsolete"></a>[BuiltinCertificateVerifierEnabled](microsoft-edge-browser-policies/BuiltinCertificateVerifierEnabled.md)|Determines whether the built-in certificate verifier will be used to verify server certificates (obsolete)|
|<a id="cecpq2enabled"></a><a id="cecpq2-post-quantum-key-agreement-enabled-for-tls-obsolete"></a>[CECPQ2Enabled](microsoft-edge-browser-policies/CECPQ2Enabled.md)|CECPQ2 post-quantum key-agreement enabled for TLS (obsolete)|
|<a id="corsnonwildcardrequestheaderssupport"></a><a id="cors-non-wildcard-request-header-support-enabled"></a>[CORSNonWildcardRequestHeadersSupport](microsoft-edge-browser-policies/CORSNonWildcardRequestHeadersSupport.md)|CORS non-wildcard request header support enabled|
|<a id="csscustomstatedeprecatedsyntaxenabled"></a><a id="controls-whether-the-deprecated---foo-syntax-for-css-custom-state-is-enabled-obsolete"></a>[CSSCustomStateDeprecatedSyntaxEnabled](microsoft-edge-browser-policies/CSSCustomStateDeprecatedSyntaxEnabled.md)|Controls whether the deprecated :--foo syntax for CSS custom state is enabled (obsolete)|
|<a id="certificatetransparencyenforcementdisabledforcas"></a><a id="disable-certificate-transparency-enforcement-for-a-list-of-subjectpublickeyinfo-hashes"></a>[CertificateTransparencyEnforcementDisabledForCas](microsoft-edge-browser-policies/CertificateTransparencyEnforcementDisabledForCas.md)|Disable Certificate Transparency enforcement for a list of subjectPublicKeyInfo hashes|
|<a id="certificatetransparencyenforcementdisabledforlegacycas"></a><a id="disable-certificate-transparency-enforcement-for-a-list-of-legacy-certificate-authorities-obsolete"></a>[CertificateTransparencyEnforcementDisabledForLegacyCas](microsoft-edge-browser-policies/CertificateTransparencyEnforcementDisabledForLegacyCas.md)|Disable Certificate Transparency enforcement for a list of legacy certificate authorities (obsolete)|
|<a id="certificatetransparencyenforcementdisabledforurls"></a><a id="disable-certificate-transparency-enforcement-for-specific-urls"></a>[CertificateTransparencyEnforcementDisabledForUrls](microsoft-edge-browser-policies/CertificateTransparencyEnforcementDisabledForUrls.md)|Disable Certificate Transparency enforcement for specific URLs|
|<a id="clearbrowsingdataonexit"></a><a id="clear-browsing-data-when-microsoft-edge-closes"></a>[ClearBrowsingDataOnExit](microsoft-edge-browser-policies/ClearBrowsingDataOnExit.md)|Clear browsing data when Microsoft Edge closes|
|<a id="clearcachedimagesandfilesonexit"></a><a id="clear-cached-images-and-files-when-microsoft-edge-closes"></a>[ClearCachedImagesAndFilesOnExit](microsoft-edge-browser-policies/ClearCachedImagesAndFilesOnExit.md)|Clear cached images and files when Microsoft Edge closes|
|<a id="clickonceenabled"></a><a id="allow-users-to-open-files-using-the-clickonce-protocol"></a>[ClickOnceEnabled](microsoft-edge-browser-policies/ClickOnceEnabled.md)|Allow users to open files using the ClickOnce protocol|
|<a id="clipboardallowedforurls"></a><a id="allow-clipboard-use-on-specific-sites"></a>[ClipboardAllowedForUrls](microsoft-edge-browser-policies/ClipboardAllowedForUrls.md)|Allow clipboard use on specific sites|
|<a id="clipboardblockedforurls"></a><a id="block-clipboard-use-on-specific-sites"></a>[ClipboardBlockedForUrls](microsoft-edge-browser-policies/ClipboardBlockedForUrls.md)|Block clipboard use on specific sites|
|<a id="collectionsservicesandexportsblocklist"></a><a id="block-access-to-a-specified-list-of-services-and-export-targets-in-collections"></a>[CollectionsServicesAndExportsBlockList](microsoft-edge-browser-policies/CollectionsServicesAndExportsBlockList.md)|Block access to a specified list of services and export targets in Collections|
|<a id="commandlineflagsecuritywarningsenabled"></a><a id="enable-security-warnings-for-command-line-flags"></a>[CommandLineFlagSecurityWarningsEnabled](microsoft-edge-browser-policies/CommandLineFlagSecurityWarningsEnabled.md)|Enable security warnings for command-line flags|
|<a id="componentupdatesenabled"></a><a id="enable-component-updates-in-microsoft-edge"></a>[ComponentUpdatesEnabled](microsoft-edge-browser-policies/ComponentUpdatesEnabled.md)|Enable component updates in Microsoft Edge|
|<a id="composeinlineenabled"></a><a id="compose-is-enabled-for-writing-on-the-web"></a>[ComposeInlineEnabled](microsoft-edge-browser-policies/ComposeInlineEnabled.md)|Compose is enabled for writing on the web|
|<a id="configuredonottrack"></a><a id="configure-do-not-track"></a>[ConfigureDoNotTrack](microsoft-edge-browser-policies/ConfigureDoNotTrack.md)|Configure Do Not Track|
|<a id="configurefriendlyurlformat"></a><a id="configure-the-default-paste-format-of-urls-copied-from-microsoft-edge-and-determine-if-additional-formats-will-be-available-to-users"></a>[ConfigureFriendlyURLFormat](microsoft-edge-browser-policies/ConfigureFriendlyURLFormat.md)|Configure the default paste format of URLs copied from Microsoft Edge, and determine if additional formats will be available to users|
|<a id="configurekeyboardshortcuts"></a><a id="configure-the-list-of-commands-for-which-to-disable-keyboard-shortcuts"></a>[ConfigureKeyboardShortcuts](microsoft-edge-browser-policies/ConfigureKeyboardShortcuts.md)|Configure the list of commands for which to disable keyboard shortcuts|
|<a id="configureonpremisesaccountautosignin"></a><a id="configure-automatic-sign-in-with-an-active-directory-domain-account-when-there-is-no-azure-ad-domain-account"></a>[ConfigureOnPremisesAccountAutoSignIn](microsoft-edge-browser-policies/ConfigureOnPremisesAccountAutoSignIn.md)|Configure automatic sign in with an Active Directory domain account when there is no Azure AD domain account|
|<a id="configureonlinetexttospeech"></a><a id="configure-online-text-to-speech"></a>[ConfigureOnlineTextToSpeech](microsoft-edge-browser-policies/ConfigureOnlineTextToSpeech.md)|Configure Online Text To Speech|
|<a id="configureshare"></a><a id="configure-the-share-experience"></a>[ConfigureShare](microsoft-edge-browser-policies/ConfigureShare.md)|Configure the Share experience|
|<a id="configureviewinfileexplorer"></a><a id="configure-the-view-in-file-explorer-feature-for-sharepoint-pages-in-microsoft-edge"></a>[ConfigureViewInFileExplorer](microsoft-edge-browser-policies/ConfigureViewInFileExplorer.md)|Configure the View in File Explorer feature for SharePoint pages in Microsoft Edge|
|<a id="copilotcdppagecontext"></a><a id="control-copilot-with-commercial-data-protection-access-to-page-context-for-microsoft-entra-id-profiles-obsolete"></a>[CopilotCDPPageContext](microsoft-edge-browser-policies/CopilotCDPPageContext.md)|Control Copilot with Commercial Data Protection access to page context for Microsoft Entra ID profiles (obsolete)|
|<a id="copilotpagecontext"></a><a id="control-copilot-access-to-page-context-for-microsoft-entra-id-profiles"></a>[CopilotPageContext](microsoft-edge-browser-policies/CopilotPageContext.md)|Control Copilot access to page context for Microsoft Entra ID profiles|
|<a id="createpasskeysinicloudkeychain"></a><a id="control-whether-passkey-creation-will-default-to-icloud-keychain"></a>[CreatePasskeysInICloudKeychain](microsoft-edge-browser-policies/CreatePasskeysInICloudKeychain.md)|Control whether passkey creation will default to iCloud Keychain.|
|<a id="crossoriginwebassemblymodulesharingenabled"></a><a id="specifies-whether-webassembly-modules-can-be-sent-cross-origin-obsolete"></a>[CrossOriginWebAssemblyModuleSharingEnabled](microsoft-edge-browser-policies/CrossOriginWebAssemblyModuleSharingEnabled.md)|Specifies whether WebAssembly modules can be sent cross-origin (obsolete)|
|<a id="cryptowalletenabled"></a><a id="enable-cryptowallet-feature-obsolete"></a>[CryptoWalletEnabled](microsoft-edge-browser-policies/CryptoWalletEnabled.md)|Enable CryptoWallet feature (obsolete)|
|<a id="customhelplink"></a><a id="specify-custom-help-link"></a>[CustomHelpLink](microsoft-edge-browser-policies/CustomHelpLink.md)|Specify custom help link|
|<a id="dnsinterceptionchecksenabled"></a><a id="dns-interception-checks-enabled"></a>[DNSInterceptionChecksEnabled](microsoft-edge-browser-policies/DNSInterceptionChecksEnabled.md)|DNS interception checks enabled|
|<a id="defaultbrowsersettingenabled"></a><a id="set-microsoft-edge-as-default-browser"></a>[DefaultBrowserSettingEnabled](microsoft-edge-browser-policies/DefaultBrowserSettingEnabled.md)|Set Microsoft Edge as default browser|
|<a id="defaultbrowsersettingscampaignenabled"></a><a id="enables-default-browser-settings-campaigns"></a>[DefaultBrowserSettingsCampaignEnabled](microsoft-edge-browser-policies/DefaultBrowserSettingsCampaignEnabled.md)|Enables default browser settings campaigns|
|<a id="defaultclipboardsetting"></a><a id="default-clipboard-site-permission"></a>[DefaultClipboardSetting](microsoft-edge-browser-policies/DefaultClipboardSetting.md)|Default clipboard site permission|
|<a id="defaultsearchprovidercontextmenuaccessallowed"></a><a id="allow-default-search-provider-context-menu-search-access"></a>[DefaultSearchProviderContextMenuAccessAllowed](microsoft-edge-browser-policies/DefaultSearchProviderContextMenuAccessAllowed.md)|Allow default search provider context menu search access|
|<a id="defaultsensorssetting"></a><a id="default-sensors-setting"></a>[DefaultSensorsSetting](microsoft-edge-browser-policies/DefaultSensorsSetting.md)|Default sensors setting|
|<a id="defaultserialguardsetting"></a><a id="control-use-of-the-serial-api"></a>[DefaultSerialGuardSetting](microsoft-edge-browser-policies/DefaultSerialGuardSetting.md)|Control use of the Serial API|
|<a id="defaultshareadditionalosregionsetting"></a><a id="set-the-default-share-additional-operating-system-region-setting"></a>[DefaultShareAdditionalOSRegionSetting](microsoft-edge-browser-policies/DefaultShareAdditionalOSRegionSetting.md)|Set the default "share additional operating system region" setting|
|<a id="definepreferredlanguages"></a><a id="define-an-ordered-list-of-preferred-languages-that-websites-should-display-in-if-the-site-supports-the-language"></a>[DefinePreferredLanguages](microsoft-edge-browser-policies/DefinePreferredLanguages.md)|Define an ordered list of preferred languages that websites should display in if the site supports the language|
|<a id="delaynavigationsforinitialsitelistdownload"></a><a id="require-that-the-enterprise-mode-site-list-is-available-before-tab-navigation"></a>[DelayNavigationsForInitialSiteListDownload](microsoft-edge-browser-policies/DelayNavigationsForInitialSiteListDownload.md)|Require that the Enterprise Mode Site List is available before tab navigation|
|<a id="deletedataonmigration"></a><a id="delete-old-browser-data-on-migration"></a>[DeleteDataOnMigration](microsoft-edge-browser-policies/DeleteDataOnMigration.md)|Delete old browser data on migration|
|<a id="developertoolsavailability"></a><a id="control-where-developer-tools-can-be-used"></a>[DeveloperToolsAvailability](microsoft-edge-browser-policies/DeveloperToolsAvailability.md)|Control where developer tools can be used|
|<a id="diagnosticdata"></a><a id="send-required-and-optional-diagnostic-data-about-browser-usage"></a>[DiagnosticData](microsoft-edge-browser-policies/DiagnosticData.md)|Send required and optional diagnostic data about browser usage|
|<a id="directinvokeenabled"></a><a id="allow-users-to-open-files-using-the-directinvoke-protocol"></a>[DirectInvokeEnabled](microsoft-edge-browser-policies/DirectInvokeEnabled.md)|Allow users to open files using the DirectInvoke protocol|
|<a id="disable3dapis"></a><a id="disable-support-for-3d-graphics-apis"></a>[Disable3DAPIs](microsoft-edge-browser-policies/Disable3DAPIs.md)|Disable support for 3D graphics APIs|
|<a id="disablescreenshots"></a><a id="disable-taking-screenshots"></a>[DisableScreenshots](microsoft-edge-browser-policies/DisableScreenshots.md)|Disable taking screenshots|
|<a id="discoverpagecontextenabled"></a><a id="enable-discover-access-to-page-contents-for-aad-profiles-obsolete"></a>[DiscoverPageContextEnabled](microsoft-edge-browser-policies/DiscoverPageContextEnabled.md)|Enable Discover access to page contents for AAD profiles (obsolete)|
|<a id="diskcachedir"></a><a id="set-disk-cache-directory"></a>[DiskCacheDir](microsoft-edge-browser-policies/DiskCacheDir.md)|Set disk cache directory|
|<a id="diskcachesize"></a><a id="set-disk-cache-size-in-bytes"></a>[DiskCacheSize](microsoft-edge-browser-policies/DiskCacheSize.md)|Set disk cache size, in bytes|
|<a id="displaycapturepermissionspolicyenabled"></a><a id="specifies-whether-the-display-capture-permissions-policy-is-checked-or-skipped-obsolete"></a>[DisplayCapturePermissionsPolicyEnabled](microsoft-edge-browser-policies/DisplayCapturePermissionsPolicyEnabled.md)|Specifies whether the display-capture permissions-policy is checked or skipped (obsolete)|
|<a id="dnsoverhttpsmode"></a><a id="control-the-mode-of-dns-over-https"></a>[DnsOverHttpsMode](microsoft-edge-browser-policies/DnsOverHttpsMode.md)|Control the mode of DNS-over-HTTPS|
|<a id="dnsoverhttpstemplates"></a><a id="specify-uri-template-of-desired-dns-over-https-resolver"></a>[DnsOverHttpsTemplates](microsoft-edge-browser-policies/DnsOverHttpsTemplates.md)|Specify URI template of desired DNS-over-HTTPS resolver|
|<a id="donotsilentlyblockprotocolsfromorigins"></a><a id="define-a-list-of-protocols-that-can-not-be-silently-blocked-by-anti-flood-protection"></a>[DoNotSilentlyBlockProtocolsFromOrigins](microsoft-edge-browser-policies/DoNotSilentlyBlockProtocolsFromOrigins.md)|Define a list of protocols that can not be silently blocked by anti-flood protection|
|<a id="doubleclickclosetabenabled"></a><a id="double-click-feature-in-microsoft-edge-enabled-only-available-in-china"></a>[DoubleClickCloseTabEnabled](microsoft-edge-browser-policies/DoubleClickCloseTabEnabled.md)|Double Click feature in Microsoft Edge enabled (only available in China)|
|<a id="downloaddirectory"></a><a id="set-download-directory"></a>[DownloadDirectory](microsoft-edge-browser-policies/DownloadDirectory.md)|Set download directory|
|<a id="downloadrestrictions"></a><a id="allow-download-restrictions"></a>[DownloadRestrictions](microsoft-edge-browser-policies/DownloadRestrictions.md)|Allow download restrictions|
|<a id="dynamiccodesettings"></a><a id="dynamic-code-settings"></a>[DynamicCodeSettings](microsoft-edge-browser-policies/DynamicCodeSettings.md)|Dynamic Code Settings|
|<a id="edge3pserptelemetryenabled"></a><a id="edge-3p-serp-telemetry-enabled"></a>[Edge3PSerpTelemetryEnabled](microsoft-edge-browser-policies/Edge3PSerpTelemetryEnabled.md)|Edge 3P SERP Telemetry Enabled|
|<a id="edgeassetdeliveryserviceenabled"></a><a id="allow-features-to-download-assets-from-the-asset-delivery-service"></a>[EdgeAssetDeliveryServiceEnabled](microsoft-edge-browser-policies/EdgeAssetDeliveryServiceEnabled.md)|Allow features to download assets from the Asset Delivery Service|
|<a id="edgeautofillmlenabled"></a><a id="machine-learning-powered-autofill-suggestions"></a>[EdgeAutofillMlEnabled](microsoft-edge-browser-policies/EdgeAutofillMlEnabled.md)|Machine learning powered autofill suggestions|
|<a id="edgecollectionsenabled"></a><a id="enable-the-collections-feature"></a>[EdgeCollectionsEnabled](microsoft-edge-browser-policies/EdgeCollectionsEnabled.md)|Enable the Collections feature|
|<a id="edgediscoverenabled"></a><a id="discover-feature-in-microsoft-edge-obsolete"></a>[EdgeDiscoverEnabled](microsoft-edge-browser-policies/EdgeDiscoverEnabled.md)|Discover feature In Microsoft Edge (obsolete)|
|<a id="edgeedropenabled"></a><a id="enable-drop-feature-in-microsoft-edge"></a>[EdgeEDropEnabled](microsoft-edge-browser-policies/EdgeEDropEnabled.md)|Enable Drop feature in Microsoft Edge|
|<a id="edgeenhanceimagesenabled"></a><a id="enhance-images-enabled-obsolete"></a>[EdgeEnhanceImagesEnabled](microsoft-edge-browser-policies/EdgeEnhanceImagesEnabled.md)|Enhance images enabled (obsolete)|
|<a id="edgeentracopilotpagecontext"></a><a id="control-copilot-access-to-microsoft-edge-page-content-for-entra-account-user-profiles-when-using-copilot-in-the-microsoft-edge-sidepane"></a>[EdgeEntraCopilotPageContext](microsoft-edge-browser-policies/EdgeEntraCopilotPageContext.md)|Control Copilot access to Microsoft Edge page content for Entra account user profiles when using Copilot in the Microsoft Edge sidepane|
|<a id="edgefollowenabled"></a><a id="enable-follow-service-in-microsoft-edge-obsolete"></a>[EdgeFollowEnabled](microsoft-edge-browser-policies/EdgeFollowEnabled.md)|Enable Follow service in Microsoft Edge (obsolete)|
|<a id="edgeopeninsidebarenabled"></a><a id="enable-open-in-sidebar"></a>[EdgeOpenInSidebarEnabled](microsoft-edge-browser-policies/EdgeOpenInSidebarEnabled.md)|Enable open in sidebar|
|<a id="edgeshoppingassistantenabled"></a><a id="shopping-in-microsoft-edge-enabled"></a>[EdgeShoppingAssistantEnabled](microsoft-edge-browser-policies/EdgeShoppingAssistantEnabled.md)|Shopping in Microsoft Edge Enabled|
|<a id="edgesidebarappurlhostallowlist"></a><a id="allow-specific-apps-to-be-opened-in-microsoft-edge-sidebar"></a>[EdgeSidebarAppUrlHostAllowList](microsoft-edge-browser-policies/EdgeSidebarAppUrlHostAllowList.md)|Allow specific apps to be opened in Microsoft Edge sidebar|
|<a id="edgesidebarappurlhostblocklist"></a><a id="control-which-apps-cannot-be-opened-in-microsoft-edge-sidebar"></a>[EdgeSidebarAppUrlHostBlockList](microsoft-edge-browser-policies/EdgeSidebarAppUrlHostBlockList.md)|Control which apps cannot be opened in Microsoft Edge sidebar|
|<a id="edgesidebarappurlhostforcelist"></a><a id="control-which-apps-are-forced-to-be-shown-in-microsoft-edge-sidebar"></a>[EdgeSidebarAppUrlHostForceList](microsoft-edge-browser-policies/EdgeSidebarAppUrlHostForceList.md)|Control which apps are forced to be shown in Microsoft Edge sidebar|
|<a id="edgesidebarcustomizeenabled"></a><a id="enable-sidebar-customize"></a>[EdgeSidebarCustomizeEnabled](microsoft-edge-browser-policies/EdgeSidebarCustomizeEnabled.md)|Enable sidebar customize|
|<a id="edgewalletcheckoutenabled"></a><a id="enable-wallet-checkout-feature"></a>[EdgeWalletCheckoutEnabled](microsoft-edge-browser-policies/EdgeWalletCheckoutEnabled.md)|Enable Wallet Checkout feature|
|<a id="edgewalletetreeenabled"></a><a id="edge-wallet-e-tree-enabled"></a>[EdgeWalletEtreeEnabled](microsoft-edge-browser-policies/EdgeWalletEtreeEnabled.md)|Edge Wallet E-Tree Enabled|
|<a id="editfavoritesenabled"></a><a id="allows-users-to-edit-favorites"></a>[EditFavoritesEnabled](microsoft-edge-browser-policies/EditFavoritesEnabled.md)|Allows users to edit favorites|
|<a id="enabledeprecatedwebplatformfeatures"></a><a id="re-enable-deprecated-web-platform-features-for-a-limited-time-obsolete"></a>[EnableDeprecatedWebPlatformFeatures](microsoft-edge-browser-policies/EnableDeprecatedWebPlatformFeatures.md)|Re-enable deprecated web platform features for a limited time (obsolete)|
|<a id="enabledomainactionsdownload"></a><a id="enable-domain-actions-download-from-microsoft-obsolete"></a>[EnableDomainActionsDownload](microsoft-edge-browser-policies/EnableDomainActionsDownload.md)|Enable Domain Actions Download from Microsoft (obsolete)|
|<a id="enableonlinerevocationchecks"></a><a id="enable-online-ocspcrl-checks"></a>[EnableOnlineRevocationChecks](microsoft-edge-browser-policies/EnableOnlineRevocationChecks.md)|Enable online OCSP/CRL checks|
|<a id="enablesha1forlocalanchors"></a><a id="allow-certificates-signed-using-sha-1-when-issued-by-local-trust-anchors-obsolete"></a>[EnableSha1ForLocalAnchors](microsoft-edge-browser-policies/EnableSha1ForLocalAnchors.md)|Allow certificates signed using SHA-1 when issued by local trust anchors (obsolete)|
|<a id="encryptedclienthelloenabled"></a><a id="tls-encrypted-clienthello-enabled"></a>[EncryptedClientHelloEnabled](microsoft-edge-browser-policies/EncryptedClientHelloEnabled.md)|TLS Encrypted ClientHello Enabled|
|<a id="enforcelocalanchorconstraintsenabled"></a><a id="determines-whether-the-built-in-certificate-verifier-will-enforce-constraints-encoded-into-trust-anchors-loaded-from-the-platform-trust-store-obsolete"></a>[EnforceLocalAnchorConstraintsEnabled](microsoft-edge-browser-policies/EnforceLocalAnchorConstraintsEnabled.md)|Determines whether the built-in certificate verifier will enforce constraints encoded into trust anchors loaded from the platform trust store (obsolete)|
|<a id="enhancesecuritymode"></a><a id="enhance-the-security-state-in-microsoft-edge"></a>[EnhanceSecurityMode](microsoft-edge-browser-policies/EnhanceSecurityMode.md)|Enhance the security state in Microsoft Edge|
|<a id="enhancesecuritymodeallowuserbypass"></a><a id="allow-users-to-bypass-enhanced-security-mode"></a>[EnhanceSecurityModeAllowUserBypass](microsoft-edge-browser-policies/EnhanceSecurityModeAllowUserBypass.md)|Allow users to bypass Enhanced Security Mode|
|<a id="enhancesecuritymodebypassintranet"></a><a id="enhanced-security-mode-configuration-for-intranet-zone-sites"></a>[EnhanceSecurityModeBypassIntranet](microsoft-edge-browser-policies/EnhanceSecurityModeBypassIntranet.md)|Enhanced Security Mode configuration for Intranet zone sites|
|<a id="enhancesecuritymodebypasslistdomains"></a><a id="configure-the-list-of-domains-for-which-enhance-security-mode-will-not-be-enforced"></a>[EnhanceSecurityModeBypassListDomains](microsoft-edge-browser-policies/EnhanceSecurityModeBypassListDomains.md)|Configure the list of domains for which enhance security mode will not be enforced|
|<a id="enhancesecuritymodeenforcelistdomains"></a><a id="configure-the-list-of-domains-for-which-enhance-security-mode-will-always-be-enforced"></a>[EnhanceSecurityModeEnforceListDomains](microsoft-edge-browser-policies/EnhanceSecurityModeEnforceListDomains.md)|Configure the list of domains for which enhance security mode will always be enforced|
|<a id="enhancesecuritymodeindicatoruienabled"></a><a id="manage-the-indicator-ui-of-the-enhanced-security-mode-esm-feature-in-microsoft-edge"></a>[EnhanceSecurityModeIndicatorUIEnabled](microsoft-edge-browser-policies/EnhanceSecurityModeIndicatorUIEnabled.md)|Manage the indicator UI of the Enhanced Security Mode (ESM) feature in Microsoft Edge|
|<a id="enhancesecuritymodeoptoutuxenabled"></a><a id="manage-opt-out-user-experience-for-enhanced-security-mode-esm-in-microsoft-edge-obsolete"></a>[EnhanceSecurityModeOptOutUXEnabled](microsoft-edge-browser-policies/EnhanceSecurityModeOptOutUXEnabled.md)|Manage opt-out user experience for Enhanced Security Mode (ESM) in Microsoft Edge (obsolete)|
|<a id="enterprisehardwareplatformapienabled"></a><a id="allow-managed-extensions-to-use-the-enterprise-hardware-platform-api"></a>[EnterpriseHardwarePlatformAPIEnabled](microsoft-edge-browser-policies/EnterpriseHardwarePlatformAPIEnabled.md)|Allow managed extensions to use the Enterprise Hardware Platform API|
|<a id="enterprisemodesitelistmanagerallowed"></a><a id="allow-access-to-the-enterprise-mode-site-list-manager-tool"></a>[EnterpriseModeSiteListManagerAllowed](microsoft-edge-browser-policies/EnterpriseModeSiteListManagerAllowed.md)|Allow access to the Enterprise Mode Site List Manager tool|
|<a id="eventpathenabled"></a><a id="re-enable-the-eventpath-api-until-microsoft-edge-version-115-obsolete"></a>[EventPathEnabled](microsoft-edge-browser-policies/EventPathEnabled.md)|Re-enable the Event.path API until Microsoft Edge version 115 (obsolete)|
|<a id="exemptdomainfiletypepairsfromfiletypedownloadwarnings"></a><a id="disable-download-file-type-extension-based-warnings-for-specified-file-types-on-domains-obsolete"></a>[ExemptDomainFileTypePairsFromFileTypeDownloadWarnings](microsoft-edge-browser-policies/ExemptDomainFileTypePairsFromFileTypeDownloadWarnings.md)|Disable download file type extension-based warnings for specified file types on domains (obsolete)|
|<a id="exemptfiletypedownloadwarnings"></a><a id="disable-download-file-type-extension-based-warnings-for-specified-file-types-on-domains"></a>[ExemptFileTypeDownloadWarnings](microsoft-edge-browser-policies/ExemptFileTypeDownloadWarnings.md)|Disable download file type extension-based warnings for specified file types on domains|
|<a id="experimentationandconfigurationservicecontrol"></a><a id="control-communication-with-the-experimentation-and-configuration-service"></a>[ExperimentationAndConfigurationServiceControl](microsoft-edge-browser-policies/ExperimentationAndConfigurationServiceControl.md)|Control communication with the Experimentation and Configuration Service|
|<a id="explicitlyallowednetworkports"></a><a id="explicitly-allowed-network-ports"></a>[ExplicitlyAllowedNetworkPorts](microsoft-edge-browser-policies/ExplicitlyAllowedNetworkPorts.md)|Explicitly allowed network ports|
|<a id="externalprotocoldialogshowalwaysopencheckbox"></a><a id="show-an-always-open-checkbox-in-external-protocol-dialog"></a>[ExternalProtocolDialogShowAlwaysOpenCheckbox](microsoft-edge-browser-policies/ExternalProtocolDialogShowAlwaysOpenCheckbox.md)|Show an "Always open" checkbox in external protocol dialog|
|<a id="familysafetysettingsenabled"></a><a id="allow-users-to-configure-family-safety-and-kids-mode"></a>[FamilySafetySettingsEnabled](microsoft-edge-browser-policies/FamilySafetySettingsEnabled.md)|Allow users to configure Family safety and Kids Mode|
|<a id="favoritesbarenabled"></a><a id="enable-favorites-bar"></a>[FavoritesBarEnabled](microsoft-edge-browser-policies/FavoritesBarEnabled.md)|Enable favorites bar|
|<a id="fetchkeepalivedurationsecondsonshutdown"></a><a id="fetch-keepalive-duration-on-shutdown"></a>[FetchKeepaliveDurationSecondsOnShutdown](microsoft-edge-browser-policies/FetchKeepaliveDurationSecondsOnShutdown.md)|Fetch keepalive duration on shutdown|
|<a id="fileordirectorypickerwithoutgestureallowedfororigins"></a><a id="allow-file-or-directory-picker-apis-to-be-called-without-prior-user-gesture"></a>[FileOrDirectoryPickerWithoutGestureAllowedForOrigins](microsoft-edge-browser-policies/FileOrDirectoryPickerWithoutGestureAllowedForOrigins.md)|Allow file or directory picker APIs to be called without prior user gesture|
|<a id="forcebingsafesearch"></a><a id="enforce-bing-safesearch"></a>[ForceBingSafeSearch](microsoft-edge-browser-policies/ForceBingSafeSearch.md)|Enforce Bing SafeSearch|
|<a id="forcebuiltinpushmessagingclient"></a><a id="forces-microsoft-edge-to-use-its-built-in-wns-push-client-to-connect-to-the-windows-push-notification-service"></a>[ForceBuiltInPushMessagingClient](microsoft-edge-browser-policies/ForceBuiltInPushMessagingClient.md)|Forces Microsoft Edge to use its built-in WNS push client to connect to the Windows Push Notification Service.|
|<a id="forcecertificatepromptsonmultiplematches"></a><a id="configure-whether-microsoft-edge-should-automatically-select-a-certificate-when-there-are-multiple-certificate-matches-for-a-site-configured-with-autoselectcertificateforurls-deprecated"></a>[ForceCertificatePromptsOnMultipleMatches](microsoft-edge-browser-policies/ForceCertificatePromptsOnMultipleMatches.md)|Configure whether Microsoft Edge should automatically select a certificate when there are multiple certificate matches for a site configured with "AutoSelectCertificateForUrls" (deprecated)|
|<a id="forceephemeralprofiles"></a><a id="enable-use-of-ephemeral-profiles"></a>[ForceEphemeralProfiles](microsoft-edge-browser-policies/ForceEphemeralProfiles.md)|Enable use of ephemeral profiles|
|<a id="forcegooglesafesearch"></a><a id="enforce-google-safesearch"></a>[ForceGoogleSafeSearch](microsoft-edge-browser-policies/ForceGoogleSafeSearch.md)|Enforce Google SafeSearch|
|<a id="forcelegacydefaultreferrerpolicy"></a><a id="use-a-default-referrer-policy-of-no-referrer-when-downgrade-obsolete"></a>[ForceLegacyDefaultReferrerPolicy](microsoft-edge-browser-policies/ForceLegacyDefaultReferrerPolicy.md)|Use a default referrer policy of no-referrer-when-downgrade (obsolete)|
|<a id="forcemajorversiontominorpositioninuseragent"></a><a id="enable-or-disable-freezing-the-user-agent-string-at-major-version-99-obsolete"></a>[ForceMajorVersionToMinorPositionInUserAgent](microsoft-edge-browser-policies/ForceMajorVersionToMinorPositionInUserAgent.md)|Enable or disable freezing the User-Agent string at major version 99 (obsolete)|
|<a id="forcenetworkinprocess"></a><a id="force-networking-code-to-run-in-the-browser-process-obsolete"></a>[ForceNetworkInProcess](microsoft-edge-browser-policies/ForceNetworkInProcess.md)|Force networking code to run in the browser process (obsolete)|
|<a id="forcepermissionpolicyunloaddefaultenabled"></a><a id="controls-whether-unload-event-handlers-can-be-disabled"></a>[ForcePermissionPolicyUnloadDefaultEnabled](microsoft-edge-browser-policies/ForcePermissionPolicyUnloadDefaultEnabled.md)|Controls whether unload event handlers can be disabled.|
|<a id="forcesync"></a><a id="force-synchronization-of-browser-data-and-do-not-show-the-sync-consent-prompt"></a>[ForceSync](microsoft-edge-browser-policies/ForceSync.md)|Force synchronization of browser data and do not show the sync consent prompt|
|<a id="forcesynctypes"></a><a id="configure-the-list-of-types-that-are-included-for-synchronization"></a>[ForceSyncTypes](microsoft-edge-browser-policies/ForceSyncTypes.md)|Configure the list of types that are included for synchronization|
|<a id="forceyoutuberestrict"></a><a id="force-minimum-youtube-restricted-mode"></a>[ForceYouTubeRestrict](microsoft-edge-browser-policies/ForceYouTubeRestrict.md)|Force minimum YouTube Restricted Mode|
|<a id="fullscreenallowed"></a><a id="allow-full-screen-mode"></a>[FullscreenAllowed](microsoft-edge-browser-policies/FullscreenAllowed.md)|Allow full screen mode|
|<a id="globallyscopehttpauthcacheenabled"></a><a id="enable-globally-scoped-http-auth-cache"></a>[GloballyScopeHTTPAuthCacheEnabled](microsoft-edge-browser-policies/GloballyScopeHTTPAuthCacheEnabled.md)|Enable globally scoped HTTP auth cache|
|<a id="gotointranetsiteforsinglewordentryinaddressbar"></a><a id="force-direct-intranet-site-navigation-instead-of-searching-on-single-word-entries-in-the-address-bar"></a>[GoToIntranetSiteForSingleWordEntryInAddressBar](microsoft-edge-browser-policies/GoToIntranetSiteForSingleWordEntryInAddressBar.md)|Force direct intranet site navigation instead of searching on single word entries in the Address Bar|
|<a id="hstspolicybypasslist"></a><a id="configure-the-list-of-names-that-will-bypass-the-hsts-policy-check"></a>[HSTSPolicyBypassList](microsoft-edge-browser-policies/HSTSPolicyBypassList.md)|Configure the list of names that will bypass the HSTS policy check|
|<a id="hardwareaccelerationmodeenabled"></a><a id="use-graphics-acceleration-when-available"></a>[HardwareAccelerationModeEnabled](microsoft-edge-browser-policies/HardwareAccelerationModeEnabled.md)|Use graphics acceleration when available|
|<a id="headlessmodeenabled"></a><a id="control-use-of-the-headless-mode"></a>[HeadlessModeEnabled](microsoft-edge-browser-policies/HeadlessModeEnabled.md)|Control use of the Headless Mode|
|<a id="hidefirstrunexperience"></a><a id="hide-the-first-run-experience-and-splash-screen"></a>[HideFirstRunExperience](microsoft-edge-browser-policies/HideFirstRunExperience.md)|Hide the First-run experience and splash screen|
|<a id="hideinternetexplorerredirectuxforincompatiblesitesenabled"></a><a id="hide-the-one-time-redirection-dialog-and-the-banner-on-microsoft-edge"></a>[HideInternetExplorerRedirectUXForIncompatibleSitesEnabled](microsoft-edge-browser-policies/HideInternetExplorerRedirectUXForIncompatibleSitesEnabled.md)|Hide the one-time redirection dialog and the banner on Microsoft Edge|
|<a id="hiderestoredialogenabled"></a><a id="hide-restore-pages-dialog-after-browser-crash"></a>[HideRestoreDialogEnabled](microsoft-edge-browser-policies/HideRestoreDialogEnabled.md)|Hide restore pages dialog after browser crash|
|<a id="httpallowlist"></a><a id="http-allowlist"></a>[HttpAllowlist](microsoft-edge-browser-policies/HttpAllowlist.md)|HTTP Allowlist|
|<a id="httpsupgradesenabled"></a><a id="enable-automatic-https-upgrades"></a>[HttpsUpgradesEnabled](microsoft-edge-browser-policies/HttpsUpgradesEnabled.md)|Enable automatic HTTPS upgrades|
|<a id="hubssidebarenabled"></a><a id="show-hubs-sidebar"></a>[HubsSidebarEnabled](microsoft-edge-browser-policies/HubsSidebarEnabled.md)|Show Hubs Sidebar|
|<a id="importautofillformdata"></a><a id="allow-importing-of-autofill-form-data"></a>[ImportAutofillFormData](microsoft-edge-browser-policies/ImportAutofillFormData.md)|Allow importing of autofill form data|
|<a id="importbrowsersettings"></a><a id="allow-importing-of-browser-settings"></a>[ImportBrowserSettings](microsoft-edge-browser-policies/ImportBrowserSettings.md)|Allow importing of browser settings|
|<a id="importcookies"></a><a id="allow-importing-of-cookies"></a>[ImportCookies](microsoft-edge-browser-policies/ImportCookies.md)|Allow importing of Cookies|
|<a id="importextensions"></a><a id="allow-importing-of-extensions"></a>[ImportExtensions](microsoft-edge-browser-policies/ImportExtensions.md)|Allow importing of extensions|
|<a id="importfavorites"></a><a id="allow-importing-of-favorites"></a>[ImportFavorites](microsoft-edge-browser-policies/ImportFavorites.md)|Allow importing of favorites|
|<a id="importhistory"></a><a id="allow-importing-of-browsing-history"></a>[ImportHistory](microsoft-edge-browser-policies/ImportHistory.md)|Allow importing of browsing history|
|<a id="importhomepage"></a><a id="allow-importing-of-home-page-settings"></a>[ImportHomepage](microsoft-edge-browser-policies/ImportHomepage.md)|Allow importing of home page settings|
|<a id="importoneachlaunch"></a><a id="allow-import-of-data-from-other-browsers-on-each-microsoft-edge-launch"></a>[ImportOnEachLaunch](microsoft-edge-browser-policies/ImportOnEachLaunch.md)|Allow import of data from other browsers on each Microsoft Edge launch|
|<a id="importopentabs"></a><a id="allow-importing-of-open-tabs"></a>[ImportOpenTabs](microsoft-edge-browser-policies/ImportOpenTabs.md)|Allow importing of open tabs|
|<a id="importpaymentinfo"></a><a id="allow-importing-of-payment-info"></a>[ImportPaymentInfo](microsoft-edge-browser-policies/ImportPaymentInfo.md)|Allow importing of payment info|
|<a id="importsavedpasswords"></a><a id="allow-importing-of-saved-passwords"></a>[ImportSavedPasswords](microsoft-edge-browser-policies/ImportSavedPasswords.md)|Allow importing of saved passwords|
|<a id="importsearchengine"></a><a id="allow-importing-of-search-engine-settings"></a>[ImportSearchEngine](microsoft-edge-browser-policies/ImportSearchEngine.md)|Allow importing of search engine settings|
|<a id="importshortcuts"></a><a id="allow-importing-of-shortcuts"></a>[ImportShortcuts](microsoft-edge-browser-policies/ImportShortcuts.md)|Allow importing of shortcuts|
|<a id="importstartuppagesettings"></a><a id="allow-importing-of-startup-page-settings"></a>[ImportStartupPageSettings](microsoft-edge-browser-policies/ImportStartupPageSettings.md)|Allow importing of startup page settings|
|<a id="inappsupportenabled"></a><a id="in-app-support-enabled"></a>[InAppSupportEnabled](microsoft-edge-browser-policies/InAppSupportEnabled.md)|In-app support Enabled|
|<a id="inprivatemodeavailability"></a><a id="configure-inprivate-mode-availability"></a>[InPrivateModeAvailability](microsoft-edge-browser-policies/InPrivateModeAvailability.md)|Configure InPrivate mode availability|
|<a id="insecureformswarningsenabled"></a><a id="enable-warnings-for-insecure-forms-deprecated"></a>[InsecureFormsWarningsEnabled](microsoft-edge-browser-policies/InsecureFormsWarningsEnabled.md)|Enable warnings for insecure forms (deprecated)|
|<a id="intensivewakeupthrottlingenabled"></a><a id="control-the-intensivewakeupthrottling-feature"></a>[IntensiveWakeUpThrottlingEnabled](microsoft-edge-browser-policies/IntensiveWakeUpThrottlingEnabled.md)|Control the IntensiveWakeUpThrottling feature|
|<a id="internetexplorerintegrationalwaysuseoscapture"></a><a id="always-use-the-os-capture-engine-to-avoid-issues-with-capturing-internet-explorer-mode-tabs"></a>[InternetExplorerIntegrationAlwaysUseOSCapture](microsoft-edge-browser-policies/InternetExplorerIntegrationAlwaysUseOSCapture.md)|Always use the OS capture engine to avoid issues with capturing Internet Explorer mode tabs|
|<a id="internetexplorerintegrationalwayswaitforunload"></a><a id="wait-for-internet-explorer-mode-tabs-to-completely-unload-before-ending-the-browser-session"></a>[InternetExplorerIntegrationAlwaysWaitForUnload](microsoft-edge-browser-policies/InternetExplorerIntegrationAlwaysWaitForUnload.md)|Wait for Internet Explorer mode tabs to completely unload before ending the browser session|
|<a id="internetexplorerintegrationcloudneutralsitesreporting"></a><a id="configure-reporting-of-potentially-misconfigured-neutral-site-urls-to-the-m365-admin-center-site-lists-app"></a>[InternetExplorerIntegrationCloudNeutralSitesReporting](microsoft-edge-browser-policies/InternetExplorerIntegrationCloudNeutralSitesReporting.md)|Configure reporting of potentially misconfigured neutral site URLs to the M365 Admin Center Site Lists app|
|<a id="internetexplorerintegrationcloudsitelist"></a><a id="configure-the-enterprise-mode-cloud-site-list"></a>[InternetExplorerIntegrationCloudSiteList](microsoft-edge-browser-policies/InternetExplorerIntegrationCloudSiteList.md)|Configure the Enterprise Mode Cloud Site List|
|<a id="internetexplorerintegrationcloudusersitesreporting"></a><a id="configure-reporting-of-ie-mode-user-list-entries-to-the-m365-admin-center-site-lists-app"></a>[InternetExplorerIntegrationCloudUserSitesReporting](microsoft-edge-browser-policies/InternetExplorerIntegrationCloudUserSitesReporting.md)|Configure reporting of IE Mode user list entries to the M365 Admin Center Site Lists app|
|<a id="internetexplorerintegrationcomplexnavdatatypes"></a><a id="configure-whether-form-data-and-http-headers-will-be-sent-when-entering-or-exiting-internet-explorer-mode"></a>[InternetExplorerIntegrationComplexNavDataTypes](microsoft-edge-browser-policies/InternetExplorerIntegrationComplexNavDataTypes.md)|Configure whether form data and HTTP headers will be sent when entering or exiting Internet Explorer mode|
|<a id="internetexplorerintegrationenhancedhangdetection"></a><a id="configure-enhanced-hang-detection-for-internet-explorer-mode"></a>[InternetExplorerIntegrationEnhancedHangDetection](microsoft-edge-browser-policies/InternetExplorerIntegrationEnhancedHangDetection.md)|Configure enhanced hang detection for Internet Explorer mode|
|<a id="internetexplorerintegrationlevel"></a><a id="configure-internet-explorer-integration"></a>[InternetExplorerIntegrationLevel](microsoft-edge-browser-policies/InternetExplorerIntegrationLevel.md)|Configure Internet Explorer integration|
|<a id="internetexplorerintegrationlocalfileallowed"></a><a id="allow-launching-of-local-files-in-internet-explorer-mode"></a>[InternetExplorerIntegrationLocalFileAllowed](microsoft-edge-browser-policies/InternetExplorerIntegrationLocalFileAllowed.md)|Allow launching of local files in Internet Explorer mode|
|<a id="internetexplorerintegrationlocalfileextensionallowlist"></a><a id="open-local-files-in-internet-explorer-mode-file-extension-allow-list"></a>[InternetExplorerIntegrationLocalFileExtensionAllowList](microsoft-edge-browser-policies/InternetExplorerIntegrationLocalFileExtensionAllowList.md)|Open local files in Internet Explorer mode file extension allow list|
|<a id="internetexplorerintegrationlocalfileshowcontextmenu"></a><a id="show-context-menu-to-open-a-file-link-in-internet-explorer-mode"></a>[InternetExplorerIntegrationLocalFileShowContextMenu](microsoft-edge-browser-policies/InternetExplorerIntegrationLocalFileShowContextMenu.md)|Show context menu to open a file:// link in Internet Explorer mode|
|<a id="internetexplorerintegrationlocalmhtfileallowed"></a><a id="allow-local-mhtml-files-to-open-automatically-in-internet-explorer-mode"></a>[InternetExplorerIntegrationLocalMhtFileAllowed](microsoft-edge-browser-policies/InternetExplorerIntegrationLocalMhtFileAllowed.md)|Allow local MHTML files to open automatically in Internet Explorer mode|
|<a id="internetexplorerintegrationlocalsitelistexpirationdays"></a><a id="specify-the-number-of-days-that-a-site-remains-on-the-local-ie-mode-site-list"></a>[InternetExplorerIntegrationLocalSiteListExpirationDays](microsoft-edge-browser-policies/InternetExplorerIntegrationLocalSiteListExpirationDays.md)|Specify the number of days that a site remains on the local IE mode site list|
|<a id="internetexplorerintegrationreloadiniemodeallowed"></a><a id="allow-unconfigured-sites-to-be-reloaded-in-internet-explorer-mode"></a>[InternetExplorerIntegrationReloadInIEModeAllowed](microsoft-edge-browser-policies/InternetExplorerIntegrationReloadInIEModeAllowed.md)|Allow unconfigured sites to be reloaded in Internet Explorer mode|
|<a id="internetexplorerintegrationsitelist"></a><a id="configure-the-enterprise-mode-site-list"></a>[InternetExplorerIntegrationSiteList](microsoft-edge-browser-policies/InternetExplorerIntegrationSiteList.md)|Configure the Enterprise Mode Site List|
|<a id="internetexplorerintegrationsitelistrefreshinterval"></a><a id="configure-how-frequently-the-enterprise-mode-site-list-is-refreshed"></a>[InternetExplorerIntegrationSiteListRefreshInterval](microsoft-edge-browser-policies/InternetExplorerIntegrationSiteListRefreshInterval.md)|Configure how frequently the Enterprise Mode Site List is refreshed|
|<a id="internetexplorerintegrationsiteredirect"></a><a id="specify-how-in-page-navigations-to-unconfigured-sites-behave-when-started-from-internet-explorer-mode-pages"></a>[InternetExplorerIntegrationSiteRedirect](microsoft-edge-browser-policies/InternetExplorerIntegrationSiteRedirect.md)|Specify how "in-page" navigations to unconfigured sites behave when started from Internet Explorer mode pages|
|<a id="internetexplorerintegrationtestingallowed"></a><a id="allow-internet-explorer-mode-testing-obsolete"></a>[InternetExplorerIntegrationTestingAllowed](microsoft-edge-browser-policies/InternetExplorerIntegrationTestingAllowed.md)|Allow Internet Explorer mode testing (obsolete)|
|<a id="internetexplorerintegrationwindowopenheightadjustment"></a><a id="configure-the-pixel-adjustment-between-windowopen-heights-sourced-from-ie-mode-pages-vs-edge-mode-pages"></a>[InternetExplorerIntegrationWindowOpenHeightAdjustment](microsoft-edge-browser-policies/InternetExplorerIntegrationWindowOpenHeightAdjustment.md)|Configure the pixel adjustment between window.open heights sourced from IE mode pages vs. Edge mode pages|
|<a id="internetexplorerintegrationwindowopenwidthadjustment"></a><a id="configure-the-pixel-adjustment-between-windowopen-widths-sourced-from-ie-mode-pages-vs-edge-mode-pages"></a>[InternetExplorerIntegrationWindowOpenWidthAdjustment](microsoft-edge-browser-policies/InternetExplorerIntegrationWindowOpenWidthAdjustment.md)|Configure the pixel adjustment between window.open widths sourced from IE mode pages vs. Edge mode pages|
|<a id="internetexplorerintegrationzoneidentifiermhtfileallowed"></a><a id="automatically-open-downloaded-mht-or-mhtml-files-from-the-web-in-internet-explorer-mode"></a>[InternetExplorerIntegrationZoneIdentifierMhtFileAllowed](microsoft-edge-browser-policies/InternetExplorerIntegrationZoneIdentifierMhtFileAllowed.md)|Automatically open downloaded MHT or MHTML files from the web in Internet Explorer mode|
|<a id="internetexplorermodecleardataonexitenabled"></a><a id="clear-history-for-ie-and-ie-mode-every-time-you-exit"></a>[InternetExplorerModeClearDataOnExitEnabled](microsoft-edge-browser-policies/InternetExplorerModeClearDataOnExitEnabled.md)|Clear history for IE and IE mode every time you exit|
|<a id="internetexplorermodeenablesavepageas"></a><a id="allow-save-page-as-in-internet-explorer-mode"></a>[InternetExplorerModeEnableSavePageAs](microsoft-edge-browser-policies/InternetExplorerModeEnableSavePageAs.md)|Allow Save page as in Internet Explorer mode|
|<a id="internetexplorermodetabinedgemodeallowed"></a><a id="allow-sites-configured-for-internet-explorer-mode-to-open-in-microsoft-edge"></a>[InternetExplorerModeTabInEdgeModeAllowed](microsoft-edge-browser-policies/InternetExplorerModeTabInEdgeModeAllowed.md)|Allow sites configured for Internet Explorer mode to open in Microsoft Edge|
|<a id="internetexplorermodetoolbarbuttonenabled"></a><a id="show-the-reload-in-internet-explorer-mode-button-in-the-toolbar"></a>[InternetExplorerModeToolbarButtonEnabled](microsoft-edge-browser-policies/InternetExplorerModeToolbarButtonEnabled.md)|Show the Reload in Internet Explorer mode button in the toolbar|
|<a id="internetexplorersetforegroundwhenactive"></a><a id="keep-the-active-microsoft-edge-window-with-an-internet-explorer-mode-tab-always-in-the-foreground"></a>[InternetExplorerSetForegroundWhenActive](microsoft-edge-browser-policies/InternetExplorerSetForegroundWhenActive.md)|Keep the active Microsoft Edge window with an Internet Explorer mode tab always in the foreground.|
|<a id="internetexplorerzoomdisplay"></a><a id="display-zoom-in-ie-mode-tabs-with-dpi-scale-included-like-it-is-in-internet-explorer"></a>[InternetExplorerZoomDisplay](microsoft-edge-browser-policies/InternetExplorerZoomDisplay.md)|Display zoom in IE Mode tabs with DPI Scale included like it is in Internet Explorer|
|<a id="intranetredirectbehavior"></a><a id="intranet-redirection-behavior"></a>[IntranetRedirectBehavior](microsoft-edge-browser-policies/IntranetRedirectBehavior.md)|Intranet Redirection Behavior|
|<a id="isolateorigins"></a><a id="enable-site-isolation-for-specific-origins"></a>[IsolateOrigins](microsoft-edge-browser-policies/IsolateOrigins.md)|Enable site isolation for specific origins|
|<a id="keyboardfocusablescrollersenabled"></a><a id="enable-keyboard-focusable-scrollers"></a>[KeyboardFocusableScrollersEnabled](microsoft-edge-browser-policies/KeyboardFocusableScrollersEnabled.md)|Enable keyboard focusable scrollers|
|<a id="livecaptionsallowed"></a><a id="live-captions-allowed"></a>[LiveCaptionsAllowed](microsoft-edge-browser-policies/LiveCaptionsAllowed.md)|Live captions allowed|
|<a id="localbrowserdatashareenabled"></a><a id="enable-windows-to-search-local-microsoft-edge-browsing-data"></a>[LocalBrowserDataShareEnabled](microsoft-edge-browser-policies/LocalBrowserDataShareEnabled.md)|Enable Windows to search local Microsoft Edge browsing data|
|<a id="localprovidersenabled"></a><a id="allow-suggestions-from-local-providers"></a>[LocalProvidersEnabled](microsoft-edge-browser-policies/LocalProvidersEnabled.md)|Allow suggestions from local providers|
|<a id="mauenabled"></a><a id="always-use-microsoft-autoupdate-as-the-updater-for-microsoft-edge"></a>[MAUEnabled](microsoft-edge-browser-policies/MAUEnabled.md)|Always use Microsoft AutoUpdate as the updater for Microsoft Edge|
|<a id="msawebsitessousingthisprofileallowed"></a><a id="allow-single-sign-on-for-microsoft-personal-sites-using-this-profile"></a>[MSAWebSiteSSOUsingThisProfileAllowed](microsoft-edge-browser-policies/MSAWebSiteSSOUsingThisProfileAllowed.md)|Allow single sign-on for Microsoft personal sites using this profile|
|<a id="managedconfigurationperorigin"></a><a id="sets-managed-configuration-values-for-websites-to-specific-origins"></a>[ManagedConfigurationPerOrigin](microsoft-edge-browser-policies/ManagedConfigurationPerOrigin.md)|Sets managed configuration values for websites to specific origins|
|<a id="managedfavorites"></a><a id="configure-favorites"></a>[ManagedFavorites](microsoft-edge-browser-policies/ManagedFavorites.md)|Configure favorites|
|<a id="managedsearchengines"></a><a id="manage-search-engines"></a>[ManagedSearchEngines](microsoft-edge-browser-policies/ManagedSearchEngines.md)|Manage Search Engines|
|<a id="mathsolverenabled"></a><a id="let-users-snip-a-math-problem-and-get-the-solution-with-a-step-by-step-explanation-in-microsoft-edge-obsolete"></a>[MathSolverEnabled](microsoft-edge-browser-policies/MathSolverEnabled.md)|Let users snip a Math problem and get the solution with a step-by-step explanation in Microsoft Edge (obsolete)|
|<a id="maxconnectionsperproxy"></a><a id="maximum-number-of-concurrent-connections-to-the-proxy-server"></a>[MaxConnectionsPerProxy](microsoft-edge-browser-policies/MaxConnectionsPerProxy.md)|Maximum number of concurrent connections to the proxy server|
|<a id="mediaroutercastallowallips"></a><a id="allow-google-cast-to-connect-to-cast-devices-on-all-ip-addresses"></a>[MediaRouterCastAllowAllIPs](microsoft-edge-browser-policies/MediaRouterCastAllowAllIPs.md)|Allow Google Cast to connect to Cast devices on all IP addresses|
|<a id="metricsreportingenabled"></a><a id="enable-usage-and-crash-related-data-reporting-obsolete"></a>[MetricsReportingEnabled](microsoft-edge-browser-policies/MetricsReportingEnabled.md)|Enable usage and crash-related data reporting (obsolete)|
|<a id="microsoftedgeinsiderpromotionenabled"></a><a id="microsoft-edge-insider-promotion-enabled"></a>[MicrosoftEdgeInsiderPromotionEnabled](microsoft-edge-browser-policies/MicrosoftEdgeInsiderPromotionEnabled.md)|Microsoft Edge Insider Promotion Enabled|
|<a id="microsofteditorproofingenabled"></a><a id="spell-checking-provided-by-microsoft-editor"></a>[MicrosoftEditorProofingEnabled](microsoft-edge-browser-policies/MicrosoftEditorProofingEnabled.md)|Spell checking provided by Microsoft Editor|
|<a id="microsofteditorsynonymsenabled"></a><a id="synonyms-are-provided-when-using-microsoft-editor-spell-checker"></a>[MicrosoftEditorSynonymsEnabled](microsoft-edge-browser-policies/MicrosoftEditorSynonymsEnabled.md)|Synonyms are provided when using Microsoft Editor spell checker|
|<a id="microsoftofficemenuenabled"></a><a id="allow-users-to-access-the-microsoft-office-menu-deprecated"></a>[MicrosoftOfficeMenuEnabled](microsoft-edge-browser-policies/MicrosoftOfficeMenuEnabled.md)|Allow users to access the Microsoft Office menu (deprecated)|
|<a id="microsoftrootstoreenabled"></a><a id="determines-whether-the-microsoft-root-store-and-built-in-certificate-verifier-will-be-used-to-verify-server-certificates-obsolete"></a>[MicrosoftRootStoreEnabled](microsoft-edge-browser-policies/MicrosoftRootStoreEnabled.md)|Determines whether the Microsoft Root Store and built-in certificate verifier will be used to verify server certificates (obsolete)|
|<a id="mousegestureenabled"></a><a id="mouse-gesture-enabled"></a>[MouseGestureEnabled](microsoft-edge-browser-policies/MouseGestureEnabled.md)|Mouse Gesture Enabled|
|<a id="mutationeventsenabled"></a><a id="enable-deprecatedremoved-mutation-events-obsolete"></a>[MutationEventsEnabled](microsoft-edge-browser-policies/MutationEventsEnabled.md)|Enable deprecated/removed Mutation Events (obsolete)|
|<a id="nativehostsexecutableslaunchdirectly"></a><a id="force-windows-executable-native-messaging-hosts-to-launch-directly"></a>[NativeHostsExecutablesLaunchDirectly](microsoft-edge-browser-policies/NativeHostsExecutablesLaunchDirectly.md)|Force Windows executable Native Messaging hosts to launch directly|
|<a id="nativewindowocclusionenabled"></a><a id="enable-native-window-occlusion-deprecated"></a>[NativeWindowOcclusionEnabled](microsoft-edge-browser-policies/NativeWindowOcclusionEnabled.md)|Enable Native Window Occlusion (deprecated)|
|<a id="navigationdelayforinitialsitelistdownloadtimeout"></a><a id="set-a-timeout-for-delay-of-tab-navigation-for-the-enterprise-mode-site-list"></a>[NavigationDelayForInitialSiteListDownloadTimeout](microsoft-edge-browser-policies/NavigationDelayForInitialSiteListDownloadTimeout.md)|Set a timeout for delay of tab navigation for the Enterprise Mode Site List|
|<a id="networkpredictionoptions"></a><a id="enable-network-prediction"></a>[NetworkPredictionOptions](microsoft-edge-browser-policies/NetworkPredictionOptions.md)|Enable network prediction|
|<a id="networkservicesandboxenabled"></a><a id="enable-the-network-service-sandbox"></a>[NetworkServiceSandboxEnabled](microsoft-edge-browser-policies/NetworkServiceSandboxEnabled.md)|Enable the network service sandbox|
|<a id="newbaseurlinheritancebehaviorallowed"></a><a id="allows-enabling-the-feature-newbaseurlinheritancebehavior-obsolete"></a>[NewBaseUrlInheritanceBehaviorAllowed](microsoft-edge-browser-policies/NewBaseUrlInheritanceBehaviorAllowed.md)|Allows enabling the feature NewBaseUrlInheritanceBehavior (obsolete)|
|<a id="newpdfreaderenabled"></a><a id="microsoft-edge-built-in-pdf-reader-powered-by-adobe-acrobat-enabled"></a>[NewPDFReaderEnabled](microsoft-edge-browser-policies/NewPDFReaderEnabled.md)|Microsoft Edge built-in PDF reader powered by Adobe Acrobat enabled|
|<a id="nonremovableprofileenabled"></a><a id="configure-whether-a-user-always-has-a-default-profile-automatically-signed-in-with-their-work-or-school-account"></a>[NonRemovableProfileEnabled](microsoft-edge-browser-policies/NonRemovableProfileEnabled.md)|Configure whether a user always has a default profile automatically signed in with their work or school account|
|<a id="organizationlogooverlayonappiconenabled"></a><a id="allow-your-organizations-logo-from-microsoft-entra-to-be-overlaid-on-the-microsoft-edge-app-icon-of-a-work-or-school-profile"></a>[OrganizationLogoOverlayOnAppIconEnabled](microsoft-edge-browser-policies/OrganizationLogoOverlayOnAppIconEnabled.md)|Allow your organization's logo from Microsoft Entra to be overlaid on the Microsoft Edge app icon of a work or school profile|
|<a id="organizationalbrandingonworkprofileuienabled"></a><a id="allow-the-use-of-your-organizations-branding-assets-from-microsoft-entra-on-the-profile-related-ui-of-a-work-or-school-profile"></a>[OrganizationalBrandingOnWorkProfileUIEnabled](microsoft-edge-browser-policies/OrganizationalBrandingOnWorkProfileUIEnabled.md)|Allow the use of your organization's branding assets from Microsoft Entra on the profile-related UI of a work or school profile|
|<a id="originagentclusterdefaultenabled"></a><a id="origin-keyed-agent-clustering-enabled-by-default"></a>[OriginAgentClusterDefaultEnabled](microsoft-edge-browser-policies/OriginAgentClusterDefaultEnabled.md)|Origin-keyed agent clustering enabled by default|
|<a id="outlookhubmenuenabled"></a><a id="allow-users-to-access-the-outlook-menu-obsolete"></a>[OutlookHubMenuEnabled](microsoft-edge-browser-policies/OutlookHubMenuEnabled.md)|Allow users to access the Outlook menu (obsolete)|
|<a id="overridesecurityrestrictionsoninsecureorigin"></a><a id="control-where-security-restrictions-on-insecure-origins-apply"></a>[OverrideSecurityRestrictionsOnInsecureOrigin](microsoft-edge-browser-policies/OverrideSecurityRestrictionsOnInsecureOrigin.md)|Control where security restrictions on insecure origins apply|
|<a id="pdfsecuremode"></a><a id="secure-mode-and-certificate-based-digital-signature-validation-in-native-pdf-reader"></a>[PDFSecureMode](microsoft-edge-browser-policies/PDFSecureMode.md)|Secure mode and Certificate-based Digital Signature validation in native PDF reader|
|<a id="pdfxfaenabled"></a><a id="xfa-support-in-native-pdf-reader-enabled"></a>[PDFXFAEnabled](microsoft-edge-browser-policies/PDFXFAEnabled.md)|XFA support in native PDF reader enabled|
|<a id="paymentmethodqueryenabled"></a><a id="allow-websites-to-query-for-available-payment-methods"></a>[PaymentMethodQueryEnabled](microsoft-edge-browser-policies/PaymentMethodQueryEnabled.md)|Allow websites to query for available payment methods|
|<a id="pdfvieweroutofprocessiframeenabled"></a><a id="use-out-of-process-iframe-pdf-viewer"></a>[PdfViewerOutOfProcessIframeEnabled](microsoft-edge-browser-policies/PdfViewerOutOfProcessIframeEnabled.md)|Use out-of-process iframe PDF Viewer|
|<a id="personalizationreportingenabled"></a><a id="allow-personalization-of-ads-microsoft-edge-search-news-and-other-microsoft-services-by-sending-browsing-history-favorites-and-collections-usage-and-other-browsing-data-to-microsoft"></a>[PersonalizationReportingEnabled](microsoft-edge-browser-policies/PersonalizationReportingEnabled.md)|Allow personalization of ads, Microsoft Edge, search, news and other Microsoft services by sending browsing history, favorites and collections, usage and other browsing data to Microsoft|
|<a id="personalizetopsitesincustomizesidebarenabled"></a><a id="personalize-my-top-sites-in-customize-sidebar-enabled-by-default"></a>[PersonalizeTopSitesInCustomizeSidebarEnabled](microsoft-edge-browser-policies/PersonalizeTopSitesInCustomizeSidebarEnabled.md)|Personalize my top sites in Customize Sidebar enabled by default|
|<a id="pictureinpictureoverlayenabled"></a><a id="enable-picture-in-picture-overlay-feature-on-supported-webpages-in-microsoft-edge"></a>[PictureInPictureOverlayEnabled](microsoft-edge-browser-policies/PictureInPictureOverlayEnabled.md)|Enable Picture in Picture overlay feature on supported webpages in Microsoft Edge|
|<a id="pinningwizardallowed"></a><a id="allow-pin-to-taskbar-wizard"></a>[PinningWizardAllowed](microsoft-edge-browser-policies/PinningWizardAllowed.md)|Allow Pin to taskbar wizard|
|<a id="postquantumkeyagreementenabled"></a><a id="enable-post-quantum-key-agreement-for-tls"></a>[PostQuantumKeyAgreementEnabled](microsoft-edge-browser-policies/PostQuantumKeyAgreementEnabled.md)|Enable post-quantum key agreement for TLS|
|<a id="proactiveauthenabled"></a><a id="enable-proactive-authentication-obsolete"></a>[ProactiveAuthEnabled](microsoft-edge-browser-policies/ProactiveAuthEnabled.md)|Enable Proactive Authentication (obsolete)|
|<a id="promotionaltabsenabled"></a><a id="enable-full-tab-promotional-content-deprecated"></a>[PromotionalTabsEnabled](microsoft-edge-browser-policies/PromotionalTabsEnabled.md)|Enable full-tab promotional content (deprecated)|
|<a id="promptfordownloadlocation"></a><a id="ask-where-to-save-downloaded-files"></a>[PromptForDownloadLocation](microsoft-edge-browser-policies/PromptForDownloadLocation.md)|Ask where to save downloaded files|
|<a id="promptonmultiplematchingcertificates"></a><a id="prompt-the-user-to-select-a-certificate-when-multiple-certificates-match"></a>[PromptOnMultipleMatchingCertificates](microsoft-edge-browser-policies/PromptOnMultipleMatchingCertificates.md)|Prompt the user to select a certificate when multiple certificates match|
|<a id="qrcodegeneratorenabled"></a><a id="enable-qr-code-generator"></a>[QRCodeGeneratorEnabled](microsoft-edge-browser-policies/QRCodeGeneratorEnabled.md)|Enable QR Code Generator|
|<a id="quicallowed"></a><a id="allow-quic-protocol"></a>[QuicAllowed](microsoft-edge-browser-policies/QuicAllowed.md)|Allow QUIC protocol|
|<a id="quicksearchshowminimenu"></a><a id="enables-microsoft-edge-mini-menu"></a>[QuickSearchShowMiniMenu](microsoft-edge-browser-policies/QuickSearchShowMiniMenu.md)|Enables Microsoft Edge mini menu|
|<a id="quickviewofficefilesenabled"></a><a id="manage-quickview-office-files-capability-in-microsoft-edge"></a>[QuickViewOfficeFilesEnabled](microsoft-edge-browser-policies/QuickViewOfficeFilesEnabled.md)|Manage QuickView Office files capability in Microsoft Edge|
|<a id="rsakeyusageforlocalanchorsenabled"></a><a id="check-rsa-key-usage-for-server-certificates-issued-by-local-trust-anchors-obsolete"></a>[RSAKeyUsageForLocalAnchorsEnabled](microsoft-edge-browser-policies/RSAKeyUsageForLocalAnchorsEnabled.md)|Check RSA key usage for server certificates issued by local trust anchors (obsolete)|
|<a id="readaloudenabled"></a><a id="enable-read-aloud-feature-in-microsoft-edge"></a>[ReadAloudEnabled](microsoft-edge-browser-policies/ReadAloudEnabled.md)|Enable Read Aloud feature in Microsoft Edge|
|<a id="redirectsitesfrominternetexplorerpreventbhoinstall"></a><a id="prevent-install-of-the-bho-to-redirect-incompatible-sites-from-internet-explorer-to-microsoft-edge"></a>[RedirectSitesFromInternetExplorerPreventBHOInstall](microsoft-edge-browser-policies/RedirectSitesFromInternetExplorerPreventBHOInstall.md)|Prevent install of the BHO to redirect incompatible sites from Internet Explorer to Microsoft Edge|
|<a id="redirectsitesfrominternetexplorerredirectmode"></a><a id="redirect-incompatible-sites-from-internet-explorer-to-microsoft-edge"></a>[RedirectSitesFromInternetExplorerRedirectMode](microsoft-edge-browser-policies/RedirectSitesFromInternetExplorerRedirectMode.md)|Redirect incompatible sites from Internet Explorer to Microsoft Edge|
|<a id="relatedmatchescloudserviceenabled"></a><a id="configure-related-matches-in-find-on-page-obsolete"></a>[RelatedMatchesCloudServiceEnabled](microsoft-edge-browser-policies/RelatedMatchesCloudServiceEnabled.md)|Configure Related Matches in Find on Page (obsolete)|
|<a id="relaunchnotification"></a><a id="notify-a-user-that-a-browser-restart-is-recommended-or-required-for-pending-updates"></a>[RelaunchNotification](microsoft-edge-browser-policies/RelaunchNotification.md)|Notify a user that a browser restart is recommended or required for pending updates|
|<a id="relaunchnotificationperiod"></a><a id="set-the-time-period-for-update-notifications"></a>[RelaunchNotificationPeriod](microsoft-edge-browser-policies/RelaunchNotificationPeriod.md)|Set the time period for update notifications|
|<a id="relaunchwindow"></a><a id="set-the-time-interval-for-relaunch"></a>[RelaunchWindow](microsoft-edge-browser-policies/RelaunchWindow.md)|Set the time interval for relaunch|
|<a id="remotedebuggingallowed"></a><a id="allow-remote-debugging"></a>[RemoteDebuggingAllowed](microsoft-edge-browser-policies/RemoteDebuggingAllowed.md)|Allow remote debugging|
|<a id="rendererappcontainerenabled"></a><a id="enable-renderer-in-app-container"></a>[RendererAppContainerEnabled](microsoft-edge-browser-policies/RendererAppContainerEnabled.md)|Enable renderer in app container|
|<a id="renderercodeintegrityenabled"></a><a id="enable-renderer-code-integrity-deprecated"></a>[RendererCodeIntegrityEnabled](microsoft-edge-browser-policies/RendererCodeIntegrityEnabled.md)|Enable renderer code integrity (deprecated)|
|<a id="requireonlinerevocationchecksforlocalanchors"></a><a id="specify-if-online-ocspcrl-checks-are-required-for-local-trust-anchors"></a>[RequireOnlineRevocationChecksForLocalAnchors](microsoft-edge-browser-policies/RequireOnlineRevocationChecksForLocalAnchors.md)|Specify if online OCSP/CRL checks are required for local trust anchors|
|<a id="resolvenavigationerrorsusewebservice"></a><a id="enable-resolution-of-navigation-errors-using-a-web-service"></a>[ResolveNavigationErrorsUseWebService](microsoft-edge-browser-policies/ResolveNavigationErrorsUseWebService.md)|Enable resolution of navigation errors using a web service|
|<a id="restorepdfview"></a><a id="restore-pdf-view"></a>[RestorePdfView](microsoft-edge-browser-policies/RestorePdfView.md)|Restore PDF view|
|<a id="restrictsignintopattern"></a><a id="restrict-which-accounts-can-be-used-to-sign-in-to-microsoft-edge"></a>[RestrictSigninToPattern](microsoft-edge-browser-policies/RestrictSigninToPattern.md)|Restrict which accounts can be used to sign in to Microsoft Edge|
|<a id="roamingprofilelocation"></a><a id="set-the-roaming-profile-directory"></a>[RoamingProfileLocation](microsoft-edge-browser-policies/RoamingProfileLocation.md)|Set the roaming profile directory|
|<a id="roamingprofilesupportenabled"></a><a id="enable-using-roaming-copies-for-microsoft-edge-profile-data"></a>[RoamingProfileSupportEnabled](microsoft-edge-browser-policies/RoamingProfileSupportEnabled.md)|Enable using roaming copies for Microsoft Edge profile data|
|<a id="runallflashinallowmode"></a><a id="extend-adobe-flash-content-setting-to-all-content-obsolete"></a>[RunAllFlashInAllowMode](microsoft-edge-browser-policies/RunAllFlashInAllowMode.md)|Extend Adobe Flash content setting to all content (obsolete)|
|<a id="sslerroroverrideallowed"></a><a id="allow-users-to-proceed-from-the-https-warning-page"></a>[SSLErrorOverrideAllowed](microsoft-edge-browser-policies/SSLErrorOverrideAllowed.md)|Allow users to proceed from the HTTPS warning page|
|<a id="sslerroroverrideallowedfororigins"></a><a id="allow-users-to-proceed-from-the-https-warning-page-for-specific-origins"></a>[SSLErrorOverrideAllowedForOrigins](microsoft-edge-browser-policies/SSLErrorOverrideAllowedForOrigins.md)|Allow users to proceed from the HTTPS warning page for specific origins|
|<a id="sslversionmin"></a><a id="minimum-tls-version-enabled-obsolete"></a>[SSLVersionMin](microsoft-edge-browser-policies/SSLVersionMin.md)|Minimum TLS version enabled (obsolete)|
|<a id="sandboxexternalprotocolblocked"></a><a id="allow-microsoft-edge-to-block-navigations-to-external-protocols-in-a-sandboxed-iframe"></a>[SandboxExternalProtocolBlocked](microsoft-edge-browser-policies/SandboxExternalProtocolBlocked.md)|Allow Microsoft Edge to block navigations to external protocols in a sandboxed iframe|
|<a id="savecookiesonexit"></a><a id="save-cookies-when-microsoft-edge-closes"></a>[SaveCookiesOnExit](microsoft-edge-browser-policies/SaveCookiesOnExit.md)|Save cookies when Microsoft Edge closes|
|<a id="savingbrowserhistorydisabled"></a><a id="disable-saving-browser-history"></a>[SavingBrowserHistoryDisabled](microsoft-edge-browser-policies/SavingBrowserHistoryDisabled.md)|Disable saving browser history|
|<a id="screencaptureallowed"></a><a id="allow-or-deny-screen-capture"></a>[ScreenCaptureAllowed](microsoft-edge-browser-policies/ScreenCaptureAllowed.md)|Allow or deny screen capture|
|<a id="screencapturewithoutgestureallowedfororigins"></a><a id="allow-screen-capture-without-prior-user-gesture"></a>[ScreenCaptureWithoutGestureAllowedForOrigins](microsoft-edge-browser-policies/ScreenCaptureWithoutGestureAllowedForOrigins.md)|Allow screen capture without prior user gesture|
|<a id="scrolltotextfragmentenabled"></a><a id="enable-scrolling-to-text-specified-in-url-fragments"></a>[ScrollToTextFragmentEnabled](microsoft-edge-browser-policies/ScrollToTextFragmentEnabled.md)|Enable scrolling to text specified in URL fragments|
|<a id="searchfiltersenabled"></a><a id="search-filters-enabled"></a>[SearchFiltersEnabled](microsoft-edge-browser-policies/SearchFiltersEnabled.md)|Search Filters Enabled|
|<a id="searchforimageenabled"></a><a id="search-for-image-enabled"></a>[SearchForImageEnabled](microsoft-edge-browser-policies/SearchForImageEnabled.md)|Search for image enabled|
|<a id="searchinsidebarenabled"></a><a id="search-in-sidebar-enabled"></a>[SearchInSidebarEnabled](microsoft-edge-browser-policies/SearchInSidebarEnabled.md)|Search in Sidebar enabled|
|<a id="searchsuggestenabled"></a><a id="enable-search-suggestions"></a>[SearchSuggestEnabled](microsoft-edge-browser-policies/SearchSuggestEnabled.md)|Enable search suggestions|
|<a id="searchbarallowed"></a><a id="enable-the-search-bar"></a>[SearchbarAllowed](microsoft-edge-browser-policies/SearchbarAllowed.md)|Enable the Search bar|
|<a id="searchbarisenabledonstartup"></a><a id="allow-the-search-bar-at-windows-startup"></a>[SearchbarIsEnabledOnStartup](microsoft-edge-browser-policies/SearchbarIsEnabledOnStartup.md)|Allow the Search bar at Windows startup|
|<a id="securitykeypermitattestation"></a><a id="websites-or-domains-that-dont-need-permission-to-use-direct-security-key-attestation"></a>[SecurityKeyPermitAttestation](microsoft-edge-browser-policies/SecurityKeyPermitAttestation.md)|Websites or domains that don't need permission to use direct Security Key attestation|
|<a id="selectparserrelaxationenabled"></a><a id="controls-whether-the-new-html-parser-behavior-for-the-select-element-is-enabled"></a>[SelectParserRelaxationEnabled](microsoft-edge-browser-policies/SelectParserRelaxationEnabled.md)|Controls whether the new HTML parser behavior for the &lt;select&gt; element is enabled|
|<a id="sendintranettointernetexplorer"></a><a id="send-all-intranet-sites-to-internet-explorer"></a>[SendIntranetToInternetExplorer](microsoft-edge-browser-policies/SendIntranetToInternetExplorer.md)|Send all intranet sites to Internet Explorer|
|<a id="sendmouseeventsdisabledformcontrolsenabled"></a><a id="control-the-new-behavior-for-event-dispatching-on-disabled-form-controls-obsolete"></a>[SendMouseEventsDisabledFormControlsEnabled](microsoft-edge-browser-policies/SendMouseEventsDisabledFormControlsEnabled.md)|Control the new behavior for event dispatching on disabled form controls (obsolete)|
|<a id="sendsiteinfotoimproveservices"></a><a id="send-site-information-to-improve-microsoft-services-obsolete"></a>[SendSiteInfoToImproveServices](microsoft-edge-browser-policies/SendSiteInfoToImproveServices.md)|Send site information to improve Microsoft services (obsolete)|
|<a id="sensorsallowedforurls"></a><a id="allow-access-to-sensors-on-specific-sites"></a>[SensorsAllowedForUrls](microsoft-edge-browser-policies/SensorsAllowedForUrls.md)|Allow access to sensors on specific sites|
|<a id="sensorsblockedforurls"></a><a id="block-access-to-sensors-on-specific-sites"></a>[SensorsBlockedForUrls](microsoft-edge-browser-policies/SensorsBlockedForUrls.md)|Block access to sensors on specific sites|
|<a id="serialaskforurls"></a><a id="allow-the-serial-api-on-specific-sites"></a>[SerialAskForUrls](microsoft-edge-browser-policies/SerialAskForUrls.md)|Allow the Serial API on specific sites|
|<a id="serialblockedforurls"></a><a id="block-the-serial-api-on-specific-sites"></a>[SerialBlockedForUrls](microsoft-edge-browser-policies/SerialBlockedForUrls.md)|Block the Serial API on specific sites|
|<a id="serviceworkertocontrolsrcdociframeenabled"></a><a id="allow-serviceworker-to-control-srcdoc-iframes"></a>[ServiceWorkerToControlSrcdocIframeEnabled](microsoft-edge-browser-policies/ServiceWorkerToControlSrcdocIframeEnabled.md)|Allow ServiceWorker to control srcdoc iframes|
|<a id="settimeoutwithout1msclampenabled"></a><a id="control-javascript-settimeout-function-minimum-timeout-obsolete"></a>[SetTimeoutWithout1MsClampEnabled](microsoft-edge-browser-policies/SetTimeoutWithout1MsClampEnabled.md)|Control Javascript setTimeout() function minimum timeout (obsolete)|
|<a id="shadowstackcrashrollbackbehavior"></a><a id="configure-shadowstack-crash-rollback-behavior-obsolete"></a>[ShadowStackCrashRollbackBehavior](microsoft-edge-browser-policies/ShadowStackCrashRollbackBehavior.md)|Configure ShadowStack crash rollback behavior (obsolete)|
|<a id="sharedarraybufferunrestrictedaccessallowed"></a><a id="specifies-whether-sharedarraybuffers-can-be-used-in-a-non-cross-origin-isolated-context"></a>[SharedArrayBufferUnrestrictedAccessAllowed](microsoft-edge-browser-policies/SharedArrayBufferUnrestrictedAccessAllowed.md)|Specifies whether SharedArrayBuffers can be used in a non cross-origin-isolated context|
|<a id="sharedlinksenabled"></a><a id="show-links-shared-from-microsoft-365-apps-in-history"></a>[SharedLinksEnabled](microsoft-edge-browser-policies/SharedLinksEnabled.md)|Show links shared from Microsoft 365 apps in History|
|<a id="sharedworkerbloburlfixenabled"></a><a id="make-sharedworker-blob-url-behavior-aligned-with-the-specification"></a>[SharedWorkerBlobURLFixEnabled](microsoft-edge-browser-policies/SharedWorkerBlobURLFixEnabled.md)|Make SharedWorker blob URL behavior aligned with the specification|
|<a id="showacrobatsubscriptionbutton"></a><a id="shows-button-on-native-pdf-viewer-in-microsoft-edge-that-allows-users-to-sign-up-for-adobe-acrobat-subscription"></a>[ShowAcrobatSubscriptionButton](microsoft-edge-browser-policies/ShowAcrobatSubscriptionButton.md)|Shows button on native PDF viewer in Microsoft Edge that allows users to sign up for Adobe Acrobat subscription|
|<a id="showdownloadstoolbarbutton"></a><a id="show-downloads-button-on-the-toolbar"></a>[ShowDownloadsToolbarButton](microsoft-edge-browser-policies/ShowDownloadsToolbarButton.md)|Show Downloads button on the toolbar|
|<a id="showhistorythumbnails"></a><a id="show-thumbnail-images-for-browsing-history"></a>[ShowHistoryThumbnails](microsoft-edge-browser-policies/ShowHistoryThumbnails.md)|Show thumbnail images for browsing history|
|<a id="showmicrosoftrewards"></a><a id="show-microsoft-rewards-experiences"></a>[ShowMicrosoftRewards](microsoft-edge-browser-policies/ShowMicrosoftRewards.md)|Show Microsoft Rewards experiences|
|<a id="showofficeshortcutinfavoritesbar"></a><a id="show-microsoft-office-shortcut-in-favorites-bar-deprecated"></a>[ShowOfficeShortcutInFavoritesBar](microsoft-edge-browser-policies/ShowOfficeShortcutInFavoritesBar.md)|Show Microsoft Office shortcut in favorites bar (deprecated)|
|<a id="showrecommendationsenabled"></a><a id="allow-feature-recommendations-and-browser-assistance-notifications-from-microsoft-edge"></a>[ShowRecommendationsEnabled](microsoft-edge-browser-policies/ShowRecommendationsEnabled.md)|Allow feature recommendations and browser assistance notifications from Microsoft Edge|
|<a id="signedhttpexchangeenabled"></a><a id="enable-signed-http-exchange-sxg-support"></a>[SignedHTTPExchangeEnabled](microsoft-edge-browser-policies/SignedHTTPExchangeEnabled.md)|Enable Signed HTTP Exchange (SXG) support|
|<a id="siteperprocess"></a><a id="enable-site-isolation-for-every-site"></a>[SitePerProcess](microsoft-edge-browser-policies/SitePerProcess.md)|Enable site isolation for every site|
|<a id="sitesafetyservicesenabled"></a><a id="allow-users-to-configure-site-safety-services-obsolete"></a>[SiteSafetyServicesEnabled](microsoft-edge-browser-policies/SiteSafetyServicesEnabled.md)|Allow users to configure Site safety services (obsolete)|
|<a id="smartactionsblocklist"></a><a id="block-smart-actions-for-a-list-of-services"></a>[SmartActionsBlockList](microsoft-edge-browser-policies/SmartActionsBlockList.md)|Block smart actions for a list of services|
|<a id="speechrecognitionenabled"></a><a id="configure-speech-recognition"></a>[SpeechRecognitionEnabled](microsoft-edge-browser-policies/SpeechRecognitionEnabled.md)|Configure Speech Recognition|
|<a id="spellcheckenabled"></a><a id="enable-spellcheck"></a>[SpellcheckEnabled](microsoft-edge-browser-policies/SpellcheckEnabled.md)|Enable spellcheck|
|<a id="spellchecklanguage"></a><a id="enable-specific-spellcheck-languages"></a>[SpellcheckLanguage](microsoft-edge-browser-policies/SpellcheckLanguage.md)|Enable specific spellcheck languages|
|<a id="spellchecklanguageblocklist"></a><a id="force-disable-spellcheck-languages"></a>[SpellcheckLanguageBlocklist](microsoft-edge-browser-policies/SpellcheckLanguageBlocklist.md)|Force disable spellcheck languages|
|<a id="splitscreenenabled"></a><a id="enable-split-screen-feature-in-microsoft-edge"></a>[SplitScreenEnabled](microsoft-edge-browser-policies/SplitScreenEnabled.md)|Enable split screen feature in Microsoft Edge|
|<a id="standalonehubssidebarenabled"></a><a id="standalone-sidebar-enabled"></a>[StandaloneHubsSidebarEnabled](microsoft-edge-browser-policies/StandaloneHubsSidebarEnabled.md)|Standalone Sidebar Enabled|
|<a id="strictermixedcontenttreatmentenabled"></a><a id="enable-stricter-treatment-for-mixed-content-obsolete"></a>[StricterMixedContentTreatmentEnabled](microsoft-edge-browser-policies/StricterMixedContentTreatmentEnabled.md)|Enable stricter treatment for mixed content (obsolete)|
|<a id="superdragdropenabled"></a><a id="super-drag-drop-enabled"></a>[SuperDragDropEnabled](microsoft-edge-browser-policies/SuperDragDropEnabled.md)|Super Drag Drop Enabled|
|<a id="suppressunsupportedoswarning"></a><a id="suppress-the-unsupported-os-warning"></a>[SuppressUnsupportedOSWarning](microsoft-edge-browser-policies/SuppressUnsupportedOSWarning.md)|Suppress the unsupported OS warning|
|<a id="syncdisabled"></a><a id="disable-synchronization-of-data-using-microsoft-sync-services"></a>[SyncDisabled](microsoft-edge-browser-policies/SyncDisabled.md)|Disable synchronization of data using Microsoft sync services|
|<a id="synctypeslistdisabled"></a><a id="configure-the-list-of-types-that-are-excluded-from-synchronization"></a>[SyncTypesListDisabled](microsoft-edge-browser-policies/SyncTypesListDisabled.md)|Configure the list of types that are excluded from synchronization|
|<a id="tls13hardeningforlocalanchorsenabled"></a><a id="enable-a-tls-13-security-feature-for-local-trust-anchors-obsolete"></a>[TLS13HardeningForLocalAnchorsEnabled](microsoft-edge-browser-policies/TLS13HardeningForLocalAnchorsEnabled.md)|Enable a TLS 1.3 security feature for local trust anchors (obsolete)|
|<a id="tlsciphersuitedenylist"></a><a id="specify-the-tls-cipher-suites-to-disable"></a>[TLSCipherSuiteDenyList](microsoft-edge-browser-policies/TLSCipherSuiteDenyList.md)|Specify the TLS cipher suites to disable|
|<a id="tabfreezingenabled"></a><a id="allow-freezing-of-background-tabs-obsolete"></a>[TabFreezingEnabled](microsoft-edge-browser-policies/TabFreezingEnabled.md)|Allow freezing of background tabs (obsolete)|
|<a id="tabservicesenabled"></a><a id="enable-tab-organization-suggestions"></a>[TabServicesEnabled](microsoft-edge-browser-policies/TabServicesEnabled.md)|Enable tab organization suggestions|
|<a id="targetblankimpliesnoopener"></a><a id="do-not-set-windowopener-for-links-targeting-blank-obsolete"></a>[TargetBlankImpliesNoOpener](microsoft-edge-browser-policies/TargetBlankImpliesNoOpener.md)|Do not set window.opener for links targeting _blank (obsolete)|
|<a id="taskmanagerendprocessenabled"></a><a id="enable-ending-processes-in-the-browser-task-manager"></a>[TaskManagerEndProcessEnabled](microsoft-edge-browser-policies/TaskManagerEndProcessEnabled.md)|Enable ending processes in the Browser task manager|
|<a id="textpredictionenabled"></a><a id="text-prediction-enabled-by-default"></a>[TextPredictionEnabled](microsoft-edge-browser-policies/TextPredictionEnabled.md)|Text prediction enabled by default|
|<a id="throttlenonvisiblecrossoriginiframesallowed"></a><a id="allows-enabling-throttling-of-non-visible-cross-origin-iframes-obsolete"></a>[ThrottleNonVisibleCrossOriginIframesAllowed](microsoft-edge-browser-policies/ThrottleNonVisibleCrossOriginIframesAllowed.md)|Allows enabling throttling of non-visible, cross-origin iframes (obsolete)|
|<a id="totalmemorylimitmb"></a><a id="set-limit-on-megabytes-of-memory-a-single-microsoft-edge-instance-can-use"></a>[TotalMemoryLimitMb](microsoft-edge-browser-policies/TotalMemoryLimitMb.md)|Set limit on megabytes of memory a single Microsoft Edge instance can use|
|<a id="trackingprevention"></a><a id="block-tracking-of-users-web-browsing-activity"></a>[TrackingPrevention](microsoft-edge-browser-policies/TrackingPrevention.md)|Block tracking of users' web-browsing activity|
|<a id="translateenabled"></a><a id="enable-translate"></a>[TranslateEnabled](microsoft-edge-browser-policies/TranslateEnabled.md)|Enable Translate|
|<a id="travelassistanceenabled"></a><a id="enable-travel-assistance-obsolete"></a>[TravelAssistanceEnabled](microsoft-edge-browser-policies/TravelAssistanceEnabled.md)|Enable travel assistance (obsolete)|
|<a id="tripledesenabled"></a><a id="enable-3des-cipher-suites-in-tls-obsolete"></a>[TripleDESEnabled](microsoft-edge-browser-policies/TripleDESEnabled.md)|Enable 3DES cipher suites in TLS (obsolete)|
|<a id="u2fsecuritykeyapienabled"></a><a id="allow-using-the-deprecated-u2f-security-key-api-obsolete"></a>[U2fSecurityKeyApiEnabled](microsoft-edge-browser-policies/U2fSecurityKeyApiEnabled.md)|Allow using the deprecated U2F Security Key API (obsolete)|
|<a id="urlallowlist"></a><a id="define-a-list-of-allowed-urls"></a>[URLAllowlist](microsoft-edge-browser-policies/URLAllowlist.md)|Define a list of allowed URLs|
|<a id="urlblocklist"></a><a id="block-access-to-a-list-of-urls"></a>[URLBlocklist](microsoft-edge-browser-policies/URLBlocklist.md)|Block access to a list of URLs|
|<a id="unthrottlednestedtimeoutenabled"></a><a id="javascript-settimeout-will-not-be-clamped-until-a-higher-nesting-threshold-is-set-deprecated"></a>[UnthrottledNestedTimeoutEnabled](microsoft-edge-browser-policies/UnthrottledNestedTimeoutEnabled.md)|JavaScript setTimeout will not be clamped until a higher nesting threshold is set (deprecated)|
|<a id="updatepolicyoverride"></a><a id="specifies-how-microsoft-edge-update-handles-available-updates-from-microsoft-edge"></a>[UpdatePolicyOverride](microsoft-edge-browser-policies/UpdatePolicyOverride.md)|Specifies how Microsoft Edge Update handles available updates from Microsoft Edge|
|<a id="uploadfromphoneenabled"></a><a id="enable-upload-files-from-mobile-in-microsoft-edge-desktop"></a>[UploadFromPhoneEnabled](microsoft-edge-browser-policies/UploadFromPhoneEnabled.md)|Enable upload files from mobile in Microsoft Edge desktop|
|<a id="urldiagnosticdataenabled"></a><a id="url-reporting-in-edge-diagnostic-data-enabled"></a>[UrlDiagnosticDataEnabled](microsoft-edge-browser-policies/UrlDiagnosticDataEnabled.md)|URL reporting in Edge diagnostic data enabled|
|<a id="useragentclienthintsenabled"></a><a id="enable-the-user-agent-client-hints-feature-obsolete"></a>[UserAgentClientHintsEnabled](microsoft-edge-browser-policies/UserAgentClientHintsEnabled.md)|Enable the User-Agent Client Hints feature (obsolete)|
|<a id="useragentclienthintsgreaseupdateenabled"></a><a id="control-the-user-agent-client-hints-grease-update-feature-obsolete"></a>[UserAgentClientHintsGREASEUpdateEnabled](microsoft-edge-browser-policies/UserAgentClientHintsGREASEUpdateEnabled.md)|Control the User-Agent Client Hints GREASE Update feature (obsolete)|
|<a id="useragentreduction"></a><a id="enable-or-disable-the-user-agent-reduction"></a>[UserAgentReduction](microsoft-edge-browser-policies/UserAgentReduction.md)|Enable or disable the User-Agent Reduction|
|<a id="userdatadir"></a><a id="set-the-user-data-directory"></a>[UserDataDir](microsoft-edge-browser-policies/UserDataDir.md)|Set the user data directory|
|<a id="userdatasnapshotretentionlimit"></a><a id="limits-the-number-of-user-data-snapshots-retained-for-use-in-case-of-emergency-rollback"></a>[UserDataSnapshotRetentionLimit](microsoft-edge-browser-policies/UserDataSnapshotRetentionLimit.md)|Limits the number of user data snapshots retained for use in case of emergency rollback|
|<a id="userfeedbackallowed"></a><a id="allow-user-feedback"></a>[UserFeedbackAllowed](microsoft-edge-browser-policies/UserFeedbackAllowed.md)|Allow user feedback|
|<a id="verticaltabsallowed"></a><a id="configures-availability-of-a-vertical-layout-for-tabs-on-the-side-of-the-browser"></a>[VerticalTabsAllowed](microsoft-edge-browser-policies/VerticalTabsAllowed.md)|Configures availability of a vertical layout for tabs on the side of the browser|
|<a id="videocaptureallowed"></a><a id="allow-or-block-video-capture"></a>[VideoCaptureAllowed](microsoft-edge-browser-policies/VideoCaptureAllowed.md)|Allow or block video capture|
|<a id="videocaptureallowedurls"></a><a id="sites-that-can-access-video-capture-devices-without-requesting-permission"></a>[VideoCaptureAllowedUrls](microsoft-edge-browser-policies/VideoCaptureAllowedUrls.md)|Sites that can access video capture devices without requesting permission|
|<a id="visualsearchenabled"></a><a id="visual-search-enabled"></a>[VisualSearchEnabled](microsoft-edge-browser-policies/VisualSearchEnabled.md)|Visual search enabled|
|<a id="wpadquickcheckenabled"></a><a id="set-wpad-optimization"></a>[WPADQuickCheckEnabled](microsoft-edge-browser-policies/WPADQuickCheckEnabled.md)|Set WPAD optimization|
|<a id="walletdonationenabled"></a><a id="wallet-donation-enabled"></a>[WalletDonationEnabled](microsoft-edge-browser-policies/WalletDonationEnabled.md)|Wallet Donation Enabled|
|<a id="webappinstallforcelist"></a><a id="configure-list-of-force-installed-web-apps"></a>[WebAppInstallForceList](microsoft-edge-browser-policies/WebAppInstallForceList.md)|Configure list of force-installed Web Apps|
|<a id="webappsettings"></a><a id="web-app-management-settings"></a>[WebAppSettings](microsoft-edge-browser-policies/WebAppSettings.md)|Web App management settings|
|<a id="webaudiooutputbufferingenabled"></a><a id="enable-adaptive-buffering-for-web-audio"></a>[WebAudioOutputBufferingEnabled](microsoft-edge-browser-policies/WebAudioOutputBufferingEnabled.md)|Enable adaptive buffering for Web Audio|
|<a id="webcaptureenabled"></a><a id="enable-the-screenshot-previously-named-web-capture-feature-in-microsoft-edge"></a>[WebCaptureEnabled](microsoft-edge-browser-policies/WebCaptureEnabled.md)|Enable the Screenshot (previously named Web Capture) feature in Microsoft Edge|
|<a id="webcomponentsv0enabled"></a><a id="re-enable-web-components-v0-api-until-m84-obsolete"></a>[WebComponentsV0Enabled](microsoft-edge-browser-policies/WebComponentsV0Enabled.md)|Re-enable Web Components v0 API until M84 (obsolete)|
|<a id="webcontentfilteringblockedcategories"></a><a id="configure-web-content-filtering"></a>[WebContentFilteringBlockedCategories](microsoft-edge-browser-policies/WebContentFilteringBlockedCategories.md)|Configure Web Content Filtering|
|<a id="webdriveroverridesincompatiblepolicies"></a><a id="allow-webdriver-to-override-incompatible-policies-obsolete"></a>[WebDriverOverridesIncompatiblePolicies](microsoft-edge-browser-policies/WebDriverOverridesIncompatiblePolicies.md)|Allow WebDriver to Override Incompatible Policies (obsolete)|
|<a id="webrtcallowlegacytlsprotocols"></a><a id="allow-legacy-tlsdtls-downgrade-in-webrtc-obsolete"></a>[WebRtcAllowLegacyTLSProtocols](microsoft-edge-browser-policies/WebRtcAllowLegacyTLSProtocols.md)|Allow legacy TLS/DTLS downgrade in WebRTC (obsolete)|
|<a id="webrtclocalipsallowedurls"></a><a id="manage-exposure-of-local-ip-addressess-by-webrtc"></a>[WebRtcLocalIpsAllowedUrls](microsoft-edge-browser-policies/WebRtcLocalIpsAllowedUrls.md)|Manage exposure of local IP addressess by WebRTC|
|<a id="webrtcrespectosroutingtableenabled"></a><a id="enable-support-for-windows-os-routing-table-rules-when-making-peer-to-peer-connections-via-webrtc"></a>[WebRtcRespectOsRoutingTableEnabled](microsoft-edge-browser-policies/WebRtcRespectOsRoutingTableEnabled.md)|Enable support for Windows OS routing table rules when making peer to peer connections via WebRTC|
|<a id="webrtcudpportrange"></a><a id="restrict-the-range-of-local-udp-ports-used-by-webrtc"></a>[WebRtcUdpPortRange](microsoft-edge-browser-policies/WebRtcUdpPortRange.md)|Restrict the range of local UDP ports used by WebRTC|
|<a id="websqlaccess"></a><a id="force-websql-to-be-enabled-obsolete"></a>[WebSQLAccess](microsoft-edge-browser-policies/WebSQLAccess.md)|Force WebSQL to be enabled (obsolete)|
|<a id="websqlinthirdpartycontextenabled"></a><a id="force-websql-in-third-party-contexts-to-be-re-enabled-obsolete"></a>[WebSQLInThirdPartyContextEnabled](microsoft-edge-browser-policies/WebSQLInThirdPartyContextEnabled.md)|Force WebSQL in third-party contexts to be re-enabled (obsolete)|
|<a id="websqlnonsecurecontextenabled"></a><a id="force-websql-in-non-secure-contexts-to-be-enabled-obsolete"></a>[WebSQLNonSecureContextEnabled](microsoft-edge-browser-policies/WebSQLNonSecureContextEnabled.md)|Force WebSQL in non-secure contexts to be enabled (obsolete)|
|<a id="webselectenabled"></a><a id="web-select-enabled-obsolete"></a>[WebSelectEnabled](microsoft-edge-browser-policies/WebSelectEnabled.md)|Web Select Enabled (obsolete)|
|<a id="webwidgetallowed"></a><a id="enable-the-search-bar-deprecated"></a>[WebWidgetAllowed](microsoft-edge-browser-policies/WebWidgetAllowed.md)|Enable the Search bar (deprecated)|
|<a id="webwidgetisenabledonstartup"></a><a id="allow-the-search-bar-at-windows-startup-obsolete"></a>[WebWidgetIsEnabledOnStartup](microsoft-edge-browser-policies/WebWidgetIsEnabledOnStartup.md)|Allow the Search bar at Windows startup (obsolete)|
|<a id="winhttpproxyresolverenabled"></a><a id="use-windows-proxy-resolver"></a>[WinHttpProxyResolverEnabled](microsoft-edge-browser-policies/WinHttpProxyResolverEnabled.md)|Use Windows proxy resolver|
|<a id="windowocclusionenabled"></a><a id="enable-window-occlusion"></a>[WindowOcclusionEnabled](microsoft-edge-browser-policies/WindowOcclusionEnabled.md)|Enable Window Occlusion|

## See also

- [Configuring Microsoft Edge](configure-microsoft-edge.md)
- [Microsoft Edge Enterprise landing page](https://aka.ms/EdgeEnterprise)
- [Microsoft Security Baselines Blog](https://techcommunity.microsoft.com/t5/microsoft-security-baselines/bg-p/Microsoft-Security-Baselines)

