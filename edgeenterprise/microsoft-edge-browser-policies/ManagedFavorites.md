---
title: "Microsoft Edge Browser Policy Documentation ManagedFavorites"
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
description: "Windows and Mac documentation for supported Microsoft Edge Browser policy: Configure favorites"
---

# ManagedFavorites

## Configure favorites


## Supported versions

- On Windows and macOS since 77 or later

## Description

Configures a list of managed favorites.

The policy creates a list of favorites. Each favorite contains the keys "name" and "url," which hold the favorite's name and its target. You can configure a subfolder by defining a favorites without an "url" key but with an additional "children" key that contains a list of favorites as defined above (some of which may be folders again). Microsoft Edge amends incomplete URLs as if they were submitted via the Address Bar, for example "microsoft.com" becomes "https://microsoft.com/".

These favorites are placed in a folder that can't be modified by the user (but the user can choose to hide it from the favorites bar). By default the folder name is "Managed favorites" but you can change it by adding to the list of favorites a dictionary containing the key "toplevel_name" with the desired folder name as the value.

Managed favorites are not synced to the user account and can't be modified by extensions.

## Supported features

- Can be mandatory: No
- Can be recommended: No
- Dynamic Policy Refresh: Yes
- Per Profile: Yes
- Applies to a profile that is signed in with a Microsoft account: No

## Data type

- Dictionary

## Windows information and settings

### Group Policy (ADMX) info

- GP unique name: ManagedFavorites
- GP name: Configure favorites
- GP path (Mandatory): N/A
- GP path (Recommended): N/A
- GP ADMX file name: MSEdge.admx

#### Example value

```
[{"toplevel_name": "My managed favorites folder"}, {"name": "Microsoft", "url": "microsoft.com"}, {"name": "Bing", "url": "bing.com"}, {"children": [{"name": "Microsoft Edge Insiders", "url": "www.microsoftedgeinsider.com"}, {"name": "Microsoft Edge", "url": "www.microsoft.com/windows/microsoft-edge"}], "name": "Microsoft Edge links"}]
```

### Registry settings

- Path (Mandatory): N/A
- Path (Recommended): N/A
- Value name: ManagedFavorites
- Value type: REG_SZ

#### Example value

```
[{"toplevel_name": "My managed favorites folder"}, {"name": "Microsoft", "url": "microsoft.com"}, {"name": "Bing", "url": "bing.com"}, {"children": [{"name": "Microsoft Edge Insiders", "url": "www.microsoftedgeinsider.com"}, {"name": "Microsoft Edge", "url": "www.microsoft.com/windows/microsoft-edge"}], "name": "Microsoft Edge links"}]
```


#### Expanded example value

```
[
  {
    "toplevel_name": "My managed favorites folder"
  },
  {
    "name": "Microsoft",
    "url": "microsoft.com"
  },
  {
    "name": "Bing",
    "url": "bing.com"
  },
  {
    "children": [
      {
        "name": "Microsoft Edge Insiders",
        "url": "www.microsoftedgeinsider.com"
      },
      {
        "name": "Microsoft Edge",
        "url": "www.microsoft.com/windows/microsoft-edge"
      }
    ],
    "name": "Microsoft Edge links"
  }
]
```

## Mac information and settings

- Preference Key name: ManagedFavorites
- Example value:

```xml
<key>ManagedFavorites</key>
<array>
  <dict>
    <key>toplevel_name</key>
    <string>My managed favorites folder</string>
  </dict>
  <dict>
    <key>name</key>
    <string>Microsoft</string>
    <key>url</key>
    <string>microsoft.com</string>
  </dict>
  <dict>
    <key>name</key>
    <string>Bing</string>
    <key>url</key>
    <string>bing.com</string>
  </dict>
  <dict>
    <key>children</key>
    <array>
      <dict>
        <key>name</key>
        <string>Microsoft Edge Insiders</string>
        <key>url</key>
        <string>www.microsoftedgeinsider.com</string>
      </dict>
      <dict>
        <key>name</key>
        <string>Microsoft Edge</string>
        <key>url</key>
        <string>www.microsoft.com/windows/microsoft-edge</string>
      </dict>
    </array>
    <key>name</key>
    <string>Microsoft Edge links</string>
  </dict>
</array>
```

## See also
- [Microsoft Edge - Policies](../microsoft-edge-policies.md)
