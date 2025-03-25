---
title: "Microsoft Edge Device Trust Overview"
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
description: "Device Trust"
---

# General Device Trust Overview

Microsoft Edge for Business Device Trust connectors enable admins to strengthen their organization’s security posture within the browser. Device trust connectors enable IDPs to obtain device-level signals directly from Microsoft Edge for Business during user authentication flows. These signals are sent to and verified by the IDP before a user can authenticate to a specified resource.

## Signals

The following signals are sent to the IDP during the device trust flow:

1. Device Manufacturer  
2. Device Model  
3. Operating System  
4. Operating System Version  
5. Device Display Name  
6. Disk Encryption State  
7. Device Serial Number  
8. OS Firewall State  
9. System DNS Servers  
10. Hostname  
11. MAC Addresses  
12. Screen Locks Secured State  
13. Secure Boot Mode (Windows only)  
14. Windows Machine Domain  
15. Windows User Domain  
16. Browser Version  
17. Built-In Browser DNS Client Enabled  
18. Site Isolation Enabled  
19. Password Protection Warning Trigger  

## Prerequisites 

- Microsoft Edge version 115.0.1901.7 or greater installed  
- Microsoft Edge Administrator permissions in the Microsoft 365 Admin Center  
- Supported OS: Windows 10/11 or Windows Server 2016 or later  
  - See Microsoft Edge Supported Operating Systems for details  

## Access the Experience

Use these steps to access the experience:

1. Go to the [Microsoft 365 admin center](https://admin.microsoft.com/Adminportal/Home#/homepage) and sign in.  
2. In the main left navigation bar, go to **Settings > Microsoft Edge**.

## Create a Configuration Profile

*Admin must have a configuration profile to link each connector configuration to.*  
*Link to walk through to create a profile.*

## Set Up a Device Trust Connector

*Link to all the subpages?*

## Privacy and Compliance

### Default Settings
- The feature is enabled only via an admin policy.  
- User consent considerations are under evaluation.

### Privacy Safeguards
- Adherence to GDPR and regional compliance regulations.  
- Secure data handling practices to maintain user privacy.

### Troubleshooting and FAQ
- TBD: feedback from the team.

## Resources

*Links to ISV documentation / EMX docs?*  
- TBD: feedback from the team.
