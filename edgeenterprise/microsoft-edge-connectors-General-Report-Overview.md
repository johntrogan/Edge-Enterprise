---
title: "Microsoft Edge Reporting Connectors"
ms.author: stmoody
author: vmliramichael
manager: venkatk
ms.date: 02/10/2025
audience: ITPro
ms.topic: reference
ms.service: microsoft-edge
ms.localizationpriority: high
ms.collection: M365-modern-desktop
ms.custom: generated
description: "Reporting Connectors"
---

# Reporting Connectors

Microsoft Edge for Business Reporting connectors enable admins to send user security events from the browser to participating provider endpoints.

## Security Events

The following security events can be enabled in a reporting connector:

| Event Value               | Event Description                                                                                   |
|---------------------------|------------------------------------------------------------------------------------------------------|
| Browser crash             | Browser or tab crashed (only reported when device-level reporting is available).                    |
| Browser extension install | Extensions are installed, updated, or removed.                                                       |
| Malware transfer (download) | Download blocked by SmartScreen, or download block bypassed/opened by user.                     |
| Unsafe site visit         | SmartScreen blocking page is shown or bypassed.                                                     |
| URL filtering interstitial| Web Content Filtering interstitial is shown (can be from SmartScreen's E5/MCAS or Edge management). |
| Content transfer          | This event will be enabled after V1 of the reporting connector launch.                              |
| Content unscanned         | Content failed to scan for DLP (requires Analysis connector to be configured).                      |
| Sensitive data transfer   | Content marked as sensitive by DLP scan (requires Analysis connector to be configured).             |
| Password changed          | A password is changed in response to a password reuse warning.                                      |
| Password reuse            | A password is detected as reused between an enterprise account and an account on an external site.  |
| Login                     | A sign-in to a domain in the specified list is successful.                                           |
| Password breach           | A password is detected as compromised as part of a known data breach.                               |

## Prerequisites

- Microsoft Edge version 115.0.1901.7 or greater installed  
- Microsoft Edge Administrator permissions in Microsoft 365 Admin Center  
- Supported operating systems: Windows 10/11 or Windows Server 2016 or later  
  - See Microsoft Edge Supported Operating Systems for details  

## Access the Experience

Use these steps to access the experience:

1. Go to the [Microsoft 365 admin center](https://admin.microsoft.com/Adminportal/Home#/homepage) and sign in  
2. In the main left navigation bar, go to **Settings > Microsoft Edge**

## Create a Configuration Profile

*Admin must have a configuration profile to link each connector configuration to.*  
*Link to walkthrough to create a profile.*

## Set Up a Reporting Connector

*Link to all the subpages?*

## Privacy and Compliance

### Default Settings

- The feature is enabled only via an admin policy  
- User consent considerations are under evaluation

### Privacy Safeguards

- Adherence to GDPR and regional compliance regulations  
- Secure data handling practices to maintain user privacy

### Troubleshooting and FAQ

- TBD: will get feedback from the team

## Resources

*Links to ISV documentation / EMX docs?*  
- TBD: will get feedback from the team
