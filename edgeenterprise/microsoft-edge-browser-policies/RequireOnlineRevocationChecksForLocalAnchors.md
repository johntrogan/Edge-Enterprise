---
title: "Microsoft Edge Browser Policy Documentation RequireOnlineRevocationChecksForLocalAnchors"
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
description: "Windows and Mac documentation for supported Microsoft Edge Browser policy: Specify if online OCSP/CRL checks are required for local trust anchors"
---

# RequireOnlineRevocationChecksForLocalAnchors

## Specify if online OCSP/CRL checks are required for local trust anchors


## Supported versions

- On Windows since 123 or later

## Description

Control whether online revocation checks (OCSP/CRL checks) are required. If Microsoft Edge can't get revocation status information, these certificates are treated as revoked ("hard-fail").

If you enable this policy, Microsoft Edge always performs revocation checking for server certificates that successfully validate and are signed by locally-installed CA certificates.

If you don't configure or disable this policy, then Microsoft Edge uses the existing online revocation checking settings.

On macOS, this policy has no effect if the [MicrosoftRootStoreEnabled](MicrosoftRootStoreEnabled.md) policy is set to False.

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

- GP unique name: RequireOnlineRevocationChecksForLocalAnchors
- GP name: Specify if online OCSP/CRL checks are required for local trust anchors
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
- Value name: RequireOnlineRevocationChecksForLocalAnchors
- Value type: REG_DWORD

#### Example value

```
0x00000000
```


## See also
- [Microsoft Edge - Policies](../microsoft-edge-policies.md)
