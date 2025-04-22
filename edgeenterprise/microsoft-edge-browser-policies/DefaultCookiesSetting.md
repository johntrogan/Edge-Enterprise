---
title: "Microsoft Edge Browser Policy Documentation DefaultCookiesSetting"
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
description: "Windows and Mac documentation for supported Microsoft Edge Browser policy: Configure cookies"
---

# DefaultCookiesSetting

## Configure cookies


## Supported versions

- On Windows and macOS since 77 or later

## Description

Control whether websites can create cookies on the user's device. This policy is all or nothing - you can let all websites create cookies, or no websites create cookies. You can't use this policy to enable cookies from specific websites.

Set the policy to 'SessionOnly' to clear cookies when the session closes.

If you don't configure this policy, the default 'AllowCookies' is used, and users can change this setting in Microsoft Edge Settings. (If you don't want users to be able to change this setting, set the policy.)

Policy options mapping:

* AllowCookies (1) = Let all sites create cookies

* BlockCookies (2) = Don't let any site create cookies

* SessionOnly (4) = Keep cookies for the duration of the session, except ones listed in [SaveCookiesOnExit](SaveCookiesOnExit.md)

Use the preceding information when configuring this policy.

## Policy options mapping:
> Use this information when configuring this policy.

- AllowCookies (1) = Let all sites create cookies
- BlockCookies (2) = Don't let any site create cookies
- SessionOnly (4) = Keep cookies for the duration of the session, except ones listed in "SaveCookiesOnExit"

## Supported features

- Can be mandatory: No
- Can be recommended: No
- Dynamic Policy Refresh: Yes
- Per Profile: Yes
- Applies to a profile that is signed in with a Microsoft account: Yes

## Data type

- Integer

## Windows information and settings

### Group Policy (ADMX) info

- GP unique name: DefaultCookiesSetting
- GP name: Configure cookies
- GP path (Mandatory): N/A
- GP path (Recommended): N/A
- GP ADMX file name: MSEdge.admx

#### Example value

```
Let all sites create cookies
```

### Registry settings

- Path (Mandatory): N/A
- Path (Recommended): N/A
- Value name: DefaultCookiesSetting
- Value type: REG_DWORD

#### Example value

```
0x00000001
```


## Mac information and settings

- Preference Key name: DefaultCookiesSetting
- Example value:

```xml
<integer>1</integer>
```

## See also
- [Microsoft Edge - Policies](../microsoft-edge-policies.md)
