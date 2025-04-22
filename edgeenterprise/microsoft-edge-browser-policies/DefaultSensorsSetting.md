---
title: "Microsoft Edge Browser Policy Documentation DefaultSensorsSetting"
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
description: "Windows and Mac documentation for supported Microsoft Edge Browser policy: Default sensors setting"
---

# DefaultSensorsSetting

## Default sensors setting


## Supported versions

- On Windows and macOS since 86 or later

## Description

Set whether websites can access and use sensors such as motion and light sensors. You can completely block or allow websites to get access to sensors.

Setting the policy to 1 lets websites access and use sensors. Setting the policy to 2 denies access to sensors.

You can override this policy for specific URL patterns by using the [SensorsAllowedForUrls](SensorsAllowedForUrls.md) and [SensorsBlockedForUrls](SensorsBlockedForUrls.md) policies.

If you don't configure this policy, websites can access and use sensors, and users can change this setting. This is the global default for [SensorsAllowedForUrls](SensorsAllowedForUrls.md) and [SensorsBlockedForUrls](SensorsBlockedForUrls.md).

Policy options mapping:

* AllowSensors (1) = Allow sites to access sensors

* BlockSensors (2) = Do not allow any site to access sensors

Use the preceding information when configuring this policy.

## Policy options mapping:
> Use this information when configuring this policy.

- AllowSensors (1) = Allow sites to access sensors
- BlockSensors (2) = Do not allow any site to access sensors

## Supported features

- Can be mandatory: No
- Can be recommended: No
- Dynamic Policy Refresh: Yes
- Per Profile: Yes
- Applies to a profile that is signed in with a Microsoft account: Yes

## Data type

- Integer

## Windows information and settings

### Group Policy (ADMX) info

- GP unique name: DefaultSensorsSetting
- GP name: Default sensors setting
- GP path (Mandatory): N/A
- GP path (Recommended): N/A
- GP ADMX file name: MSEdge.admx

#### Example value

```
Do not allow any site to access sensors
```

### Registry settings

- Path (Mandatory): N/A
- Path (Recommended): N/A
- Value name: DefaultSensorsSetting
- Value type: REG_DWORD

#### Example value

```
0x00000002
```


## Mac information and settings

- Preference Key name: DefaultSensorsSetting
- Example value:

```xml
<integer>2</integer>
```

## See also
- [Microsoft Edge - Policies](../microsoft-edge-policies.md)
