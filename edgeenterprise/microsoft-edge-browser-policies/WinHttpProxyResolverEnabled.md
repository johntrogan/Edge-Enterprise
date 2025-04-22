---
title: "Microsoft Edge Browser Policy Documentation WinHttpProxyResolverEnabled"
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
description: "Windows and Mac documentation for supported Microsoft Edge Browser policy: Use Windows proxy resolver"
---

# WinHttpProxyResolverEnabled

## Use Windows proxy resolver


## Supported versions

- On Windows since 84 or later

## Description

This policy will be superseded by a similar feature in a future release. For more information, see https://crbug.com/1032820.

Use Windows to resolve proxies for all browser networking instead of the proxy resolver built into Microsoft Edge. The Windows proxy resolver enables Windows proxy features such as DirectAccess/NRPT.

This policy comes with the problems described by https://crbug.com/644030. It causes PAC files to be fetched and executed by Windows code, including PAC files set via the [ProxyPacUrl](ProxyPacUrl.md) policy. Since Network Fetches for the PAC file happen via Windows instead of Microsoft Edge code, network policies such as [DnsOverHttpsMode](DnsOverHttpsMode.md) will not apply to network fetches for a PAC file.

If you enable this policy, the Windows proxy resolver will be used.

If you disable or don't configure this policy, the Microsoft Edge proxy resolver will be used.

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

- GP unique name: WinHttpProxyResolverEnabled
- GP name: Use Windows proxy resolver
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
- Value name: WinHttpProxyResolverEnabled
- Value type: REG_DWORD

#### Example value

```
0x00000001
```


## See also
- [Microsoft Edge - Policies](../microsoft-edge-policies.md)
