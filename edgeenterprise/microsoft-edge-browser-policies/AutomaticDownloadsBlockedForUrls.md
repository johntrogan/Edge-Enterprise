---
title: "Microsoft Edge Browser Policy Documentation AutomaticDownloadsBlockedForUrls"
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
description: "Windows and Mac documentation for supported Microsoft Edge Browser policy: Block multiple automatic downloads in quick succession on specific sites"
---

# AutomaticDownloadsBlockedForUrls

## Block multiple automatic downloads in quick succession on specific sites


## Supported versions

- On Windows and macOS since 110 or later

## Description

Define a list of sites, based on URL patterns, where multiple successive automatic downloads aren't allowed.
If you don't configure this policy, [DefaultAutomaticDownloadsSetting](DefaultAutomaticDownloadsSetting.md) applies for all sites, if it's set.  If it isn't set, then the user's personal setting applies.
For more detailed information about valid URL patterns, see [https://go.microsoft.com/fwlink/?linkid=2095322](https://go.microsoft.com/fwlink/?linkid=2095322).

## Supported features

- Can be mandatory: No
- Can be recommended: No
- Dynamic Policy Refresh: Yes
- Per Profile: Yes
- Applies to a profile that is signed in with a Microsoft account: Yes

## Data type

- List of strings

## Windows information and settings

### Group Policy (ADMX) info

- GP unique name: AutomaticDownloadsBlockedForUrls
- GP name: Block multiple automatic downloads in quick succession on specific sites
- GP path (Mandatory): N/A
- GP path (Recommended): N/A
- GP ADMX file name: MSEdge.admx

#### Example value

Show...

```
https://contoso.com
```

```
[*.]contoso.com
```

### Registry settings

- Path (Mandatory): N/A
- Path (Recommended): N/A
- Value name: 1, 2, 3
- Value type: List of REG_SZ

#### Example value

SOFTWARE\Policies\Microsoft\Edge\AutomaticDownloadsBlockedForUrls\0 =
```
https://contoso.com
```

SOFTWARE\Policies\Microsoft\Edge\AutomaticDownloadsBlockedForUrls\1 =
```
[*.]contoso.com
```




## Mac information and settings

- Preference Key name: AutomaticDownloadsBlockedForUrls
- Example value:

```xml
<array>
  <string>https://contoso.com</string>
  <string>[*.]contoso.com</string>
</array>
```

## See also
- [Microsoft Edge - Policies](../microsoft-edge-policies.md)
