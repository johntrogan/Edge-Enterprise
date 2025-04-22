---
title: "Microsoft Edge Browser Policy Documentation FullscreenAllowed"
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
description: "Windows and Mac documentation for supported Microsoft Edge Browser policy: Allow full screen mode"
---

# FullscreenAllowed

## Allow full screen mode


## Supported versions

- On Windows since 77 or later

## Description

Set the availability of full screen mode - all Microsoft Edge UI is hidden and only web content is visible.

If you enable this policy or don't configure it, the user, apps, and extensions with appropriate permissions can enter full screen mode.

If you disable this policy, users, apps, and extensions can't enter full screen mode.

Opening Microsoft Edge in kiosk mode using the command line is unavailable when full screen mode is disabled.

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

- GP unique name: FullscreenAllowed
- GP name: Allow full screen mode
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
- Value name: FullscreenAllowed
- Value type: REG_DWORD

#### Example value

```
0x00000001
```


## See also
- [Microsoft Edge - Policies](../microsoft-edge-policies.md)
