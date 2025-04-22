---
title: "Microsoft Edge Browser Policy Documentation SendSiteInfoToImproveServices"
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
description: "Windows and Mac documentation for supported Microsoft Edge Browser policy: Send site information to improve Microsoft services (obsolete)"
---

# SendSiteInfoToImproveServices

## Send site information to improve Microsoft services (obsolete)
> OBSOLETE: This policy is obsolete and doesn't work after Microsoft Edge 88.

## Supported versions

- On Windows and macOS since 77, until 88

## Description

This policy is no longer supported. It is replaced by [DiagnosticData](DiagnosticData.md) (for Windows 7, Windows 8, and macOS) and Allow Telemetry on Win 10 ([[https://go.microsoft.com/fwlink/?linkid=2099569](https://go.microsoft.com/fwlink/?linkid=2099569)]([https://go.microsoft.com/fwlink/?linkid=2099569](https://go.microsoft.com/fwlink/?linkid=2099569))).

This policy enables sending info about websites visited in Microsoft Edge to Microsoft to improve services like search.

Enable this policy to send info about websites visited in Microsoft Edge to Microsoft. Disable this policy to not send info about websites visited in Microsoft Edge to Microsoft. In both cases, users can't change or override the setting.

On Windows 10, if you don't configure this policy, Microsoft Edge will default to the Windows diagnostic data setting. If this policy is enabled Microsoft Edge will only send info about websites visited in Microsoft Edge if the Windows Diagnostic data setting is set to Full. If this policy is disabled Microsoft Edge will not send info about websites visited. Learn more about Windows Diagnostic data settings: [[https://go.microsoft.com/fwlink/?linkid=2099569](https://go.microsoft.com/fwlink/?linkid=2099569)]([https://go.microsoft.com/fwlink/?linkid=2099569](https://go.microsoft.com/fwlink/?linkid=2099569))

On Windows 7, windows 8, and macOS this policy controls sending info about websites visited. If you don't configure this policy, Microsoft Edge will default to the user's preference.

To enable this policy, [MetricsReportingEnabled](MetricsReportingEnabled.md) must be set to Enabled. If [SendSiteInfoToImproveServices](SendSiteInfoToImproveServices.md) or [MetricsReportingEnabled](MetricsReportingEnabled.md) is Not Configured or Disabled, this data will not be sent to Microsoft.

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

- GP unique name: SendSiteInfoToImproveServices
- GP name: Send site information to improve Microsoft services (obsolete)
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
- Value name: SendSiteInfoToImproveServices
- Value type: REG_DWORD

#### Example value

```
0x00000000
```


## Mac information and settings

- Preference Key name: SendSiteInfoToImproveServices
- Example value:

```xml
<false/>
```

## See also
- [Microsoft Edge - Policies](../microsoft-edge-policies.md)
