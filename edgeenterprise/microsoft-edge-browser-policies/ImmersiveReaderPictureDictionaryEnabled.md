---
title: "Microsoft Edge Browser Policy Documentation ImmersiveReaderPictureDictionaryEnabled"
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
description: "Windows and Mac documentation for supported Microsoft Edge Browser policy: Enable Picture Dictionary feature within Immersive Reader in Microsoft Edge (obsolete)"
---

# ImmersiveReaderPictureDictionaryEnabled

## Enable Picture Dictionary feature within Immersive Reader in Microsoft Edge (obsolete)
> OBSOLETE: This policy is obsolete and doesn't work after Microsoft Edge 126.

## Supported versions

- On Windows and macOS since 110, until 126

## Description

This Policy is obsoleted because Picture Dictionary is deprecated from Edge as of Sept, 2023. This policy won't work in Microsoft Edge Version 127. Enables the Picture Dictionary feature within Immersive Reader in Microsoft Edge.
This feature helps in reading comprehension by letting a user to click on any single word and see an illustration related to the meaning.

If you enable this policy or don't configure it, the Picture Dictionary option shows up within Immersive Reader.
If you disable this policy, users can't access the Picture Dictionary feature within Immersive Reader.

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

- GP unique name: ImmersiveReaderPictureDictionaryEnabled
- GP name: Enable Picture Dictionary feature within Immersive Reader in Microsoft Edge (obsolete)
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
- Value name: ImmersiveReaderPictureDictionaryEnabled
- Value type: REG_DWORD

#### Example value

```
0x00000001
```


## Mac information and settings

- Preference Key name: ImmersiveReaderPictureDictionaryEnabled
- Example value:

```xml
<true/>
```

## See also
- [Microsoft Edge - Policies](../microsoft-edge-policies.md)
