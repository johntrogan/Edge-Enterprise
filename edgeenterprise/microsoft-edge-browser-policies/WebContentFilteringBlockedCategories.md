---
title: "Microsoft Edge Browser Policy Documentation WebContentFilteringBlockedCategories"
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
description: "Windows and Mac documentation for supported Microsoft Edge Browser policy: Configure Web Content Filtering"
---

# WebContentFilteringBlockedCategories

## Configure Web Content Filtering


## Supported versions

- On Windows since 135 or later

## Description

You can configure this policy to block certain categories of URLs. Blocking a category prevents users in specified device groups from accessing URLs associated with the category.

The list of possible categories, their Category String, and their description are detailed at [https://go.microsoft.com/fwlink/?linkid=2249965](https://go.microsoft.com/fwlink/?linkid=2249965)

To block a category, add the Category String of the category to the following List of blocked categories If you leave this policy unset or disable the policy, no URLs will be blocked.

If you want to block a specific URL without blocking an entire category, add the URL to the list of blocked URLs using the [URLBlocklist](URLBlocklist.md) policy.

If you want a specific URL in a blocked category to be accessible, add the URL to the list of allowed URLs using the [URLAllowlist](URLAllowlist.md) policy.

This Web Content Filtering policy only works on Microsoft Edge on Windows 10 devices or above.

Policy options mapping:

* chat (chat) = Chat

* child_abuse_images (child_abuse_images) = Child Abuse Images

* criminal_activity (criminal_activity) = Criminal Activity

* download_sites (download_sites) = Download Sites

* gambling (gambling) = Gambling

* games (games) = Games

* hacking (hacking) = Hacking

* hate_and_intolerance (hate_and_intolerance) = Hate and Intolerance

* illegal_drug (illegal_drug) = Illegal Drug

* illegal_software (illegal_software) = Illegal Software

* image_sharing (image_sharing) = Image Sharing

* instant_messaging (instant_messaging) = Instant Messaging

* nudity (nudity) = Nudity

* peer_to_peer (peer_to_peer) = Peer to Peer

* pornography_or_sexually_explicit (pornography_or_sexually_explicit) = Pornography or Sexually Explicit

* professional_networking (professional_networking) = Professional Networking

* self_harm (self_harm) = Self Harm

* sex_education (sex_education) = Sex Education

* social_networking (social_networking) = Social Networking

* streaming_and_downloads (streaming_and_downloads) = Streaming Media and Downloads

* tasteless (tasteless) = Tasteless

* violence (violence) = Violence

* weapons (weapons) = Weapons

* web_based_email (web_based_email) = Web Based Email

* none (none) = None

Use the preceding information when configuring this policy.

## Policy options mapping:
> Use this information when configuring this policy.

- chat = Chat
- child_abuse_images = Child Abuse Images
- criminal_activity = Criminal Activity
- download_sites = Download Sites
- gambling = Gambling
- games = Games
- hacking = Hacking
- hate_and_intolerance = Hate and Intolerance
- illegal_drug = Illegal Drug
- illegal_software = Illegal Software
- image_sharing = Image Sharing
- instant_messaging = Instant Messaging
- nudity = Nudity
- peer_to_peer = Peer to Peer
- pornography_or_sexually_explicit = Pornography or Sexually Explicit
- professional_networking = Professional Networking
- self_harm = Self Harm
- sex_education = Sex Education
- social_networking = Social Networking
- streaming_and_downloads = Streaming Media and Downloads
- tasteless = Tasteless
- violence = Violence
- weapons = Weapons
- web_based_email = Web Based Email
- none = None

## Supported features

- Can be mandatory: Yes
- Can be recommended: No
- Dynamic Policy Refresh: Yes
- Per Profile: No
- Applies to a profile that is signed in with a Microsoft account: Yes

## Data type

- List of strings

## Windows information and settings

### Group Policy (ADMX) info

- GP unique name: WebContentFilteringBlockedCategories
- GP name: Configure Web Content Filtering
- GP path (Mandatory): Administrative Templates/Microsoft Edge
- GP path (Recommended): N/A
- GP ADMX file name: MSEdge.admx

#### Example value

Show...

```
Gambling
```

```
Streaming Media and Downloads
```

```
Games
```

### Registry settings

- Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge\WebContentFilteringBlockedCategories
- Path (Recommended): N/A
- Value name: 1, 2, 3
- Value type: List of REG_SZ

#### Example value

SOFTWARE\Policies\Microsoft\Edge\WebContentFilteringBlockedCategories\0 =
```
gambling
```

SOFTWARE\Policies\Microsoft\Edge\WebContentFilteringBlockedCategories\1 =
```
streaming_and_downloads
```

SOFTWARE\Policies\Microsoft\Edge\WebContentFilteringBlockedCategories\2 =
```
games
```




## See also
- [Microsoft Edge - Policies](../microsoft-edge-policies.md)
