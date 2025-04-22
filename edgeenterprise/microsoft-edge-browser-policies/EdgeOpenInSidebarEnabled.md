---
title: "Microsoft Edge Browser Policy Documentation EdgeOpenInSidebarEnabled"
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
description: "Windows and Mac documentation for supported Microsoft Edge Browser policy: Enable open in sidebar"
---

# EdgeOpenInSidebarEnabled

## Enable open in sidebar


## Supported versions

- On Windows and macOS since 122 or later

## Description

Allow/Disallow user open a website or an app to the sidebar.

If you enable or don't configure this policy, users will be able to access the feature.
If you disable this policy, users will not be able to access the feature.

## Supported features

- Can be mandatory: No
- Can be recommended: No
- Dynamic Policy Refresh: No - Requires browser restart
- Per Profile: No
- Applies to a profile that is signed in with a Microsoft account: Yes

## Data type

- Boolean

## Windows information and settings

### Group Policy (ADMX) info

- GP unique name: EdgeOpenInSidebarEnabled
- GP name: Enable open in sidebar
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
- Value name: EdgeOpenInSidebarEnabled
- Value type: REG_DWORD

#### Example value

```
0x00000001
```


## Mac information and settings

- Preference Key name: EdgeOpenInSidebarEnabled
- Example value:

```xml
<true/>
```

## See also
- [Microsoft Edge - Policies](../microsoft-edge-policies.md)
