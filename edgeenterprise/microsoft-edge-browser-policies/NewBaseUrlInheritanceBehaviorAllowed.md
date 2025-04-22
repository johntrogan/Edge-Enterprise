---
title: "Microsoft Edge Browser Policy Documentation NewBaseUrlInheritanceBehaviorAllowed"
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
description: "Windows and Mac documentation for supported Microsoft Edge Browser policy: Allows enabling the feature NewBaseUrlInheritanceBehavior (obsolete)"
---

# NewBaseUrlInheritanceBehaviorAllowed

## Allows enabling the feature NewBaseUrlInheritanceBehavior (obsolete)
> OBSOLETE: This policy is obsolete and doesn't work after Microsoft Edge 135.

## Supported versions

- On Windows and macOS since 123, until 135

## Description

NewBaseUrlInheritanceBehavior is a Microsoft Edge feature that causes about:blank and about:srcdoc frames to consistently inherit their base url values via snapshots of their initiator's base url.

If you disable this policy, it prevents users or Microsoft Edge variations from enabling NewBaseUrlInheritanceBehavior, in case compatibility issues are discovered.

If you enable or don't configure this policy, it allows enabling NewBaseUrlInheritanceBehavior.

The policy has been obsoleted starting from Microsoft Edge version 136, but the NewBaseUrlInheritanceBehaviorAllowed feature was removed in Microsoft Edge version 123.

## Supported features

- Can be mandatory: No
- Can be recommended: No
- Dynamic Policy Refresh: Yes
- Per Profile: No
- Applies to a profile that is signed in with a Microsoft account: Yes

## Data type

- Boolean

## Windows information and settings

### Group Policy (ADMX) info

- GP unique name: NewBaseUrlInheritanceBehaviorAllowed
- GP name: Allows enabling the feature NewBaseUrlInheritanceBehavior (obsolete)
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
- Value name: NewBaseUrlInheritanceBehaviorAllowed
- Value type: REG_DWORD

#### Example value

```
0x00000001
```


## Mac information and settings

- Preference Key name: NewBaseUrlInheritanceBehaviorAllowed
- Example value:

```xml
<true/>
```

## See also
- [Microsoft Edge - Policies](../microsoft-edge-policies.md)
