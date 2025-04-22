---
title: "Microsoft Edge Browser Policy Documentation DefaultJavaScriptSetting"
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
description: "Windows and Mac documentation for supported Microsoft Edge Browser policy: Default JavaScript setting"
---

# DefaultJavaScriptSetting

## Default JavaScript setting


## Supported versions

- On Windows and macOS since 77 or later

## Description

Set whether websites can run JavaScript. You can allow it for all sites ('AllowJavaScript') or block it for all sites ('BlockJavaScript').

If you don't configure this policy, all sites can run JavaScript by default, and the user can change this setting.

Policy options mapping:

* AllowJavaScript (1) = Allow all sites to run JavaScript

* BlockJavaScript (2) = Don't allow any site to run JavaScript

Use the preceding information when configuring this policy.

## Policy options mapping:
> Use this information when configuring this policy.

- AllowJavaScript (1) = Allow all sites to run JavaScript
- BlockJavaScript (2) = Don't allow any site to run JavaScript

## Supported features

- Can be mandatory: No
- Can be recommended: No
- Dynamic Policy Refresh: Yes
- Per Profile: Yes
- Applies to a profile that is signed in with a Microsoft account: No

## Data type

- Integer

## Windows information and settings

### Group Policy (ADMX) info

- GP unique name: DefaultJavaScriptSetting
- GP name: Default JavaScript setting
- GP path (Mandatory): N/A
- GP path (Recommended): N/A
- GP ADMX file name: MSEdge.admx

#### Example value

```
Allow all sites to run JavaScript
```

### Registry settings

- Path (Mandatory): N/A
- Path (Recommended): N/A
- Value name: DefaultJavaScriptSetting
- Value type: REG_DWORD

#### Example value

```
0x00000001
```


## Mac information and settings

- Preference Key name: DefaultJavaScriptSetting
- Example value:

```xml
<integer>1</integer>
```

## See also
- [Microsoft Edge - Policies](../microsoft-edge-policies.md)
