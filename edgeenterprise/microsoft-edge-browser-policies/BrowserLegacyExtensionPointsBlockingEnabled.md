---
title: "Microsoft Edge Browser Policy Documentation BrowserLegacyExtensionPointsBlockingEnabled"
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
description: "Windows and Mac documentation for supported Microsoft Edge Browser policy: Enable browser legacy extension point blocking"
---

# BrowserLegacyExtensionPointsBlockingEnabled

## Enable browser legacy extension point blocking


## Supported versions

- On Windows since 95 or later

## Description

Sets the ProcessExtensionPointDisablePolicy on Microsoft Edge's browser process to block code injection from legacy third party applications.

If you enable or don't configure this policy, the ProcessExtensionPointDisablePolicy is applied to block legacy extension points in the browser process.

If you disable this policy, the ProcessExtensionPointDisablePolicy is not applied to block legacy extension points in the browser process. This has a detrimental effect on Microsoft Edge's security and stability as unknown and potentially hostile code can load inside Microsoft Edge's browser process. Only turn off the policy if there are compatibility issues with third-party software that must run inside Microsoft Edge's browser process.

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

- GP unique name: BrowserLegacyExtensionPointsBlockingEnabled
- GP name: Enable browser legacy extension point blocking
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
- Value name: BrowserLegacyExtensionPointsBlockingEnabled
- Value type: REG_DWORD

#### Example value

```
0x00000000
```


## See also
- [Microsoft Edge - Policies](../microsoft-edge-policies.md)
