---
title: "Microsoft Edge Browser Policy Documentation InternetExplorerIntegrationLocalFileAllowed"
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
description: "Windows and Mac documentation for supported Microsoft Edge Browser policy: Allow launching of local files in Internet Explorer mode"
---

# InternetExplorerIntegrationLocalFileAllowed

## Allow launching of local files in Internet Explorer mode


## Supported versions

- On Windows since 88 or later

## Description

This policy controls the availability of the --ie-mode-file-url command line argument which is used to launch Microsoft Edge with a local file specified on the command line into Internet Explorer mode.

This setting works in conjunction with:
[InternetExplorerIntegrationLevel](InternetExplorerIntegrationLevel.md) is set to 'IEMode'.

If you set this policy to true, or don't configure it, the user is allowed to use the --ie-mode-file-url command line argument for launching local files in Internet Explorer mode.

If you set this policy to false, the user isn't allowed to use the --ie-mode-file-url command line argument for launching local files in Internet Explorer mode.

To learn more about Internet Explorer mode, see [https://go.microsoft.com/fwlink/?linkid=2094210](https://go.microsoft.com/fwlink/?linkid=2094210)

## Supported features

- Can be mandatory: No
- Can be recommended: No
- Dynamic Policy Refresh: Yes
- Per Profile: Yes
- Applies to a profile that is signed in with a Microsoft account: Yes

## Data type

- Boolean

## Windows information and settings

### Group Policy (ADMX) info

- GP unique name: InternetExplorerIntegrationLocalFileAllowed
- GP name: Allow launching of local files in Internet Explorer mode
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
- Value name: InternetExplorerIntegrationLocalFileAllowed
- Value type: REG_DWORD

#### Example value

```
0x00000001
```


## See also
- [Microsoft Edge - Policies](../microsoft-edge-policies.md)
