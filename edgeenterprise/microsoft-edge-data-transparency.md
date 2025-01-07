---
title: "Microsoft Edge Data Transparency For Connecte Users"
ms.author: archandr
author: dan-wesley
manager: likuba
ms.date: 01/07/2025
audience: ITPro
ms.topic: conceptual
ms.service: microsoft-edge
ms.localizationpriority: medium
ms.collection: M365-modern-desktop
description: "Microsoft Edge Data Transparency For Connecte Users"
---

# Data transparency in Microsoft Edge: Connected Experiences for Entra ID users 

The connected experiences in Microsoft Edge help you to search, discover, collaborate, and access work apps on the web more productively. For example, you can translate the contents of a web page into a different language, or automatically group tabs. Connected experiences might analyze the content of the web pages you're seeing in Microsoft Edge to offer editing suggestions, help you discover related articles, and more. Microsoft Copilot, Editor, and Text Prediction are all examples of connected experiences.

Microsoft Edge is committed to enhancing user productivity by providing innovative features while maintaining the highest standards of privacy and security. We offer policies to disable or configure these features as needed.

This article provides information for administrators and end users about the data collected by connected experiences available to Entra ID users and how Microsoft Edge processes this data.  

The Data retention section refers to the data outlined in this document: page content, title, url, or user input. For more details about these features or about diagnostics data, refer to [Microsoft Edge Privacy Whitepaper](/legal/microsoft-edge/privacy), [Manage Connected Experiences in Microsoft Edge](https://support.microsoft.com/microsoft-edge/manage-connected-experiences-in-microsoft-edge-6cd3d4b3-ec94-4ac6-92e6-89d0127a5e33), and [Microsoft Privacy Statement](https://www.microsoft.com/privacy/privacystatement).

The following table summarizes the connected experiences.

| Connected Experience  | Uses LLM or SLM  | Sends page content, title, or URL  | Sends user input  | Is Microsoft processor or controller  | Data retention  | Example of data  | Feature policy  |
|:---|:---|:---|:---|:---|:---|:---|:---|
| **Copilot**  |  |  |  |  |  |  |  |
| [Microsoft 365 Copilot](/copilot/edge)  | x  | x  | x  | Microsoft is data processor  | Transient data (<48h)  | Prompt user enters in Copilot in Edge  | |
| [Microsoft Copilot](/copilot/edge)  | x  | x  | x  | Microsoft is data processor  | Transient data (<48h)  | Prompt user enters in Copilot in Edge  | |
| [Page Context in Copilot](/copilot/edge)  | x  | x  | x  | Microsoft is data processor  | Transient data (<48h)  | Content of the user’s current page to help answer a contextual prompt  | [https://learn.microsoft.com/deployedge/microsoft-edge-policies#edgeentracopilotpagecontext](/deployedge/microsoft-edge-policies#edgeentracopilotpagecontext) | 
| [Tab Auto Grouping](/legal/microsoft-edge/privacy#tab-organization)  | x  | x  |  | Microsoft is data controller | Transient data (<48h)  | Page title and URL to generate tab groups  | [https://learn.microsoft.com/deployedge/microsoft-edge-policies#tabservicesenabled](/deployedge/microsoft-edge-policies#tabservicesenabled)  |
| [Tab Auto Naming](/legal/microsoft-edge/privacy#tab-organization)  | x  | x  |  | Microsoft is data controller | Transient data (<48h)  | Page title and URL to generate tab groups  | [https://learn.microsoft.com/deployedge/microsoft-edge-policies#tabservicesenabled](/deployedge/microsoft-edge-policies#tabservicesenabled)  |
| [Workspaces](/legal/microsoft-edge/privacy#workspaces)  |  | x  | x  | Microsoft is data controller | Retained (only to provide the service)  | Set of tabs and favorites curated by the user in a workspace to share with their collaborators  | [https://learn.microsoft.com/deployedge/microsoft-edge-policies#edgeworkspacesenabled](/deployedge/microsoft-edge-policies#edgeworkspacesenabled)  |
| [Collections](/legal/microsoft-edge/privacy#collections)  |  | x  | x  | Microsoft is data controller | Retained (only to provide the service)  | Collections, saved items, notes, and images within a Collection to sync across devices  | [https://learn.microsoft.com/deployedge/microsoft-edge-policies#edgecollectionsenabled](/deployedge/microsoft-edge-policies#edgecollectionsenabled)  |
| [Translate](/legal/microsoft-edge/privacy#translate) |  | x |  | Microsoft is data controller | Retained (to provide the service and for service improvement)  | Text of the user’s webpage, along with *to* and *from* language to translate  | [https://learn.microsoft.com/deployedge/microsoft-edge-policies#translateenabled](/deployedge/microsoft-edge-policies#translateenabled)     |
| [Editor](/legal/microsoft-edge/privacy#writing-assistance)  |  | x  | x  | Microsoft is data controller | Transient data (<48h)  | Texted user types to detect spelling and grammar errors  | [https://learn.microsoft.com/deployedge/microsoft-edge-policies#microsofteditorproofingenabled](/deployedge/microsoft-edge-policies#microsofteditorproofingenabled)<br> [https://learn.microsoft.com/en-us/deployedge/microsoft-edge-policies#microsofteditorsynonymsenabled](/deployedge/microsoft-edge-policies#microsofteditorsynonymsenabled)  |
| [Text Prediction](/legal/microsoft-edge/privacy#text-prediction)  |  | x  | x | Microsoft is data controller | Retained (to provide the service and for service improvement)  | Characters typed by the user, top language from browser setting and a text box identifier to generate text predictions  | [https://learn.microsoft.com/deployedge/microsoft-edge-policies#textpredictionenabled](/deployedge/microsoft-edge-policies#textpredictionenabled)  |
 | [Autofill (sub-feature: ML suggestions)](/legal/microsoft-edge/privacy#autofill) |  | x | x | Microsoft is data controller | Transient data (<48h) |  Form metadata from current page along with the user’s sync   |  |
 | [Image Descriptions](/legal/microsoft-edge/privacy#image-descriptions) | | x |  |  Microsoft is data controller | Transient data (<48h) | Images without alt text to generate captions. Only when a screen reader is connected to Microsoft Edge |[https://learn.microsoft.com/deployedge/microsoft-edge-policies#accessibilityimagelabelsenabled ](/deployedge/microsoft-edge-policies#accessibilityimagelabelsenabled )  |
 | [Speech Recognition](/legal/microsoft-edge/privacy#speech-recognition) |   |   | x |  Microsoft is data controller |  Transient data (<48h)   | Recorded audio to translate into text | [https://learn.microsoft.com/deployedge/microsoft-edge-policies#speechrecognitionenabled](/deployedge/microsoft-edge-policies#speechrecognitionenabled)   |
 | [Read Aloud (sub-feature: Online Voices)](/legal/microsoft-edge/privacy#read-aloud)  |  | x  |  | Microsoft is data controller | Transient data (<48h)  | Content of the user’s webpage to convert from text to speech  | [https://learn.microsoft.com/deployedge/microsoft-edge-policies#readaloudenabled](/deployedge/microsoft-edge-policies#readaloudenabled)   |
 | [Developer Tools (sub-feature: Explain Console Errors)](/legal/microsoft-edge/privacy#read-aloud)  | x  | x  |  | Microsoft is data controller | Transient data (<48h)  | Error message content from the page to explain console error  | [https://learn.microsoft.com/deployedge/microsoft-edge-policies#developertoolsavailability](/deployedge/microsoft-edge-policies#developertoolsavailability)  |
 | [Web Content Filtering](/deployedge/microsoft-edge-web-content-filtering)  |  | x  |  | Microsoft is data controller | Transient data (<48h)  | When admin configures this feature, URL of the page user is trying to access is used to retrieve the site category, the page is blocked if it's a category blocked by admin  | [https://learn.microsoft.com/deployedge/microsoft-edge-web-content-filtering](/deployedge/microsoft-edge-web-content-filtering)  |
 |  [Website Typo Protection](https://www.microsoft.com/edge/learning-center/how-edge-can-protect-you-from-typosquatting?form=MA13I2)  |  | x  |  | Microsoft is data controller | Retained (only to provide the service)  | URL is used to warn user if they mistype a popular domain name and could land on a malicious webpage  | [https://learn.microsoft.com/deployedge/microsoft-edge-policies#preventtyposquattingpromptoverride](/deployedge/microsoft-edge-policies#preventtyposquattingpromptoverride)  |
 | [Password Monitor](/legal/microsoft-edge/privacy#password-monitor)  |  |  | x  | Microsoft is data controller | Transient data (<48h)  | Saved credentials are compared against encrypted list of known breached credentials to warn user about potential breach  | [https://learn.microsoft.com/deployedge/microsoft-edge-policies#passwordmonitorallowed](/deployedge/microsoft-edge-policies#passwordmonitorallowed )  |
 | [Geolocation (inference service)](/legal/microsoft-edge/privacy#geolocation)  |  |  |  | Microsoft is data controller | Transient data (<48h)  | Device IP address, or device location if user grants access, is provided to websites that request device location  | [https:/deployedge/microsoft-edge-policies#defaultgeolocationsetting](/deployedge/microsoft-edge-policies#defaultgeolocationsetting)|
 | [Suggest Similar Pages](/legal/microsoft-edge/privacy#suggest-similar-sites)  |  | x  |  | Microsoft is data controller | Transient data (<48h)  | Domain of the web address to suggest a corrected URL when a navigation error occurs  | [https://learn.microsoft.com/\deployedge/microsoft-edge-policies#alternateerrorpagesenabled](/deployedge/microsoft-edge-policies#alternateerrorpagesenabled)   |
 | [Edge Recommendations (ENP)](/legal/microsoft-edge/privacy#shopping)  |  |  | x  | Microsoft is data controller | Transient data (<48h)  | Typed characters for search to provide user with relevant tips and feature recommendations  | [https://learn.microsoft.com/deployedge/microsoft-edge-policies#showrecommendationsenabled](/deployedge/microsoft-edge-policies#showrecommendationsenabled)  | 
 | [Rewards](/legal/microsoft-edge/privacy#rewards)  |  |  |  | Microsoft is data controller | Retained (to provide the service and for service improvement)  | In case of linked MSA account for an Entra ID profile, the rewards service uses the Microsoft account identity to add points for searching, playing, and shopping on Microsoft Edge  | [https://learn.microsoft.com/deployedge/microsoft-edge-policies#showmicrosoftrewards](/deployedge/microsoft-edge-policies#showmicrosoftrewards)   |  
 | [Shopping](/legal/microsoft-edge/privacy#shopping)  |  | x  |  | Microsoft is data controller | Retained (to provide the service and for service improvement)  | URL and page content if the page was determined as a shopping domain, to help user find coupons, rebates, and better prices  | [https://learn.microsoft.com//deployedge/microsoft-edge-policies#edgeshoppingassistantenabled ](/deployedge/microsoft-edge-policies#edgeshoppingassistantenabled)   |
 | [Supported Causes & Nonprofits](/legal/microsoft-edge/privacy#shopping)  |  | x  | x  | Microsoft is data controller | Retained (only to provide the service)  | Payment method details if user chooses to save card to facilitate donations when user visits Edge Wallet or charity websites  | [https://learn.microsoft.com/deployedge/microsoft-edge-policies#walletdonationenabled](/deployedge/microsoft-edge-policies#walletdonationenabled) |

In addition to the preceding connected experiences, the services in the following table provide core functionality for the browser, or significantly enhance the usability, security, and overall browsing experience in Microsoft Edge. These features can be managed through individual policies. To learn more about these features, refer to [Microsoft Edge Privacy Whitepaper](/legal/microsoft-edge/privacy).

| Feature name | Feature description | Feature policy |
|:------|:-------|:------|
| [Network Time](/legal/microsoft-edge/privacy#network-time) | Microsoft network time service to track time from an external source such as a time server. | [https://learn.microsoft.com/deployedge/microsoft-edge-policies#browsernetworktimequeriesenabled](/deployedge/microsoft-edge-policies#browsernetworktimequeriesenabled) |
| [Edge Asset Delivery](/deployedge/microsoft-edge-policies#edgeassetdeliveryserviceenabled) | General pipeline used to deliver assets to the Microsoft Edge Clients. These assets can be config files or Machine Learning models that power the features that use this service. | [https://learn.microsoft.com/deployedge/microsoft-edge-policies#edgeassetdeliveryserviceenabled ](/deployedge/microsoft-edge-policies#edgeassetdeliveryserviceenabled) |
| [Navigation Errors](/legal/microsoft-edge/privacy#resolve-navigation-errors) | If Microsoft Edge detects SSL connection timeouts, certificate errors, or other network issues that are caused by a captive portal, it runs network connectivity tests | [https://learn.microsoft.com/deployedge/microsoft-edge-policies#resolvenavigationerrorsusewebservice](/deployedge/microsoft-edge-policies#resolvenavigationerrorsusewebservice) |
| [Edge Diagnostic Data](/legal/microsoft-edge/privacy#diagnostic-data)  | Required diagnostic data is collected to keep Microsoft Edge secure, up to date and performing as expected, but can be disabled by organizations. | [https://learn.microsoft.com/deployedge/microsoft-edge-policies#diagnosticdata](/deployedge/microsoft-edge-policies#diagnosticdata) |
| [SmartScreen](/legal/microsoft-edge/privacy#smartscreen) | Provides warning messages to help protect users from potential phishing scams and malicious software. | [https://learn.microsoft.com/deployedge/microsoft-edge-policies#smartscreenenabled](/deployedge/microsoft-edge-policies#smartscreenenabled) |
| [Experimentation and Configuration Service](/deployedge/edge-configuration-and-experiments) | To enable new functions for randomly selected users, Microsoft Edge regularly sends required information about OS, channel, and other device configuration data to the configuration service. | [https://learn.microsoft.com/deployedge/microsoft-edge-policies#experimentationandconfigurationservicecontrol](/deployedge/microsoft-edge-policies#experimentationandconfigurationservicecontrol) |
| [New Tab Page](/legal/microsoft-edge/privacy#new-tab-page)  | This is the default "Start Page," powered by MSN/Start that shows news and other information to users when a new tab is created. | [https://learn.microsoft.com/deployedge/microsoft-edge-policies#newtabpagelocation](/deployedge/microsoft-edge-policies#newtabpagelocation) |
| [Sync](/legal/microsoft-edge/privacy#sync)| The synced data is also stored in an encrypted state in Microsoft servers. If you're using a work or school account, all data types are further encrypted before being synced using Microsoft Purview Information Protection. | [https://learn.microsoft.com/deployedge/microsoft-edge-policies#syncdisabled ](/deployedge/microsoft-edge-policies#syncdisabled) |
| [Address bar Suggestions](/legal/microsoft-edge/privacy#address-bar-and-suggestions)| Suggestions are presented to the user as they type in the address bar. | [https://learn.microsoft.com/deployedge/microsoft-edge-policies#searchsuggestenabled](/deployedge/microsoft-edge-policies#searchsuggestenabled) |
| [Autofill](/legal/microsoft-edge/privacy#autofill) | This service helps users autofill form data |  [https://learn.microsoft.com/deployedge/microsoft-edge-policies#autofilladdressenabled](/deployedge/microsoft-edge-policies#autofilladdressenabled)<br><br>[https://learn.microsoft.com/deployedge/microsoft-edge-policies#autofillcreditcardenabled](/deployedge/microsoft-edge-policies#autofillcreditcardenabled)<br><br>[https://learn.microsoft.com/deployedge/microsoft-edge-policies#autofillmembershipsenabled](/deployedge/microsoft-edge-policies#autofillmembershipsenabled)  |

Microsoft Edge also supports features based on administrator configurations; this includes:

- Security and compliance features.
- Other add-on services that admins can configure (such as Bing at Work, and Enterprise New Tab Page.)

When the enterprise features in the next table are turned on, the browser sends auditing and diagnostic data to the administrator as per the feature's need to function, and manage or diagnose properly. This data collection is controlled by the enterprise administrator and end users aren't able to opt out.

| Feature | Article |
|:-----|:-----|
| Windows Information Protection (WIP)     |  [Protect your enterprise data using Windows Information Protection (WIP)](/windows/security/information-protection/windows-information-protection/protect-enterprise-data-using-wip)     |
| Microsoft Endpoint Data Loss Prevention (DLP)    | [Learn about Endpoint data loss prevention](/microsoft-365/compliance/endpoint-dlp-learn-about) |
| Microsoft Purview Information Protection (MPIP)  | [Protect Office documents with Microsoft Purview \| Microsoft Learn](/deployedge/microsoft-edge-management-service-office-mip)      |
| Microsoft Defender for Cloud Apps (Preview)     |  [Session policies](/defender-cloud-apps/session-policy-aad)    |
| Microsoft Insider Risk Management | [Insider risk management](/microsoft-365/compliance/insider-risk-management-solution-overview)  |
| Microsoft Edge management service | [Microsoft Edge management service](/deployedge/microsoft-edge-management-service) |
| Intune Mobile Application Management (MAM)      |  [Manage Microsoft Edge on iOS and Android with Intune](/mem/intune/apps/manage-microsoft-edge)     |
| Conditional Access     |  [Microsoft Edge and Conditional Access \| Microsoft Learn](/deployedge/ms-edge-security-conditional-access) |

## See also

- [Microsoft Edge Privacy Whitepaper](/legal/microsoft-edge/privacy)