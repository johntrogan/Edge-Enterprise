---
title: "Microsoft Edge Browser Policy Documentation SerialAllowAllPortsForUrls"
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
description: "Windows and Mac documentation for supported Microsoft Edge Browser policy: Automatically grant sites permission to connect all serial ports"
---

# SerialAllowAllPortsForUrls

## Automatically grant sites permission to connect all serial ports


## Supported versions

- On Windows and macOS since 97 or later

## Description

Setting the policy allows you to list sites which are automatically granted permission to access all available serial ports.

The URLs must be valid, or the policy is ignored. Only the origin (scheme, host, and port) of the URL is considered.

This policy overrides [DefaultSerialGuardSetting](DefaultSerialGuardSetting.md), [SerialAskForUrls](SerialAskForUrls.md), [SerialBlockedForUrls](SerialBlockedForUrls.md) and the user's preferences.

## Supported features

- Can be mandatory: No
- Can be recommended: No
- Dynamic Policy Refresh: Yes
- Per Profile: No
- Applies to a profile that is signed in with a Microsoft account: Yes

## Data type

- List of strings

## Windows information and settings

### Group Policy (ADMX) info

- GP unique name: SerialAllowAllPortsForUrls
- GP name: Automatically grant sites permission to connect all serial ports
- GP path (Mandatory): N/A
- GP path (Recommended): N/A
- GP ADMX file name: MSEdge.admx

#### Example value

Show...

```
https://www.example.com
```

### Registry settings

- Path (Mandatory): N/A
- Path (Recommended): N/A
- Value name: 1, 2, 3
- Value type: List of REG_SZ

#### Example value

SOFTWARE\Policies\Microsoft\Edge\SerialAllowAllPortsForUrls\0 =
```
https://www.example.com
```




## Mac information and settings

- Preference Key name: SerialAllowAllPortsForUrls
- Example value:

```xml
<array>
  <string>https://www.example.com</string>
</array>
```

## See also
- [Microsoft Edge - Policies](../microsoft-edge-policies.md)
