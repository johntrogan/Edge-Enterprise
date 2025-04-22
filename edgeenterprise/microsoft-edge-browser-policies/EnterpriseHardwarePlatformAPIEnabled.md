---
title: "Microsoft Edge Browser Policy Documentation EnterpriseHardwarePlatformAPIEnabled"
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
description: "Windows and Mac documentation for supported Microsoft Edge Browser policy: Allow managed extensions to use the Enterprise Hardware Platform API"
---

# EnterpriseHardwarePlatformAPIEnabled

## Allow managed extensions to use the Enterprise Hardware Platform API


## Supported versions

- On Windows and macOS since 78 or later

## Description

When this policy is set to enabled, extensions installed by enterprise policy are allowed to use the Enterprise Hardware Platform API.
When this policy is set to disabled or isn't set, no extensions are allowed to use the Enterprise Hardware Platform API.
This policy also applies to component extensions.

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

- GP unique name: EnterpriseHardwarePlatformAPIEnabled
- GP name: Allow managed extensions to use the Enterprise Hardware Platform API
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
- Value name: EnterpriseHardwarePlatformAPIEnabled
- Value type: REG_DWORD

#### Example value

```
0x00000001
```


## Mac information and settings

- Preference Key name: EnterpriseHardwarePlatformAPIEnabled
- Example value:

```xml
<true/>
```

## See also
- [Microsoft Edge - Policies](../microsoft-edge-policies.md)
