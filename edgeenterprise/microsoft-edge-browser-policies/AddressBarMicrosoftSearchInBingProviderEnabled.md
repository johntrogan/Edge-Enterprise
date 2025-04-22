---
title: "Microsoft Edge Browser Policy Documentation AddressBarMicrosoftSearchInBingProviderEnabled"
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
description: "Windows and Mac documentation for supported Microsoft Edge Browser policy: Enable Microsoft Search in Bing suggestions in the address bar (deprecated)"
---

# AddressBarMicrosoftSearchInBingProviderEnabled

## Enable Microsoft Search in Bing suggestions in the address bar (deprecated)
> This policy is deprecated. It is currently supported but will become obsolete in a future release.

## Supported versions

- On Windows and macOS since 81 or later

## Description

Enables the display of relevant Microsoft Search in Bing suggestions in the address bar's suggestion list when the user enters a search query in the address bar. If you enable or don't configure this policy, users can see internal results powered by Microsoft Search in Bing in the Microsoft Edge address bar suggestion list. To access Microsoft Search in Bing results, the user must be signed into Microsoft Edge with their organization's Azure AD account.

If you disable this policy, users won't see internal results in the Microsoft Edge address bar suggestion list.

Starting with Microsoft Edge version 89, Microsoft Search in Bing suggestions will be available even if Bing is not the user's default search provider.

This policy is deprecated due to changes in access to work search through Bing-related endpoints and will be obsolete in Microsoft Edge version 137. Use the AddressBarWorkSearchResultsEnabled policy instead.

## Supported features

- Can be mandatory: No
- Can be recommended: No
- Dynamic Policy Refresh: No - Requires browser restart
- Per Profile: Yes
- Applies to a profile that is signed in with a Microsoft account: No

## Data type

- Boolean

## Windows information and settings

### Group Policy (ADMX) info

- GP unique name: AddressBarMicrosoftSearchInBingProviderEnabled
- GP name: Enable Microsoft Search in Bing suggestions in the address bar (deprecated)
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
- Value name: AddressBarMicrosoftSearchInBingProviderEnabled
- Value type: REG_DWORD

#### Example value

```
0x00000001
```


## Mac information and settings

- Preference Key name: AddressBarMicrosoftSearchInBingProviderEnabled
- Example value:

```xml
<true/>
```

## See also
- [Microsoft Edge - Policies](../microsoft-edge-policies.md)
