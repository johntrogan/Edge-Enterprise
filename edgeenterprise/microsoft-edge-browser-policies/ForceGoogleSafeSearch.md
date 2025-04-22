---
title: "Microsoft Edge Browser Policy Documentation ForceGoogleSafeSearch"
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
description: "Windows and Mac documentation for supported Microsoft Edge Browser policy: Enforce Google SafeSearch"
---

# ForceGoogleSafeSearch

## Enforce Google SafeSearch


## Supported versions

- On Windows and macOS since 77 or later

## Description

Forces queries in Google Web Search to be performed with SafeSearch set to active, and prevents users from changing this setting.

If you enable this policy, SafeSearch in Google Search is always active.

If you disable this policy or don't configure it, SafeSearch in Google Search isn't enforced.

## Supported features

- Can be mandatory: No
- Can be recommended: No
- Dynamic Policy Refresh: Yes
- Per Profile: Yes
- Applies to a profile that is signed in with a Microsoft account: Yes

## Data type

- Boolean

## Windows information and settings

### Group Policy (ADMX) info

- GP unique name: ForceGoogleSafeSearch
- GP name: Enforce Google SafeSearch
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
- Value name: ForceGoogleSafeSearch
- Value type: REG_DWORD

#### Example value

```
0x00000000
```


## Mac information and settings

- Preference Key name: ForceGoogleSafeSearch
- Example value:

```xml
<false/>
```

## See also
- [Microsoft Edge - Policies](../microsoft-edge-policies.md)
