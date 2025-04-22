---
title: "Microsoft Edge Browser Policy Documentation EnableAuthNegotiatePort"
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
description: "Windows and Mac documentation for supported Microsoft Edge Browser policy: Include non-standard port in Kerberos SPN"
---

# EnableAuthNegotiatePort

## Include non-standard port in Kerberos SPN


## Supported versions

- On Windows and macOS since 77 or later

## Description

Specifies whether the generated Kerberos SPN should include a non-standard port.

If you enable this policy, and a user includes a non-standard port (a port other than 80 or 443) in a URL, that port is included in the generated Kerberos SPN.

If you don't configure or disable this policy, the generated Kerberos SPN won't include a port in any case.

## Supported features

- Can be mandatory: No
- Can be recommended: No
- Dynamic Policy Refresh: No - Requires browser restart
- Per Profile: No
- Applies to a profile that is signed in with a Microsoft account: Yes

## Data type

- Boolean

## Windows information and settings

### Group Policy (ADMX) info

- GP unique name: EnableAuthNegotiatePort
- GP name: Include non-standard port in Kerberos SPN
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
- Value name: EnableAuthNegotiatePort
- Value type: REG_DWORD

#### Example value

```
0x00000000
```


## Mac information and settings

- Preference Key name: EnableAuthNegotiatePort
- Example value:

```xml
<false/>
```

## See also
- [Microsoft Edge - Policies](../microsoft-edge-policies.md)
