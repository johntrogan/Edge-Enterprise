---
title: "Microsoft Edge Browser Policy Documentation BlockExternalExtensions"
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
description: "Windows and Mac documentation for supported Microsoft Edge Browser policy: Blocks external extensions from being installed"
---

# BlockExternalExtensions

## Blocks external extensions from being installed


## Supported versions

- On Windows and macOS since 88 or later

## Description

Control the installation of external extensions.

If you enable this setting, external extensions are blocked from being installed.

If you disable this setting or leave it unset, external extensions are allowed to be installed.

External extensions and their installation are documented at [Alternate extension distribution methods](/microsoft-edge/extensions-chromium/developer-guide/alternate-distribution-options).

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

- GP unique name: BlockExternalExtensions
- GP name: Blocks external extensions from being installed
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
- Value name: BlockExternalExtensions
- Value type: REG_DWORD

#### Example value

```
0x00000001
```


## Mac information and settings

- Preference Key name: BlockExternalExtensions
- Example value:

```xml
<true/>
```

## See also
- [Microsoft Edge - Policies](../microsoft-edge-policies.md)
