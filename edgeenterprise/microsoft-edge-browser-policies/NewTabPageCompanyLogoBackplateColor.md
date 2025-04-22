---
title: "Microsoft Edge Browser Policy Documentation NewTabPageCompanyLogoBackplateColor"
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
description: "Windows and Mac documentation for supported Microsoft Edge Browser policy: Set the company logo backplate color on the new tab page."
---

# NewTabPageCompanyLogoBackplateColor

## Set the company logo backplate color on the new tab page.


## Supported versions

- On Windows and macOS since 135 or later

## Description

By default, the new tab page sets the company logo backplate color to the neutralStrokeActive (#cecece) constant.

You can configure this policy with a color hex code to change the company logo backplate color on the new tab page.

If this policy is not configured, the default neutralStrokeActive (#cecece) color will be used as the backplate color.

## Supported features

- Can be mandatory: No
- Can be recommended: No
- Dynamic Policy Refresh: Yes
- Per Profile: Yes
- Applies to a profile that is signed in with a Microsoft account: No

## Data type

- String

## Windows information and settings

### Group Policy (ADMX) info

- GP unique name: NewTabPageCompanyLogoBackplateColor
- GP name: Set the company logo backplate color on the new tab page.
- GP path (Mandatory): N/A
- GP path (Recommended): N/A
- GP ADMX file name: MSEdge.admx

#### Example value

```
#cecece
```

### Registry settings

- Path (Mandatory): N/A
- Path (Recommended): N/A
- Value name: NewTabPageCompanyLogoBackplateColor
- Value type: REG_SZ

#### Example value

```
#cecece
```


## Mac information and settings

- Preference Key name: NewTabPageCompanyLogoBackplateColor
- Example value:

```xml
<string>#cecece</string>
```

## See also
- [Microsoft Edge - Policies](../microsoft-edge-policies.md)
