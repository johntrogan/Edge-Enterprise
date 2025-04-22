---
title: "Microsoft Edge Browser Policy Documentation ExtensionInstallTypeBlocklist"
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
description: "Windows and Mac documentation for supported Microsoft Edge Browser policy: Blocklist for extension install types"
---

# ExtensionInstallTypeBlocklist

## Blocklist for extension install types


## Supported versions

- On Windows and macOS since 123 or later

## Description

The blocklist controls which extension install types are disallowed.

Setting the "command_line" will block an extension from being loaded from command line.

Policy options mapping:

* command_line (command_line) = Blocks extensions from being loaded from command line

Use the preceding information when configuring this policy.

## Policy options mapping:
> Use this information when configuring this policy.

- command_line = Blocks extensions from being loaded from command line

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

- GP unique name: ExtensionInstallTypeBlocklist
- GP name: Blocklist for extension install types
- GP path (Mandatory): N/A
- GP path (Recommended): N/A
- GP ADMX file name: MSEdge.admx

#### Example value

Show...

```
Blocks extensions from being loaded from command line
```

### Registry settings

- Path (Mandatory): N/A
- Path (Recommended): N/A
- Value name: 1, 2, 3
- Value type: List of REG_SZ

#### Example value

SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallTypeBlocklist\0 =
```
command_line
```




## Mac information and settings

- Preference Key name: ExtensionInstallTypeBlocklist
- Example value:

```xml
<array>
  <string>command_line</string>
</array>
```

## See also
- [Microsoft Edge - Policies](../microsoft-edge-policies.md)
