---
title: "Microsoft Edge Browser Policy Documentation MAMEnabled"
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
description: "Windows and Mac documentation for supported Microsoft Edge Browser policy: Mobile App Management Enabled"
---

# MAMEnabled

## Mobile App Management Enabled


## Supported versions

- On Windows and macOS since 89 or later

## Description

Allows the Microsoft Edge browser to retrieve policies from the Intune application management services and apply them to users' profiles.

If you enable this policy or don't configure it, Mobile App Management (MAM) Policies can be applied.

If you disable this policy, Microsoft Edge will not communicate with Intune to request MAM Policies.

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

- GP unique name: MAMEnabled
- GP name: Mobile App Management Enabled
- GP path (Mandatory): N/A
- GP path (Recommended): N/A
- GP ADMX file name: MSEdge.admx

#### Example value

```
Disabled
```

### Registry settings

- Path (Mandatory): N/A
- Path (Recommended): N/A
- Value name: MAMEnabled
- Value type: REG_DWORD

#### Example value

```
0x00000000
```


## Mac information and settings

- Preference Key name: MAMEnabled
- Example value:

```xml
<false/>
```

## See also
- [Microsoft Edge - Policies](../microsoft-edge-policies.md)
