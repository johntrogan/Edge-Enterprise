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


| **Signal**                             | **Category**           | **Description**                                                  |
|----------------------------------------|------------------------|------------------------------------------------------------------|
| Device Manufacturer                    | Hardware Information   | The company that manufactures the device                         |
| Device Model                           | Hardware Information   | The model name of the device                                     |
| Operating System                       | OS Information         | The OS installed on the device                                   |
| Operating System Version               | OS Information         | Version number of the operating system                           |
| Device Display Name                    | Hardware Information   | The name given to the device in the system                       |
| Disk Encryption State                  | Security Features      | Whether disk encryption is enabled                               |
| Device Serial Number                   | Hardware Information   | The unique serial number of the device                           |
| OS Firewall State                      | OS Information         | The current state of the OS firewall                             |
| System DNS Servers                     | Network Information    | The DNS servers configured for the device                        |
| Hostname                               | General Information    | The hostname of the device                                       |
| MAC Addresses                          | Hardware Information   | The MAC addresses assigned to the device                         |
| Screen Locks Secured State             | Security Features      | Whether the screen lock is secured                               |
| Secure Boot Mode (Windows only)        | OS Information         | Indicates whether secure boot is enabled                         |
| Windows Machine Domain                 | OS Information         | The domain to which the machine belongs                          |
| Windows User Domain                    | OS Information         | The user domain for Windows                                      |
| Browser Version                        | Browser Information    | The version of the browser used                                  |
| Built-In Browser DNS Client Enabled    | Browser Information    | Indicates if the built-in browser DNS client is enabled          |
| Site Isolation Enabled                 | Browser Information    | Whether site isolation is enabled in the browser                 |
| Password Protection Warning Trigger    | Security Features      | A warning triggered for password-related protections             |

## Create a Configuration Policy

Admins must have a configuration profile set up as a prerequisite for configuring a connector. [Follow this guide to create a configuration profile](https://review.learn.microsoft.com/en-us/deployedge/microsoft-edge-management-service?branch=pr-en-us-5295).

## Set Up a Device Trust Connector
Visit https://admin.microsoft.com/Adminportal/Home#/Edge/Connectors to access the connectors page in the Edge Management service.

- [Duo Connector Setup](https://review.learn.microsoft.com/en-us/deployedge/microsoft-edge-connectors-duo?branch=pr-en-us-5295)
- [Ping Identity]()
- [RSA]()


