---
title: "Microsoft Edge Browser Policy Documentation RegisteredProtocolHandlers"
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
description: "Windows and Mac documentation for supported Microsoft Edge Browser policy: Register protocol handlers"
---

# RegisteredProtocolHandlers

## Register protocol handlers


## Supported versions

- On Windows and macOS since 77 or later

## Description

Set this policy (recommended only) to register a list of protocol handlers. This list is merged with ones registered by the user and both are available to use.

To register a protocol handler:

- Set the protocol property to the scheme (for example, "mailto")
- Set the URL property to the URL property of the application that handlers the scheme specified in the "protocol" field. The pattern can include a "%s" placeholder, which the handled URL replaces.

Users can't remove a protocol handler registered by this policy. However, they can install a new default protocol handler to override the existing protocol handlers.

## Supported features

- Can be mandatory: No
- Can be recommended: Yes
- Dynamic Policy Refresh: No - Requires browser restart
- Per Profile: Yes
- Applies to a profile that is signed in with a Microsoft account: No

## Data type

- Dictionary

## Windows information and settings

### Group Policy (ADMX) info

- GP unique name: RegisteredProtocolHandlers
- GP name: Register protocol handlers
- GP path (Mandatory): N/A
- GP path (Recommended): Administrative Templates/Microsoft Edge - Default Settings (users can override)/Content settings
- GP ADMX file name: MSEdge.admx

#### Example value

```
[{"default": true, "protocol": "mailto", "url": "https://mail.contoso.com/mail/?extsrc=mailto&url=%s"}]
```

### Registry settings

- Path (Mandatory): N/A
- Path (Recommended): SOFTWARE\Policies\Microsoft\Edge\Recommended
- Value name: RegisteredProtocolHandlers
- Value type: REG_SZ

#### Example value

```
[{"default": true, "protocol": "mailto", "url": "https://mail.contoso.com/mail/?extsrc=mailto&url=%s"}]
```


#### Expanded example value

```
[
  {
    "default": true,
    "protocol": "mailto",
    "url": "https://mail.contoso.com/mail/?extsrc=mailto&url=%s"
  }
]
```

## Mac information and settings

- Preference Key name: RegisteredProtocolHandlers
- Example value:

```xml
<key>RegisteredProtocolHandlers</key>
<array>
  <dict>
    <key>default</key>
    <true/>
    <key>protocol</key>
    <string>mailto</string>
    <key>url</key>
    <string>https://mail.contoso.com/mail/?extsrc=mailto&url=%s</string>
  </dict>
</array>
```

## See also
- [Microsoft Edge - Policies](../microsoft-edge-policies.md)
