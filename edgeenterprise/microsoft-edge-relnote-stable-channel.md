---
title: "Microsoft Edge release notes for Stable Channel"
ms.author: archandr
author: vmliramichael
manager: likuba
ms.date: 07/1/2025
audience: ITPro
ms.topic: release-notes
ms.service: microsoft-edge
ms.localizationpriority: high
ms.collection: M365-modern-desktop
description: "Microsoft Edge release note for Stable Channel"
---

# Release notes for Microsoft Edge Stable Channel

These release notes provide information about new features and nonsecurity updates that are included in the Microsoft Edge Stable Channel.

- All the security updates are listed in [Release notes for Microsoft Edge Security Updates](./microsoft-edge-relnotes-security.md).
- Archived release notes for Microsoft Edge Stable Channel are located in [Archived release notes for Microsoft Edge Stable Channel](./microsoft-edge-relnote-archive-stable-channel.md).

 To understand Microsoft Edge channels, see the [Overview of the Microsoft Edge channels](./microsoft-edge-channels.md).

> [!NOTE]
> For the Stable Channel, updates roll out progressively over one or more days. To learn more, see [Progressive rollouts for Microsoft Edge updates](./microsoft-edge-update-progressive-rollout.md).
>
> Microsoft Edge Web Platform constantly evolves to improve user experience, security, and privacy. To learn more, see [Site compatibility-impacting changes coming to Microsoft Edge](/microsoft-edge/web-platform/site-impacting-changes).

## Version 139.0.3405.86: August 7, 2025

Fixed various bugs and performance issues for Stable Channel

Stable channel security updates are listed [here](/deployedge/microsoft-edge-relnotes-security#August-7-2025).

### Fixes

- Fixed an issue where MIP-protected PDF files from different sovereign cloud environments (including GCCH) failed to open and instead displayed the error message: “Need permissions. Contact the owner of the file to give you permissions.”

- Fixed an issue which affected IE mode, including errors when displaying PDF files, running Java applets, and showing the Information Bar in IE mode.  
 
### Improved reliability

- Fixed a browser crash that occurred on first launch when the [BrowserSignin](/deployedge/microsoft-edge-browser-policies/browsersignin) policy was enabled and configured to "Force (2) = Force users to sign-in to use the browser (all profiles)."
 
### Feature updates

- **Open external links in another profile when recommended by external applications**.  When Microsoft Edge is set as the default browser to open external links from applications, Microsoft Edge must determine which profile to open the links. Users can control which profile to use through the “Default profile for external links” setting. Applications such as Microsoft Teams or Outlook can also recommend a profile for the links. Currently, the user setting is prioritized over application recommendations. With this feature, the application recommended profile is given priority, instead of the profile selected in the setting. Admins can control the availability of the feature using the [EdgeOpenExternalLinksWithAppSpecifiedProfile](/deployedge/microsoft-edge-browser-policies/edgeopenexternallinkswithappspecifiedprofile) policy. **Note:** This is a controlled feature rollout. If you don't see this feature, check back as we continue our rollout.

- **Changes to Wallet in Microsoft Edge**. Wallet is being phased out to support a streamlined experience within Microsoft Edge. This affects the Wallet feature in Settings and the Mini Wallet found by clicking the profile icon in the top banner.  Users will be directed to the new Passwords, Payment, and Personal Information management experience in Settings. Also, a new Password management experience will be available in Settings. For more information, see Changes to Wallet in [Microsoft Edge](https://support.microsoft.com/en-us/microsoft-edge/changes-to-wallet-in-microsoft-edge-bc52418a-4d35-444e-845c-e09df6033b81).  **Note:** This is a controlled feature rollout. If you don't see this feature, check back as we continue our rollout.
 
- **Introducing a new policy that can enable/disable Microsoft 365 Copilot Chat in Edge for Business from showing in the toolbar**. Edge for Business now has a dedicated policy, [Microsoft365CopilotChatIconEnabled](/deployedge/microsoft-edge-browser-policies/microsoft365copilotchaticonenabled), to enable and disable **Copilot in Edge from showing in the Edge toolbar. When both this policy and [HubsSidebarEnabled](/deployedge/microsoft-edge-browser-policies/hubssidebarenabled) are configured, this policy takes precedence in determining whether Copilot appears in the toolbar. If this policy isn't configured and [HubsSidebarEnabled](/deployedge/microsoft-edge-browser-policies/hubssidebarenabled) is disabled, Copilot will remain hidden. In a future release, this policy is the sole control for managing Copilot's visibility in the toolbar.
 
- **Real-time notifications for compromised passwords**. Microsoft Edge is integrating an in-context password breach notification system. This feature proactively informs users if their saved login credentials have been compromised in known data breaches, enabling them to take immediate action to secure their accounts.  Admins can control availability to this feature using the [PasswordMonitorAllowed](/deployedge/microsoft-edge-browser-policies/passwordmonitorallowed) policy.  **Note:** This is a controlled feature rollout. If you don't see this feature, check back as we continue our rollout.
 
- **Edge Settings Improvements**.  Edge Settings is migrating to WebUI2 to boost page responsiveness and introducing a series of minor visual and content upgrades to improve overall usability and utility. This includes optimizing for concise wording of individual settings, simplifying the number of pages and reorganizing content, and creating a cohesive user interface.
 
- **New Autofill Personal Information Settings Configuration**.  A web form field collection consent toggle will be available in Autofill settings (edge://settings/autofill/personalInfo). This will allow users to consent to Microsoft Edge collecting web form field labels (e.g., "First Name," "Email") to improve Autofill suggestion accuracy.  Only field labels are collected and not user-entered data.  The web field labels are stored securely per Microsoft's [privacy standards](https://www.microsoft.com/en-us/privacy/privacystatement).

   This new setting is manageable via existing policies in Autofill (e.g., [AutofillAddressEnabled](/deployedge/microsoft-edge-browser-policies/autofilladdressenabled)), [EdgeAutofillMlEnabled](/deployedge/microsoft-edge-browser-policies/edgeautofillmlenabled). [AutofillAddressEnabled](/deployedge/microsoft-edge-browser-policies/autofilladdressenabled)is the parent setting for[EdgeAutofillMlEnabled](/deployedge/microsoft-edge-browser-policies/edgeautofillmlenabled). The [EdgeAutofillMlEnabled](/deployedge/microsoft-edge-browser-policies/edgeautofillmlenabled) policy is the parent of this new setting, thus turning off the [EdgeAutofillMlEnabled](/deployedge/microsoft-edge-browser-policies/edgeautofillmlenabled) policy will turn off this setting. 

- **Web AI APIs for prompt and writing assistance**. Microsoft Edge now implements the [Writing Assistance APIs](https://learn.microsoft.com/en-us/microsoft-edge/web-platform/writing-assistance-apis) and the [Prompt API](https://learn.microsoft.com/en-us/microsoft-edge/web-platform/prompt-api) (for Edge extensions) with a local language model, [Phi-4-mini](https://huggingface.co/microsoft/Phi-4-mini-instruct), that is built into the browser. These easy-to-use JavaScript APIs are made available via Edge flags (set to Enabled, by default only for the Summarizer and Prompt API for extensions) so that sites and extensions can apply AI capabilities on the web. The small language model is downloaded as the first time any of these APIs is used and later shared across all domains, serving local AI use-cases with reduced cost, network independence, and increased privacy (since data input to the model doesn't leave the user’s device). Admins can control the availability of these APIs via the [GenAILocalFoundationalModelSettings](/deployedge/microsoft-edge-browser-policies/genailocalfoundationalmodelsettings) policy. These APIs are currently not implemented in China. Read the announcement [here](https://blogs.windows.com/msedgedev/2025/05/19/introducing-the-prompt-and-writing-assistance-apis/), and feel free to provide [feedback](https://github.com/MicrosoftEdge/MSEdgeExplainers/issues/1012).
 
- **Enhancements to Performance and Secure network**.  **Browser essentials** is now separated into two distinct experiences (**Performance and Secure Network**) - both available from the **Settings and more** menu (“…” on the menu bar).  
 
- **Reset Microsoft Edge enterprise sync**.  For users having problems syncing browsing data across other signed-in devices, they can reset sync data from the Microsoft servers via Edge Settings edge://settings/profiles/sync/reset. This option should only be used if the sync data is available on one of the user's devices or if they want to delete all sync data from the servers.  **Note:** In Microsoft Edge 139, reset sync is enabled for users encountering a "No permissions" MIP error and in Microsoft Edge 140, reset sync is enabled for users encountering a "Service disabled" MIP error.  
 
- **Update to Microsoft AutoUpdate policy**. The [MAUEnabled](/deployedge/microsoft-edge-browser-policies/mauenabled) policy allowed admins to continue using Microsoft AutoUpdate on macOS. Since Microsoft Edge now uses EdgeUpdate, the [MAUEnabled](/deployedge/microsoft-edge-browser-policies/mauenabled) policy is planned to be obsoleted in Microsoft Edge version 140. 
 
### Policy updates

#### New policies

- [EdgeOpenExternalLinksWithAppSpecifiedProfile](/deployedge/microsoft-edge-browser-policies/edgeopenexternallinkswithappspecifiedprofile) - Prioritize App specified profile to open external links
- [EnableUnsafeSwiftShader](/deployedge/microsoft-edge-browser-policies/enableunsafeswiftshader) - Allow software WebGL fallback using SwiftShader
- [MandatoryExtensionsForInPrivateNavigation](/deployedge/microsoft-edge-browser-policies/mandatoryextensionsforinprivatenavigation) - Specify extensions users must allow in order to navigate using InPrivate mode
- [Microsoft365CopilotChatIconEnabled](/deployedge/microsoft-edge-browser-policies/microsoft365copilotchaticonenabled) - Control whether Microsoft 365 Copilot Chat shows in the Microsoft Edge for Business toolbar
- [OnSecurityEventEnterpriseConnector](/deployedge/microsoft-edge-browser-policies/onsecurityevententerpriseconnector) - Configuration policy for Microsoft Edge for Business Reporting Connectors

### Obsoleted policies

- [KeyboardFocusableScrollersEnabled](/deployedge/microsoft-edge-browser-policies/keyboardfocusablescrollersenabled) - Enable keyboard focusable scrollers (obsolete)
- [SelectParserRelaxationEnabled](/deployedge/microsoft-edge-browser-policies/selectparserrelaxationenabled) - Controls whether the new HTML parser behavior for the `SELECT` element is enabled (obsolete)

>[!NOTE]
>For the latest web platform features and updates, see [Microsoft Edge 139 web platform release notes (August 2025)](/microsoft-edge/web-platform/release-notes/139)


## Version 138.0.3351.132: August 7, 2025

Fixed various bugs, and performance issues for Extended Stable Channel.

## Version 138.0.3351.121: July 31, 2025

Fixed various bugs and performance issues for Stable Channel

Stable channel security updates are listed [here](/deployedge/microsoft-edge-relnotes-security#july-31-2025).

## Version 138.0.3351.109: July 25, 2025

Fixed various bugs, feature updates, and performance issues for Stable Channel.

Stable channel security updates are listed [here](/deployedge/microsoft-edge-relnotes-security#july-25-2025).

### Feature updates

- **Edge contextual capabilities in Business Chat work tab**.  Microsoft Copilot in Edge now supports page summarization and contextual queries to the Work tab for Microsoft 365 Copilot Business Chat. With this feature, users can ask Copilot contextual queries such as “summarize this page.” This feature also includes contextual prompt suggestions to help users ask relevant questions about open pages in Edge. Page summarization and contextual prompt suggestions is accessible for users when using Copilot through the Edge side pane. 
 

  A Microsoft 365 Copilot license is required to use this feature.  Administrators can control the availability using the [EdgeEntraCopilotPageContext](/deployedge/microsoft-edge-policies#edgeentracopilotpagecontext) policy.  


## Version 138.0.3351.95: July 16, 2025

Fixed various bugs, feature updates, and performance issues for Stable Channel.

Stable channel security updates are listed [here](/deployedge/microsoft-edge-relnotes-security#july-16-2025).

### Feature updates

- **Microsoft Edge policies to manage Shadow IT**. This feature restricts access to non-Microsoft Generative AI tools using Edge policies.  Using the [WebContentFilteringBlockedCategories](/deployedge/microsoft-edge-browser-policies/webcontentfilteringblockedcategories) policy, admins can restrict access to other LLMs (except Copilot Chat) along with all browsers (except Microsoft Edge). This helps admins address the shadow IT problem, which is the use of Gen AI tools without oversight of IT admins in the organization. Some of these Gen AI apps can cause data loss and don't comply with the organization's security policies.

## Version 138.0.3351.83: July 10, 2025

Fixed various bugs and performance issues for Stable Channel.

### Improved reliability

- Fixed a browser crash that occurred when the [BrowsingDataLifetime](/deployedge/microsoft-edge-browser-policies/browsingdatalifetime) policy was enabled.

## Version 138.0.3351.77: July 7, 2025

Fixed various bugs and performance issues and feature updates.

### Fixes

- Reverted a change that caused audio issues when playing videos with AAC audio on certain websites.  This is planned to be a temporary mitigation, as the root cause is a bug in outdated versions of the HLS.js library used by websites.  Affected site owners are encouraged to update to a newer version of HLS.js to ensure compatibility.

### Feature Updates

- **Find on Page in Microsoft Edge for Business will soon be integrated with Microsoft 365 Copilot Chat**.  Microsoft Edge for Business is introducing Microsoft 365 Copilot Chat to Find on Page (CTRL+F). This feature seeks to help users more easily find relevant content and save time.


## Version 138.0.3351.65: July 1, 2025

Fixed various bugs and performance issues for Stable Channel.

Stable channel security updates are listed [here](/deployedge/microsoft-edge-relnotes-security#july-1-2025).

## Version 138.0.3351.55: June 26, 2025

Fixed various bugs and performance issues, feature updates, policy updates, and web platform release notes.

Stable channel security updates are listed [here](/deployedge/microsoft-edge-relnotes-security#June-26-2025).

### Fixes

- Fixed an issue, which caused WebDriver automation to fail in Microsoft Edge versions 133 and later. 
 
- Fixed an issue where re-enabled `<textarea>` elements remained noneditable.  This issue affected activating a role assignment in Privileged Identity Management.  
 
### Feature updates

- **Inline protections integrated with Microsoft Purview**. Microsoft Edge for Business is introducing integrated protections using Microsoft Purview. Without using browser extensions, [Admins in Purview can configure policies to collect and protect data that users share with unmanaged generative AI apps](/purview/dlp-browser-dlp-learn), detecting for sensitive information inline and auditing or blocking the interaction accordingly.

- **Use Primary work profile as default profile to open external links**.  Microsoft Edge currently opens external links using the “Last Used” profile by default. While for enterprise users, the Primary Work Profile (signed in with a Microsoft Entra ID for enrolling the device) is normally the best profile for opening external links. With this feature, for Windows, Edge checks if the Primary Work Profile exists and makes it the default profile for opening external links if available. For Mac and Linux, if only one work profile signed in with a Microsoft Entra ID account is found, it’s treated as the Primary Work Profile. Admins can control availability to this feature using the  [EdgeOpenExternalLinksWithPrimaryWorkProfileEnabled](/deployedge/microsoft-edge-browser-policies/edgeopenexternallinkswithprimaryworkprofileenabled) policy. **Note:** This is a controlled feature rollout. If you don't see this feature, check back as we continue our rollout.

- **New Autofill Personal Information Settings Configuration**.  A web form field collection consent toggle will be available in Autofill settings (edge://settings/autofill/personalInfo). This allows users to consent to Microsoft Edge collecting web form field labels (for example, "First Name," "Email") to improve Autofill suggestion accuracy.  Only field labels are collected and not user-entered data.  The web field labels are stored securely per Microsoft's [privacy standards](https://www.microsoft.com/en-us/privacy/privacystatement).
 
  This new setting is manageable via existing policies in Autofill (for example, [AutofillAddressEnabled](/deployedge/microsoft-edge-browser-policies/autofilladdressenabled), [EdgeAutofillMlEnabled](/deployedge/microsoft-edge-browser-policies/edgeautofillmlenabled). [AutofillAddressEnabled](/deployedge/microsoft-edge-browser-policies/autofilladdressenabled)) is the parent setting for (EdgeAutofillMlEnabled)[/deployedge/microsoft-edge-browser-policies/edgeautofillmlenabled]. The EdgeAutofillMlEnabled policy is the parent of this new setting, thus turning off the EdgeAutofillMlEnabled policy turns off this setting.  **Note:** These features are a controlled feature rollout. If you don't see these features, check back as we continue our rollout.

- **AI-powered History search**. Enhanced search finds sites in your History even when you use a synonym, phrase, or typo. After this feature is turned on, sites you visit will be shown in enhanced history search results. An on-device model is trained using your data, which never leaves your device and is never sent to Microsoft. Admins can control availability to this feature using the [EdgeHistoryAISearchEnabled](/deployedge/microsoft-edge-browser-policies/edgehistoryaisearchenabled) policy. **Note:** This is a controlled feature rollout. If you don't see this feature, check back as we continue our rollout.
 
- **Microsoft 365 Copilot Chat Summarization in Microsoft Edge Context Menu**. Microsoft Edge is introducing a Microsoft 365 Copilot Chat summarization menu item to our context menu. This feature helps users quickly unpack and ask questions about their open page. **Note:** This feature is a controlled feature rollout. If you don't see this feature, check back as we continue our rollout.

- **Improvements to surfacing performance notifications**. Microsoft Edge is making improvements to how users can learn about and improve their browser's responsiveness. Performance and Extensions Detector notifications may appear in the **Settings and more menu** when Edge's performance slows. **Note:** This feature is a controlled feature rollout. If you don't see this feature, check back as we continue our rollout.
 
- **Copilot on the Microsoft Edge New Tab Page (NTP)**. Starting at the end of May 2025, users may see suggested work and productivity-related Copilot prompts by their search box on the NTP page. Also, users may see the Copilot icon in their search box allowing them to click on the icon to send their current search query to Copilot. The Copilot admin policy [NewTabPageBingChatEnabled](/deployedge/microsoft-edge-browser-policies/newtabpagebingchatenabled) continues to be enforced and will still apply. NTP changes are rolled out to all Microsoft Edge release channels. **Note:** These features are a controlled feature rollout. If you don't see these features, check back as we continue our rollout.

- **Adding support for viewing Sensitivity labels applied to a Microsoft Information Protection (MIP) Protected PDF**. Enterprise customers can view sensitivity labels applied to MIP protected PDF to be well informed of the data classification to enable them to handle such sensitive documents. This change is available in the new Microsoft Edge built-in PDF reader. **Note:** This is a controlled feature rollout. If you don't see this feature, check back as we continue our rollout.

### Policy updates

#### New policies

- [BuiltInAIAPIsEnabled](/deployedge/microsoft-edge-browser-policies/builtinaiapisenabled) - Allow pages to use the built-in AI APIs
- [EdgeHistoryAISearchEnabled](/deployedge/microsoft-edge-browser-policies/edgehistoryaisearchenabled) - Control access to AI-enhanced search in History
- [EdgeOpenExternalLinksWithPrimaryWorkProfileEnabled](/deployedge/microsoft-edge-browser-policies/edgeopenexternallinkswithprimaryworkprofileenabled) - Use Primary Work Profile as default to open external link
- [LocalNetworkAccessRestrictionsEnabled](/deployedge/microsoft-edge-browser-policies/localnetworkaccessrestrictionsenabled) - Specifies whether to block requests from public websites
- [PrefetchWithServiceWorkerEnabled](/deployedge/microsoft-edge-browser-policies/prefetchwithserviceworkerenabled) - Allow SpeculationRules prefetch for ServiceWorker-controlled URLs
- [TLS13EarlyDataEnabled](/deployedge/microsoft-edge-browser-policies/tls13earlydataenabled) - Control whether TLS 1.3 Early Data is enabled in Microsoft Edge

#### Obsoleted policies

- [InsecurePrivateNetworkRequestsAllowed](/deployedge/microsoft-edge-browser-policies/insecureprivatenetworkrequestsallowed) - Specifies whether to allow websites to make requests to any network endpoint in an insecure manner (obsolete)
- [InsecurePrivateNetworkRequestsAllowedForUrls](/deployedge/microsoft-edge-browser-policies/insecureprivatenetworkrequestsallowedforurls) - Allow the listed sites to make requests to more-private network endpoints from in an insecure manner (obsolete)
- [PrivateNetworkAccessRestrictionsEnabled](/deployedge/microsoft-edge-browser-policies/privatenetworkaccessrestrictionsenabled) - Specifies whether to apply restrictions to requests to more private network endpoints (obsolete)
- [ZstdContentEncodingEnabled](/deployedge/microsoft-edge-browser-policies/zstdcontentencodingenabled) - Enable zstd content encoding support (obsolete)

>[!NOTE]
>For the latest web platform features and updates, see [Microsoft Edge 138 web platform release notes (June 2025)](/microsoft-edge/web-platform/release-notes/138)




<!-- ===================== snip for archive ========================== -->
<!-- Version 130.0.2849.46: Octovber 17, 2024 to Version 137.0.3296.93: June 20, 2025 --->
<!-- Version  129.0.2792.52: September 12, 2024 to Version 129.0.2792.89: October 10, 2024 --->
<!-- Version 128.0.2739.79: September 12, 2024 to Version 128.0.2739.42: August 22, 2024 --->
<!-- Version 127.0.2651.105: August 15, 2024 to Version 127.0.2651.74: July 25, 2024 --->
<!-- Version 126.0.2592.113: July 18, 2024 to Version 126.0.2592.61: June 17, 2024 --->
<!-- Version 124.0.2478.109: May 16, 2024 to Version 124.0.2478.51: April 18, 2024 -->
<!-- Version 123.0.2420.97: April 12, 2024 to Version 123.0.2420.53: March 22, 2024 -->
<!-- Version 122.0.2365.106: March 21, 2024 to Version 120.0.2210.181: February 20, 2024 -->
<!-- Version 121.0.2277.128: February 15, 2024 to Version 118.0.2088.122: November 29, 2023 -->
<!-- Version 119.0.2151.97: November 29, 2023 to Version 118.0.2088.57: October 18, 2023 -->
<!-- from Version 118.0.2088.46: October 13, 2023 to Version 109.0.1518.140: September 15, 2023 -->
<!-- from Version 117.0.2045.31: September 15, 2023 to Version 116.0.1938.62: August 25, 2023 -->
<!-- from Version 116.0.1938.54: August 21, 2023 to Version 114.0.1823.41: June 6, 2023 -->
<!-- from Version 114.0.1823.37: June 2, 2023 to Version 112.0.1722.77: May 9, 2023 -->
<!-- from Version 113.0.1774.35: May 5, 2023 to Version 112.0.1722.39: April 10, 2023 -->
<!-- from Version 112.0.1722.34: April 6, 2023 to Version 111.0.1661.43: March 15, 2023 -->
<!-- from Version 111.0.1661.41: March 13, 2023 to Version 110.0.1587.46: February 14, 2023 -->
<!-- from Version Version 110.0.1587.41: February 9, 2023 to Version 108.0.1462.83: January 12, 2023 -->
<!-- from Version 109.0.1518.49: January 12, 2023 to Version 108.0.1462.46: December 8, 2022 -->
<!-- from Version 108.0.1462.42: December 5, 2022 to Version 106.0.1370.59: October 27, 2022 -->
<!--- from Version 107.0.1418.24: October 27, 2022 to Version 106.0.1370.37: October 6, 2022 -->
<!--- from Version 106.0.1370.34: October 3, 2022 to Version 105.0.1343.27: September 2, 2022 -->
<!--- from Version 105.0.1343.25: September 1, 2022 to  Version 104.0.1293.70: August 25, 2022 -->
<!--- from Version 104.0.1293.63: August 19 to Version 102.0.1245.50: June 23 ---->
<!--- from Version 103.0.1264.37: June 23 to Version 102.0.1245.33: June 3 ---->
<!--- from Version 103.0.1264.37: June 23 to Version 102.0.1245.33: June 3 ---->
<!--- from Version 102.0.1245.30: May 31 to Version 100.0.1185.57: May 2 ---->
<!-- from Version 101.0.1210.32: April 28 to Version 100.0.1185.36: April 7 -->
<!---from Version 100.0.1185.29: April 1  to  Version 99.0.1150.36: March 7 --->
<!--- from Version 99.0.1150.30: March 3 to Version 98.0.1108.50: February 10 --->
<!--- from Version 98.0.1108.43: February 3 to Version 96.0.1054.72: January 6  -->
<!---- From Version 97.0.1072.55: January 6 to Version 96.0.1054.34: November 23 ---->
<!---archive from Version 96.0.1054.29: November 19 to Version 94.0.992.57: October 27 --->
<!-- archive from Version 95.0.1020.30: October 21 to Version 94.0.992.37: September 30 -->
<!-- archive from Version 94.0.992.31: September 24 to Version 93.0.961.44: September 9  -->
<!--- Archive from Version 93.0.961.38: September 2 to Version 92.0.902.62: July 29 --->
<!-- Archive from Version 92.0.902.55: July 22 to Version 91.0.864.37: May 27 -->
<!-- Archive from 89.0.774.45: March 4 to 90.0.818.66: May 20 ->
<!-- Archive from 86.0.622.43: October 15 to beta 88.0.705.81: February 25  ->
<!-- Archive from 86.0.622.38-october-9 to beta 86.0.62.215-september-14  ->
<!-- Archived to version 84.0.522.40: July 16 -->

## See also

- [Microsoft Edge Enterprise landing page](https://aka.ms/EdgeEnterprise)
