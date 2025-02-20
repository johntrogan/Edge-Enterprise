---
title: "Microsoft Edge identity support and configuration"
ms.author: archandr
author: dan-wesley
manager: likuba
ms.date: 02/12/2025
audience: ITPro
ms.topic: conceptual
ms.service: microsoft-edge
ms.localizationpriority: medium
ms.collection: M365-modern-desktop
description: "Microsoft Edge identity support and configuration"
---

# Microsoft Edge identity support and configuration

This article describes how Microsoft Edge uses identity to support features such as sync and single sign-on (SSO). Microsoft Edge supports signing in with Active Directory Domain Services (AD DS), Microsoft Entra ID, and Microsoft accounts (MSA). Currently, Microsoft Edge only supports Microsoft Entra accounts belonging to the global cloud or the GCC sovereign cloud. We're working on adding support for other sovereign clouds.

> [!NOTE]
> This applies  to Microsoft Edge version 77 or later.

## Browser sign-in and authenticated features

Microsoft Edge supports signing into a browser profile with a Microsoft Entra ID, MSA, or a domain account. The type of account used for sign-in determines which authenticated features are available for the user in Microsoft Edge. The following table summarizes the feature support for each type of account.

| Feature   | Microsoft Entra ID | Microsoft Entra ID Free | On-premises AD DS | MSA     |
|----|------------------|---------------|----------------|---------|
| Sync | Yes | No | No | Yes |
| SSO with Primary Refresh Token | Yes | Yes | No | Yes |
| Seamless SSO | Yes | Yes | Yes | N/A |
| Integrated Windows Authentication | Yes | Yes | Yes | N/A |
| Enterprise New tab page | Requires O365 |   Requires O365 | No | N/A |
| Microsoft Search | Requires O365 | Requires O365 | No | N/A |

## How users can sign into Microsoft Edge

### Automatic sign-in

Microsoft Edge uses the OS default account to auto sign into the browser. Depending on how a device is configured, users can get auto signed into Microsoft Edge using one of the following approaches.

- **The device is hybrid/AAD-J:** Available on Win10, down-level Windows, and corresponding server versions.
The user gets automatically signed in with their Microsoft Entra account.
- **The device is domain joined:** Available on Win10, down-level Windows, and corresponding server versions.
By default, the user isn't automatically signed in. If you want to automatically sign in users with domain accounts, use the [ConfigureOnPremisesAccountAutoSignIn](./microsoft-edge-policies.md#configureonpremisesaccountautosignin) policy. If you want to automatically sign in users with their Microsoft Entra accounts, consider hybrid joining your devices.
- **OS default account is MSA:** Windows 10 Fall Creators Update (Version 1709/Build 10.0.16299) and above. This scenario is unlikely on enterprise devices. But, if the OS default account is MSA, Microsoft Edge signs in automatically with the MSA account.

### Manual sign-in

If the user doesn't get automatically signed into Microsoft Edge, they can manually sign into Microsoft Edge during the first run experience, browser settings, or by opening the identity flyout.

### Managing browser sign-in

If you want to manage browser sign-in, you can use the following policies:

- Ensure that users always have a work profile on Microsoft Edge. [See NonRemovableProfileEnabled](./microsoft-edge-policies.md#nonremovableprofileenabled)
- Restrict sign-in to a trusted set of accounts. [See RestrictSigninToPattern](./microsoft-edge-policies.md#restrictsignintopattern)
- Disable or force browser sign-in. [See BrowserSignin](./microsoft-edge-policies.md#browsersignin)

## Browser to Web Single Sign-On (SSO)

On some platforms, you can configure Microsoft Edge to automatically sign into websites for your users. This option saves them the trouble of reentering their credentials to access their work websites and increases their productivity.

### SSO with Primary Refresh Token (PRT)

Microsoft Edge has native support for PRT-based SSO, and you don't need an extension. On Windows 10 Fall Creators Update and above, if a user is signed into their browser profile, they get SSO with the PRT mechanism to websites that support PRT-based SSO.

A Primary Refresh Token (PRT) is a Microsoft Entra ID key that's used for authentication on Windows 10/11, iOS, and Android devices. It enables single sign-on (SSO) across the applications used on those devices. For more information, see [What is a Primary Refresh Token?](/azure/active-directory/devices/concept-primary-refresh-token).

### Seamless SSO

Just like PRT SSO, Microsoft Edge has native Seamless SSO support without needing an extension. On Windows 10 Fall Creators Update and above, if a user is signed into their browser profile, they get SSO with the PRT mechanism to websites that support PRT-based SSO.

Seamless Single Sign-On automatically signs users in when they're on corporate devices connected to a corporate network. When enabled, users don't need to type in their passwords to sign in to Microsoft Entra ID. Typically they don't even have to type in their usernames. For more information, see [Active Directory Seamless Single Sign-On](/azure/active-directory/hybrid/how-to-connect-sso).

### Windows Integrated Authentication (WIA)

Microsoft Edge also supports Windows Integrated Authentication for authentication requests within an organization's internal network for any application that uses a browser for its authentication. This is supported on all versions of Windows 10/11 and down-level Windows. By default, Microsoft Edge uses the intranet zone as an allowlist for WIA. Alternatively, you can customize the list of servers that are enabled for Integrated Authentication by using the [AuthServerAllowlist](./microsoft-edge-policies.md#authserverallowlist) policy. On macOS, this policy is required to enable Integrated Authentication.

To support WIA-based SSO on Microsoft Edge (version 77 and later), you might also have to do some server-side configuration. You'll probably have to configure the Active Directory Federation Services (AD FS) property **WiaSupportedUserAgents** to add support for the new Microsoft Edge user agent string. For instructions on how to do this, see [View WIASupportedUserAgent](/windows-server/identity/ad-fs/operations/configure-ad-fs-browser-wia#view-wiasupporteduseragent-settings) settings and [Change WIASupportedUserAgent](/windows-server/identity/ad-fs/operations/configure-ad-fs-browser-wia#change-wiasupporteduseragent-settings) settings. An example of the Microsoft Edge user agent string on Windows 10 is shown below, and you can learn more about the [Microsoft Edge UA string here](/microsoft-edge/web-platform/user-agent-string). 

The following example of a UA string is for the latest Dev Channel build when this article was published:<br> `"Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/80.0.3951.0 Safari/537.36 Edg/80.0.334.2"`

For services that require delegating Negotiate credentials, Microsoft Edge supports Constrained Delegation using the [AuthNegotiateDelegateAllowlist](./microsoft-edge-policies.md#authnegotiatedelegateallowlist) policy.

## Additional authentication concepts

### Proactive Authentication

Proactive authentication is an optimization over browser to website SSO that front loads authentication to certain first party websites. This improves address bar performance if the user is using Bing as the search engine. This gives users personalized and Microsoft Search for Business (MSB) search results. It also enables allowing authentication to key services such as the Office New Tab Page, MSN and Microsoft Copilot.

> [!NOTE]
> You can control this service using the [ProactiveAuthWorkflowEnabled](/deployedge/microsoft-edge-policies#proactiveauthworkflowenabled) policy for Microsoft Edge version 126 or higher;
or using [ProactiveAuthEnabled](/deployedge/microsoft-edge-policies#proactiveauthenabled) policy for Microsoft Edge version 90 or lower. For in between versions, if you want to configure browser sign in, use the [BrowserSignin](/deployedge/microsoft-edge-policies#browsersignin) policy.

> [!NOTE]
> When [Mobile Application Management (MAM)](/mem/intune/fundamentals/deployment-guide-enrollment-mamwe) is applied to Edge,
> this authentication integration will stop working. Some functionalities on New Tab Page might also be affected.

### Windows Hello CredUI for NTLM Authentication

When a website tries to sign users in using the NTLM or Negotiate mechanisms and SSO isn't available, we offer users an experience where they can share their OS credentials with the website to satisfy the authentication challenge using Windows Hello Cred UI. This sign-in flow will only appear for users on Windows 10/11 who don't get single-sign-on during an NTLM or Negotiate challenge.

### Sign in automatically using saved passwords

If a user saves passwords in Microsoft Edge, they can enable a feature that automatically logs them into websites where they have saved credentials. Users can toggle this feature by navigating to *edge://settings/passwords*. If you want to configure this ability, you can use the [password manager](./microsoft-edge-policies.md#password-manager-and-protection) policies.

## See also

- [Microsoft Edge Enterprise landing page](https://aka.ms/EdgeEnterprise)
- [Video: Microsoft Edge and Identity](microsoft-edge-video-identity.md)
- [Identity and access management](https://www.microsoft.com/security/technology/identity-access-management)
- [Identity platform](https://developer.microsoft.com/identity)
- [Four steps to a strong identity foundation with Microsoft Entra ID](/azure/active-directory/hybrid/four-steps)
