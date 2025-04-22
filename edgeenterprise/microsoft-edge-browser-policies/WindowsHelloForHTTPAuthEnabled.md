---
title: "Microsoft Edge Browser Policy Documentation WindowsHelloForHTTPAuthEnabled"
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
description: "Windows and Mac documentation for supported Microsoft Edge Browser policy: Windows Hello For HTTP Auth Enabled"
---

# WindowsHelloForHTTPAuthEnabled

## Windows Hello For HTTP Auth Enabled


## Supported versions

- On Windows since 90 or later

## Description

Indicates if Windows Credential UI should be used to respond to NTLM and Negotiate authentication challenges.

If you disable this policy, a basic username and password prompt will be used to respond to NTLM and Negotiate challenges. If you enable or don't configure this policy, Windows Credential UI will be used.

## Supported features

- Can be mandatory: No
- Can be recommended: Yes
- Dynamic Policy Refresh: No - Requires browser restart
- Per Profile: No
- Applies to a profile that is signed in with a Microsoft account: Yes

## Data type

- Boolean

## Windows information and settings

### Group Policy (ADMX) info

- GP unique name: WindowsHelloForHTTPAuthEnabled
- GP name: Windows Hello For HTTP Auth Enabled
- GP path (Mandatory): N/A
- GP path (Recommended): Administrative Templates/Microsoft Edge - Default Settings (users can override)/HTTP authentication
- GP ADMX file name: MSEdge.admx

#### Example value

```
Enabled
```

### Registry settings

- Path (Mandatory): N/A
- Path (Recommended): SOFTWARE\Policies\Microsoft\Edge\Recommended
- Value name: WindowsHelloForHTTPAuthEnabled
- Value type: REG_DWORD

#### Example value

```
0x00000001
```


## See also
- [Microsoft Edge - Policies](../microsoft-edge-policies.md)
