---
title: "Microsoft Edge Browser Policy Documentation SpellcheckLanguage"
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
description: "Windows and Mac documentation for supported Microsoft Edge Browser policy: Enable specific spellcheck languages"
---

# SpellcheckLanguage

## Enable specific spellcheck languages


## Supported versions

- On Windows since 77 or later

## Description

Enables different languages for spellcheck. Any language that you specify that isn't recognized is ignored.

If you enable this policy, spellcheck is enabled for the languages specified, as well as any languages the user has enabled.

If you don't configure or disable this policy, there's no change to the user's spellcheck preferences.

If the [SpellcheckEnabled](SpellcheckEnabled.md) policy is disabled, this policy will have no effect.

If a language is included in both the 'SpellcheckLanguage' and the [SpellcheckLanguageBlocklist](SpellcheckLanguageBlocklist.md) policy, the spellcheck language is enabled.

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

- GP unique name: SpellcheckLanguage
- GP name: Enable specific spellcheck languages
- GP path (Mandatory): N/A
- GP path (Recommended): N/A
- GP ADMX file name: MSEdge.admx

#### Example value

Show...

```
fr
```

```
es
```

### Registry settings

- Path (Mandatory): N/A
- Path (Recommended): N/A
- Value name: 1, 2, 3
- Value type: List of REG_SZ

#### Example value

SOFTWARE\Policies\Microsoft\Edge\SpellcheckLanguage\0 =
```
fr
```

SOFTWARE\Policies\Microsoft\Edge\SpellcheckLanguage\1 =
```
es
```




## See also
- [Microsoft Edge - Policies](../microsoft-edge-policies.md)
