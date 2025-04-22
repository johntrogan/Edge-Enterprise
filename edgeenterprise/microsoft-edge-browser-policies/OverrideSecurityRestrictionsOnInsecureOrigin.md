---
title: "Microsoft Edge Browser Policy Documentation OverrideSecurityRestrictionsOnInsecureOrigin"
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
description: "Windows and Mac documentation for supported Microsoft Edge Browser policy: Control where security restrictions on insecure origins apply"
---

# OverrideSecurityRestrictionsOnInsecureOrigin

## Control where security restrictions on insecure origins apply


## Supported versions

- On Windows and macOS since 77 or later

## Description

Specifies a list of origins (URLs) or hostname patterns (like "*.contoso.com") for which security restrictions on insecure origins don't apply.

This policy allows you to specify permitted origins for legacy applications that cannot deploy TLS or for internal web development staging servers. It enables developers to test features requiring secure contexts without the need to configure TLS on the staging server. Patterns are only accepted for hostnames; URLs or origins with schemes must be exact matches. This policy also prevents the origin from being labeled "Not Secure" in the omnibox.

Setting a list of URLs in this policy has the same effect as setting the command-line flag '--unsafely-treat-insecure-origin-as-secure' to a comma-separated list of the same URLs. If you enable this policy, it overrides the command-line flag.

For more information on secure contexts, see https://www.w3.org/TR/secure-contexts/.

## Supported features

- Can be mandatory: No
- Can be recommended: No
- Dynamic Policy Refresh: No - Requires browser restart
- Per Profile: No
- Applies to a profile that is signed in with a Microsoft account: Yes

## Data type

- List of strings

## Windows information and settings

### Group Policy (ADMX) info

- GP unique name: OverrideSecurityRestrictionsOnInsecureOrigin
- GP name: Control where security restrictions on insecure origins apply
- GP path (Mandatory): N/A
- GP path (Recommended): N/A
- GP ADMX file name: MSEdge.admx

#### Example value

Show...

```
http://testserver.contoso.com/
```

```
*.contoso.com
```

### Registry settings

- Path (Mandatory): N/A
- Path (Recommended): N/A
- Value name: 1, 2, 3
- Value type: List of REG_SZ

#### Example value

SOFTWARE\Policies\Microsoft\Edge\OverrideSecurityRestrictionsOnInsecureOrigin\0 =
```
http://testserver.contoso.com/
```

SOFTWARE\Policies\Microsoft\Edge\OverrideSecurityRestrictionsOnInsecureOrigin\1 =
```
*.contoso.com
```




## Mac information and settings

- Preference Key name: OverrideSecurityRestrictionsOnInsecureOrigin
- Example value:

```xml
<array>
  <string>http://testserver.contoso.com/</string>
  <string>*.contoso.com</string>
</array>
```

## See also
- [Microsoft Edge - Policies](../microsoft-edge-policies.md)
