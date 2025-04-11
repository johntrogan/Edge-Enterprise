---
title: "Device Trust Connectors"
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
description: "Device Trust Connectors"
---

# Device Trust Connectors

Microsoft Edge for Business Device Trust connectors enable administrators to enhance their organization's security posture directly within the browser. These connectors allow Identity Providers (IDPs) to obtain device-level signals from Microsoft Edge for Business during user authentication flows. These signals are then sent to and verified by the IDP before a user can authenticate to a specified resource.

## Benefits for Administrators
- Enhanced Security: By ensuring that only trusted devices can access corporate resources, administrators can significantly reduce the risk of unauthorized access and potential security breaches 

- Seamless Integration: Device Trust connectors integrate seamlessly with existing security measures and protocols, extending the reach of security investments without additional costs  


|Signals|                                       |
|----|------------------------------------------|
| 1  | Device Manufacturer                      |
| 2  | Device Model                             |
| 3  | Operating System                         |
| 4  | Operating System Version                 |
| 5  | Device Display Name                      |
| 6  | Disk Encryption State                    |
| 7  | Device Serial Number                     |
| 8  | OS Firewall State                        |
| 9  | System DNS Servers                       |
| 10 | Hostname                                 |
| 11 | MAC Addresses                            |
| 12 | Screen Locks Secured State               |
| 13 | Secure Boot Mode (Windows only)          |
| 14 | Windows Machine Domain                   |
| 15 | Windows User Domain                      |
| 16 | Browser Version                          |
| 17 | Built-In Browser DNS Client Enabled      |
| 18 | Site Isolation Enabled                   |
| 19 | Password Protection Warning Trigger      |

## Prerequisites 

- Microsoft Edge version 115.0.1901.7 or greater installed  
- Microsoft Edge Administrator permissions in the Microsoft 365 Admin Center  
- Supported OS: Windows 10/11 or Windows Server 2016 or later  
  - See Microsoft Edge Supported Operating Systems for details  

## Access the Edge Management Service

Use these steps to access the experience:

1. Go to the [Microsoft 365 admin center](https://admin.microsoft.com/Adminportal/Home#/homepage) and sign in.  
2. In the main left navigation bar, go to **Settings > Microsoft Edge**.

## Create a Configuration Policy

Admins must have a configuration profile set up as a prerequisite for configuring a connector. [Follow this guide to create a configuration profile](https://review.learn.microsoft.com/en-us/deployedge/microsoft-edge-management-service?branch=pr-en-us-5295).

## Set Up a Device Trust Connector
Visit https://admin.microsoft.com/Adminportal/Home#/Edge/Connectors to access the connectors page in the Edge Management service.

- [Duo Connector Setup](https://review.learn.microsoft.com/en-us/deployedge/microsoft-edge-connectors-duo?branch=pr-en-us-5295)
- [Ping Identity]()
- [RSA]()


