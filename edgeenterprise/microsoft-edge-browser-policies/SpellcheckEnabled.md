---
title: "Microsoft Edge Browser Policy Documentation SpellcheckEnabled"
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
description: "Windows and Mac documentation for supported Microsoft Edge Browser policy: Enable spellcheck"
---

# SpellcheckEnabled

## Enable spellcheck


## Supported versions

- On Windows and macOS since 77 or later

## Description

If you enable or don't configure this policy, the user can use spellcheck.

If you disable this policy, the user can't use spellcheck and the [SpellcheckLanguage](SpellcheckLanguage.md) and [SpellcheckLanguageBlocklist](SpellcheckLanguageBlocklist.md) policies are also disabled.

## Supported features

- Can be mandatory: No
- Can be recommended: No
- Dynamic Policy Refresh: Yes
- Per Profile: Yes
- Applies to a profile that is signed in with a Microsoft account: No

## Data type

- Boolean

## Windows information and settings

### Group Policy (ADMX) info

- GP unique name: SpellcheckEnabled
- GP name: Enable spellcheck
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
- Value name: SpellcheckEnabled
- Value type: REG_DWORD

#### Example value

```
0x00000000
```


## Mac information and settings

- Preference Key name: SpellcheckEnabled
- Example value:

```xml
<false/>
```

## See also
- [Microsoft Edge - Policies](../microsoft-edge-policies.md)
