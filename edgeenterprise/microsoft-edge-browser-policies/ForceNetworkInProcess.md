---
title: "Microsoft Edge Browser Policy Documentation ForceNetworkInProcess"
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
description: "Windows and Mac documentation for supported Microsoft Edge Browser policy: Force networking code to run in the browser process (obsolete)"
---

# ForceNetworkInProcess

## Force networking code to run in the browser process (obsolete)
> OBSOLETE: This policy is obsolete and doesn't work after Microsoft Edge 83.

## Supported versions

- On Windows since 78, until 83

## Description

This policy doesn't work because it was only intended to be a short-term mechanism to give enterprises more time to migrate to 3rd party software that doesn't depend on hooking networking APIs. Proxy servers are recommended over LSPs and Win32 API patching.

This policy forces networking code to run in the browser process.

This policy is disabled by default. If enabled, users are open to security issues when the networking process is sandboxed.

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

- GP unique name: ForceNetworkInProcess
- GP name: Force networking code to run in the browser process (obsolete)
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
- Value name: ForceNetworkInProcess
- Value type: REG_DWORD

#### Example value

```
0x00000000
```


## See also
- [Microsoft Edge - Policies](../microsoft-edge-policies.md)
