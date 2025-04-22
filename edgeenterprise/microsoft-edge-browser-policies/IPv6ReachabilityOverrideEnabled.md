---
title: "Microsoft Edge Browser Policy Documentation IPv6ReachabilityOverrideEnabled"
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
description: "Windows and Mac documentation for supported Microsoft Edge Browser policy: Enable IPv6 reachability check override"
---

# IPv6ReachabilityOverrideEnabled

## Enable IPv6 reachability check override


## Supported versions

- On Windows and macOS since 132 or later

## Description

This policy enables an override of the IPv6 reachability check. When overridden, the
system will always query AAAA records when resolving host names. It applies to
all users and interfaces on the device.

If you enable this policy, the IPv6 reachability check will be overridden.

If you disable or don't configure this policy, the IPv6 reachability check will not be overridden.
The system only queries AAAA records when it is reachable to a global IPv6 host.

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

- GP unique name: IPv6ReachabilityOverrideEnabled
- GP name: Enable IPv6 reachability check override
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
- Value name: IPv6ReachabilityOverrideEnabled
- Value type: REG_DWORD

#### Example value

```
0x00000001
```


## Mac information and settings

- Preference Key name: IPv6ReachabilityOverrideEnabled
- Example value:

```xml
<true/>
```

## See also
- [Microsoft Edge - Policies](../microsoft-edge-policies.md)
