---
title: "Microsoft Edge Browser Policy Documentation AllowSystemNotifications"
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
description: "Windows and Mac documentation for supported Microsoft Edge Browser policy: Allows system notifications"
---

# AllowSystemNotifications

## Allows system notifications


## Supported versions

- On Windows since 117 or later

## Description

Lets you use system notifications instead of Microsoft Edge's embedded Message Center on Windows and Linux.

If set to True or not set, Microsoft Edge is allowed to use system notifications.

If set to False, Microsoft Edge will not use system notifications. Microsoft Edge's embedded Message Center will be used as a fallback.

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

- GP unique name: AllowSystemNotifications
- GP name: Allows system notifications
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
- Value name: AllowSystemNotifications
- Value type: REG_DWORD

#### Example value

```
0x00000001
```


## See also
- [Microsoft Edge - Policies](../microsoft-edge-policies.md)
