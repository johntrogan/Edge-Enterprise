---
title: "Microsoft Edge Browser Policy Documentation KeyboardFocusableScrollersEnabled"
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
description: "Windows and Mac documentation for supported Microsoft Edge Browser policy: Enable keyboard focusable scrollers"
---

# KeyboardFocusableScrollersEnabled

## Enable keyboard focusable scrollers


## Supported versions

- On Windows and macOS since 128 or later

## Description

This policy provides a temporary opt-out for the new keyboard focusable scrollers behavior.

When this policy is Enabled or unset, scrollers without focusable children are keyboard focusable by default.

When this policy is Disabled, scrollers are not keyboard focusable by default.

This policy is a temporary workaround and will be removed in Edge Stable 135.

## Supported features

- Can be mandatory: No
- Can be recommended: No
- Dynamic Policy Refresh: Yes
- Per Profile: Yes
- Applies to a profile that is signed in with a Microsoft account: No

## Data type

- Boolean

## Windows information and settings

### Group Policy (ADMX) info

- GP unique name: KeyboardFocusableScrollersEnabled
- GP name: Enable keyboard focusable scrollers
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
- Value name: KeyboardFocusableScrollersEnabled
- Value type: REG_DWORD

#### Example value

```
0x00000001
```


## Mac information and settings

- Preference Key name: KeyboardFocusableScrollersEnabled
- Example value:

```xml
<true/>
```

## See also
- [Microsoft Edge - Policies](../microsoft-edge-policies.md)
