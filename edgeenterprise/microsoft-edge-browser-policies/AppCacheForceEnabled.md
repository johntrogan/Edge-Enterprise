---
title: "Microsoft Edge Browser Policy Documentation AppCacheForceEnabled"
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
description: "Windows and Mac documentation for supported Microsoft Edge Browser policy: Allows the AppCache feature to be re-enabled, even if it&#x27;s turned off by default (obsolete)"
---

# AppCacheForceEnabled

## Allows the AppCache feature to be re-enabled, even if it's turned off by default (obsolete)
> OBSOLETE: This policy is obsolete and doesn't work after Microsoft Edge 96.

## Supported versions

- On Windows and macOS since 84, until 96

## Description

Support for AppCache and this policy was removed from Microsoft Edge starting in version 97.

If you set this policy to true, the AppCache is enabled, even when AppCache in Microsoft Edge is not available by default.

If you set this policy to false, or don't set it, AppCache will follow Microsoft Edge's defaults.

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

- GP unique name: AppCacheForceEnabled
- GP name: Allows the AppCache feature to be re-enabled, even if it's turned off by default (obsolete)
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
- Value name: AppCacheForceEnabled
- Value type: REG_DWORD

#### Example value

```
0x00000000
```


## Mac information and settings

- Preference Key name: AppCacheForceEnabled
- Example value:

```xml
<false/>
```

## See also
- [Microsoft Edge - Policies](../microsoft-edge-policies.md)
