---
title: "Microsoft Edge Browser Policy Documentation PromotionalTabsEnabled"
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
description: "Windows and Mac documentation for supported Microsoft Edge Browser policy: Enable full-tab promotional content (deprecated)"
---

# PromotionalTabsEnabled

## Enable full-tab promotional content (deprecated)
> This policy is deprecated. It is currently supported but will become obsolete in a future release.

## Supported versions

- On Windows and macOS since 77 or later

## Description

Control the presentation of full-tab promotional or educational content. This setting controls the presentation of welcome pages that help users sign into Microsoft Edge, choose their default browser, or learn about product features.

If you enable this policy (set it true) or don't configure it, Microsoft Edge can show full-tab content to users to provide product information.

If you disable (set to false) this policy, Microsoft Edge can't show full-tab content to users.

This is deprecated - use ShowRecommendationsEnabled instead.

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

- GP unique name: PromotionalTabsEnabled
- GP name: Enable full-tab promotional content (deprecated)
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
- Value name: PromotionalTabsEnabled
- Value type: REG_DWORD

#### Example value

```
0x00000000
```


## Mac information and settings

- Preference Key name: PromotionalTabsEnabled
- Example value:

```xml
<false/>
```

## See also
- [Microsoft Edge - Policies](../microsoft-edge-policies.md)
