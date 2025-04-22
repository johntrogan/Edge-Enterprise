---
title: "Microsoft Edge Browser Policy Documentation TabCaptureAllowedByOrigins"
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
description: "Windows and Mac documentation for supported Microsoft Edge Browser policy: Allow Tab capture by these origins"
---

# TabCaptureAllowedByOrigins

## Allow Tab capture by these origins


## Supported versions

- On Windows and macOS since 97 or later

## Description

Setting the policy lets you set a list of URL patterns that can use Tab Capture.

Leaving the policy unset means that sites will not be considered for an override at this scope of capture.

This policy is not considered if a site matches a URL pattern in the [SameOriginTabCaptureAllowedByOrigins](SameOriginTabCaptureAllowedByOrigins.md) policy.

If a site matches a URL pattern in this policy, the following policies will not be considered: [WindowCaptureAllowedByOrigins](WindowCaptureAllowedByOrigins.md), [ScreenCaptureAllowedByOrigins](ScreenCaptureAllowedByOrigins.md), [ScreenCaptureAllowed](ScreenCaptureAllowed.md).

For detailed information on valid url patterns, please see [https://go.microsoft.com/fwlink/?linkid=2095322](https://go.microsoft.com/fwlink/?linkid=2095322).  This policy only matches based on origin, so any path in the URL pattern is ignored.

## Supported features

- Can be mandatory: No
- Can be recommended: No
- Dynamic Policy Refresh: Yes
- Per Profile: Yes
- Applies to a profile that is signed in with a Microsoft account: No

## Data type

- List of strings

## Windows information and settings

### Group Policy (ADMX) info

- GP unique name: TabCaptureAllowedByOrigins
- GP name: Allow Tab capture by these origins
- GP path (Mandatory): N/A
- GP path (Recommended): N/A
- GP ADMX file name: MSEdge.admx

#### Example value

Show...

```
https://www.example.com
```

```
[*.]example.edu
```

### Registry settings

- Path (Mandatory): N/A
- Path (Recommended): N/A
- Value name: 1, 2, 3
- Value type: List of REG_SZ

#### Example value

SOFTWARE\Policies\Microsoft\Edge\TabCaptureAllowedByOrigins\0 =
```
https://www.example.com
```

SOFTWARE\Policies\Microsoft\Edge\TabCaptureAllowedByOrigins\1 =
```
[*.]example.edu
```




## Mac information and settings

- Preference Key name: TabCaptureAllowedByOrigins
- Example value:

```xml
<array>
  <string>https://www.example.com</string>
  <string>[*.]example.edu</string>
</array>
```

## See also
- [Microsoft Edge - Policies](../microsoft-edge-policies.md)
