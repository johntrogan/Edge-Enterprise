---
title: "Microsoft Edge Browser Policy Documentation EnableMediaRouter"
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
description: "Windows and Mac documentation for supported Microsoft Edge Browser policy: Enable Google Cast"
---

# EnableMediaRouter

## Enable Google Cast


## Supported versions

- On Windows and macOS since 77 or later

## Description

Enable this policy to enable Google Cast. Users will be able to launch it from the app menu, page context menus, media controls on Cast-enabled websites, and (if shown) the Cast toolbar icon.

Disable this policy to disable Google Cast.

By default, Google Cast is enabled.

## Supported features

- Can be mandatory: No
- Can be recommended: No
- Dynamic Policy Refresh: No - Requires browser restart
- Per Profile: Yes
- Applies to a profile that is signed in with a Microsoft account: No

## Data type

- Boolean

## Windows information and settings

### Group Policy (ADMX) info

- GP unique name: EnableMediaRouter
- GP name: Enable Google Cast
- GP path (Mandatory): N/A
- GP path (Recommended): N/A
- GP ADMX file name: MSEdge.admx

#### Example value

```
Enabled
```

### Registry settings

- Path (Mandatory): N/A
- Path (Recommended): N/A
- Value name: EnableMediaRouter
- Value type: REG_DWORD

#### Example value

```
0x00000001
```


## Mac information and settings

- Preference Key name: EnableMediaRouter
- Example value:

```xml
<true/>
```

## See also
- [Microsoft Edge - Policies](../microsoft-edge-policies.md)
