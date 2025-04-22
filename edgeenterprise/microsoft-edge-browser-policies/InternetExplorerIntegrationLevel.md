---
title: "Microsoft Edge Browser Policy Documentation InternetExplorerIntegrationLevel"
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
description: "Windows and Mac documentation for supported Microsoft Edge Browser policy: Configure Internet Explorer integration"
---

# InternetExplorerIntegrationLevel

## Configure Internet Explorer integration


## Supported versions

- On Windows since 77 or later

## Description

For guidance about configuring the optimal experience for Internet Explorer mode see [https://go.microsoft.com/fwlink/?linkid=2094210](https://go.microsoft.com/fwlink/?linkid=2094210)

Policy options mapping:

* None (0) = None

* IEMode (1) = Internet Explorer mode

* NeedIE (2) = Internet Explorer 11

Use the preceding information when configuring this policy.

## Policy options mapping:
> Use this information when configuring this policy.

- None (0) = None
- IEMode (1) = Internet Explorer mode
- NeedIE (2) = Internet Explorer 11

## Supported features

- Can be mandatory: No
- Can be recommended: No
- Dynamic Policy Refresh: No - Requires browser restart
- Per Profile: Yes
- Applies to a profile that is signed in with a Microsoft account: Yes

## Data type

- Integer

## Windows information and settings

### Group Policy (ADMX) info

- GP unique name: InternetExplorerIntegrationLevel
- GP name: Configure Internet Explorer integration
- GP path (Mandatory): N/A
- GP path (Recommended): N/A
- GP ADMX file name: MSEdge.admx

#### Example value

```
Internet Explorer mode
```

### Registry settings

- Path (Mandatory): N/A
- Path (Recommended): N/A
- Value name: InternetExplorerIntegrationLevel
- Value type: REG_DWORD

#### Example value

```
0x00000001
```


## See also
- [Microsoft Edge - Policies](../microsoft-edge-policies.md)
