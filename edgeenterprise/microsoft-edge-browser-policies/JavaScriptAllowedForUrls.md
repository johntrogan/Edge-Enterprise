---
title: "Microsoft Edge Browser Policy Documentation JavaScriptAllowedForUrls"
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
description: "Windows and Mac documentation for supported Microsoft Edge Browser policy: Allow JavaScript on specific sites"
---

# JavaScriptAllowedForUrls

## Allow JavaScript on specific sites


## Supported versions

- On Windows and macOS since 77 or later

## Description

Define a list of sites, based on URL patterns, that are allowed to run JavaScript.

If you don't configure this policy, [DefaultJavaScriptSetting](DefaultJavaScriptSetting.md) applies for all sites, if it's set. If not, the user's personal setting applies.

For detailed information about valid url patterns, please see [https://go.microsoft.com/fwlink/?linkid=2095322](https://go.microsoft.com/fwlink/?linkid=2095322). Wildcards, *, are allowed.

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

- GP unique name: JavaScriptAllowedForUrls
- GP name: Allow JavaScript on specific sites
- GP path (Mandatory): N/A
- GP path (Recommended): N/A
- GP ADMX file name: MSEdge.admx

#### Example value

Show...

```
https://www.contoso.com
```

```
[*.]contoso.edu
```

### Registry settings

- Path (Mandatory): N/A
- Path (Recommended): N/A
- Value name: 1, 2, 3
- Value type: List of REG_SZ

#### Example value

SOFTWARE\Policies\Microsoft\Edge\JavaScriptAllowedForUrls\0 =
```
https://www.contoso.com
```

SOFTWARE\Policies\Microsoft\Edge\JavaScriptAllowedForUrls\1 =
```
[*.]contoso.edu
```




## Mac information and settings

- Preference Key name: JavaScriptAllowedForUrls
- Example value:

```xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```

## See also
- [Microsoft Edge - Policies](../microsoft-edge-policies.md)
