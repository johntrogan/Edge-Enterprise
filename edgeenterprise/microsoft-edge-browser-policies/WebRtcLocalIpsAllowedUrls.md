---
title: "Microsoft Edge Browser Policy Documentation WebRtcLocalIpsAllowedUrls"
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
description: "Windows and Mac documentation for supported Microsoft Edge Browser policy: Manage exposure of local IP addressess by WebRTC"
---

# WebRtcLocalIpsAllowedUrls

## Manage exposure of local IP addressess by WebRTC


## Supported versions

- On Windows and macOS since 80 or later

## Description

Specifies a list of origins (URLs) or hostname patterns (like "*contoso.com*") for which local IP address should be exposed by WebRTC.

If you enable this policy and set a list of origins (URLs) or hostname patterns, when edge://flags/#enable-webrtc-hide-local-ips-with-mdns is Enabled, WebRTC will expose the local IP address for cases that match patterns in the list.

If you disable or don't configure this policy, and edge://flags/#enable-webrtc-hide-local-ips-with-mdns is Enabled, WebRTC will not expose local IP addresses. The local IP address is concealed with an mDNS hostname.

If you enable, disable, or don't configure this policy, and edge://flags/#enable-webrtc-hide-local-ips-with-mdns is Disabled, WebRTC will expose local IP addresses.

Please note that this policy weakens the protection of local IP addresses that might be needed by administrators.

## Supported features

- Can be mandatory: No
- Can be recommended: No
- Dynamic Policy Refresh: No - Requires browser restart
- Per Profile: Yes
- Applies to a profile that is signed in with a Microsoft account: No

## Data type

- List of strings

## Windows information and settings

### Group Policy (ADMX) info

- GP unique name: WebRtcLocalIpsAllowedUrls
- GP name: Manage exposure of local IP addressess by WebRTC
- GP path (Mandatory): N/A
- GP path (Recommended): N/A
- GP ADMX file name: MSEdge.admx

#### Example value

Show...

```
https://www.contoso.com
```

```
*contoso.com*
```

### Registry settings

- Path (Mandatory): N/A
- Path (Recommended): N/A
- Value name: 1, 2, 3
- Value type: List of REG_SZ

#### Example value

SOFTWARE\Policies\Microsoft\Edge\WebRtcLocalIpsAllowedUrls\0 =
```
https://www.contoso.com
```

SOFTWARE\Policies\Microsoft\Edge\WebRtcLocalIpsAllowedUrls\1 =
```
*contoso.com*
```




## Mac information and settings

- Preference Key name: WebRtcLocalIpsAllowedUrls
- Example value:

```xml
<array>
  <string>https://www.contoso.com</string>
  <string>*contoso.com*</string>
</array>
```

## See also
- [Microsoft Edge - Policies](../microsoft-edge-policies.md)
