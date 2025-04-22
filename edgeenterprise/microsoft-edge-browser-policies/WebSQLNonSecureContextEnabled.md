---
title: "Microsoft Edge Browser Policy Documentation WebSQLNonSecureContextEnabled"
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
description: "Windows and Mac documentation for supported Microsoft Edge Browser policy: Force WebSQL in non-secure contexts to be enabled (obsolete)"
---

# WebSQLNonSecureContextEnabled

## Force WebSQL in non-secure contexts to be enabled (obsolete)
> OBSOLETE: This policy is obsolete and doesn't work after Microsoft Edge 112.

## Supported versions

- On Windows and macOS since 107, until 112

## Description

This policy doesn't work because WebSQL in non-secure contexts is on by default as of Microsoft Edge 105.
If you enable this policy, WebSQL in non-secure contexts will be enabled.
If you disable or don't configure this policy, WebSQL in non-secure contexts will follow the default settings of the browser.

This policy was removed in Microsoft Edge 113 and is ignored if configured.

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

- GP unique name: WebSQLNonSecureContextEnabled
- GP name: Force WebSQL in non-secure contexts to be enabled (obsolete)
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
- Value name: WebSQLNonSecureContextEnabled
- Value type: REG_DWORD

#### Example value

```
0x00000001
```


## Mac information and settings

- Preference Key name: WebSQLNonSecureContextEnabled
- Example value:

```xml
<true/>
```

## See also
- [Microsoft Edge - Policies](../microsoft-edge-policies.md)
