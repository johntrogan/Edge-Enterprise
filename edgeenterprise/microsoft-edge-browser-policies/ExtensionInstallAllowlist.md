---
title: "Microsoft Edge Browser Policy Documentation ExtensionInstallAllowlist"
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
description: "Windows and Mac documentation for supported Microsoft Edge Browser policy: Allow specific extensions to be installed"
---

# ExtensionInstallAllowlist

## Allow specific extensions to be installed


## Supported versions

- On Windows and macOS since 77 or later

## Description

Setting this policy specifies which extensions are not subject to the blocklist.

A blocklist value of * means all extensions are blocked and users can only install extensions listed in the allow list.

By default, all extensions are allowed. However, if you prohibited extensions by policy, you can use the list of allowed extensions to change that policy.

## Supported features

- Can be mandatory: No
- Can be recommended: No
- Dynamic Policy Refresh: Yes
- Per Profile: Yes
- Applies to a profile that is signed in with a Microsoft account: No

## Data type

- List of strings

## Windows information and settings

### Group Policy (ADMX) info

- GP unique name: ExtensionInstallAllowlist
- GP name: Allow specific extensions to be installed
- GP path (Mandatory): N/A
- GP path (Recommended): N/A
- GP ADMX file name: MSEdge.admx

#### Example value

Show...

```
extension_id1
```

```
extension_id2
```

### Registry settings

- Path (Mandatory): N/A
- Path (Recommended): N/A
- Value name: 1, 2, 3
- Value type: List of REG_SZ

#### Example value

SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallAllowlist\0 =
```
extension_id1
```

SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallAllowlist\1 =
```
extension_id2
```




## Mac information and settings

- Preference Key name: ExtensionInstallAllowlist
- Example value:

```xml
<array>
  <string>extension_id1</string>
  <string>extension_id2</string>
</array>
```

## See also
- [Microsoft Edge - Policies](../microsoft-edge-policies.md)
