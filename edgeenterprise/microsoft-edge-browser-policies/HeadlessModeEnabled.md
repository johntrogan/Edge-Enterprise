---
title: "Microsoft Edge Browser Policy Documentation HeadlessModeEnabled"
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
description: "Windows and Mac documentation for supported Microsoft Edge Browser policy: Control use of the Headless Mode"
---

# HeadlessModeEnabled

## Control use of the Headless Mode


## Supported versions

- On Windows and macOS since 92 or later

## Description

This policy setting lets you decide whether users can launch Microsoft Edge in headless mode.

If you enable or don't configure this policy, Microsoft Edge allows use of the headless mode.

If you disable this policy, Microsoft Edge denies use of the headless mode.

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

- GP unique name: HeadlessModeEnabled
- GP name: Control use of the Headless Mode
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
- Value name: HeadlessModeEnabled
- Value type: REG_DWORD

#### Example value

```
0x00000001
```


## Mac information and settings

- Preference Key name: HeadlessModeEnabled
- Example value:

```xml
<true/>
```

## See also
- [Microsoft Edge - Policies](../microsoft-edge-policies.md)
