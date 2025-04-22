---
title: "Microsoft Edge Browser Policy Documentation Edge3PSerpTelemetryEnabled"
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
description: "Windows and Mac documentation for supported Microsoft Edge Browser policy: Edge 3P SERP Telemetry Enabled"
---

# Edge3PSerpTelemetryEnabled

## Edge 3P SERP Telemetry Enabled


## Supported versions

- On Windows since 120 or later

## Description

Edge3P Telemetry in Microsoft Edge captures the searches user does on third party search providers without identifying the person or the device and captures only if the user has consented to this collection of data. User can turn off the collection at any time in the browser settings.

If you enable or don't configure this policy, Edge 3P SERP Telemetry feature will be enabled.

If you disable this policy, Edge 3P SERP Telemetry feature will be disabled.

## Supported features

- Can be mandatory: No
- Can be recommended: Yes
- Dynamic Policy Refresh: Yes
- Per Profile: No
- Applies to a profile that is signed in with a Microsoft account: Yes

## Data type

- Boolean

## Windows information and settings

### Group Policy (ADMX) info

- GP unique name: Edge3PSerpTelemetryEnabled
- GP name: Edge 3P SERP Telemetry Enabled
- GP path (Mandatory): N/A
- GP path (Recommended): Administrative Templates/Microsoft Edge - Default Settings (users can override)
- GP ADMX file name: MSEdge.admx

#### Example value

```
Enabled
```

### Registry settings

- Path (Mandatory): N/A
- Path (Recommended): SOFTWARE\Policies\Microsoft\Edge\Recommended
- Value name: Edge3PSerpTelemetryEnabled
- Value type: REG_DWORD

#### Example value

```
0x00000001
```


## See also
- [Microsoft Edge - Policies](../microsoft-edge-policies.md)
