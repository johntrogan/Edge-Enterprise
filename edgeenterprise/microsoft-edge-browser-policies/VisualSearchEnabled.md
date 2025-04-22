---
title: "Microsoft Edge Browser Policy Documentation VisualSearchEnabled"
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
description: "Windows and Mac documentation for supported Microsoft Edge Browser policy: Visual search enabled"
---

# VisualSearchEnabled

## Visual search enabled


## Supported versions

- On Windows since 95 or later
- On macOS since 114 or later

## Description

Visual search lets you quickly explore more related content about entities in an image.

If you enable or don't configure this policy, visual search will be enabled via image hover, context menu, and search in sidebar.

If you disable this policy, visual search will be disabled and you won't be able to get more info about images via hover, context menu, and search in sidebar.

Note: Visual Search in Web Capture is still managed by [WebCaptureEnabled](WebCaptureEnabled.md) policy.

## Supported features

- Can be mandatory: No
- Can be recommended: Yes
- Dynamic Policy Refresh: Yes
- Per Profile: Yes
- Applies to a profile that is signed in with a Microsoft account: No

## Data type

- Boolean

## Windows information and settings

### Group Policy (ADMX) info

- GP unique name: VisualSearchEnabled
- GP name: Visual search enabled
- GP path (Mandatory): N/A
- GP path (Recommended): Administrative Templates/Microsoft Edge - Default Settings (users can override)
- GP ADMX file name: MSEdge.admx

#### Example value

```
Disabled
```

### Registry settings

- Path (Mandatory): N/A
- Path (Recommended): SOFTWARE\Policies\Microsoft\Edge\Recommended
- Value name: VisualSearchEnabled
- Value type: REG_DWORD

#### Example value

```
0x00000000
```


## Mac information and settings

- Preference Key name: VisualSearchEnabled
- Example value:

```xml
<false/>
```

## See also
- [Microsoft Edge - Policies](../microsoft-edge-policies.md)
