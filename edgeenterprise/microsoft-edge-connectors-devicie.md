---
title: "Devicie"
ms.author: stmoody
author: vmliramichael
manager: venkatk
ms.date: 04/18/2025
audience: ITPro
ms.topic: reference
ms.service: microsoft-edge
ms.localizationpriority: high
ms.collection: M365-modern-desktop
ms.custom: generated
description: "Devicie"
---

# Set up a Devicie Connector

Devicie extends the power of Microsoft Intune by automating policy enforcement, compliance, and security configurations across managed devices. For Managed Service Providers and Enterprises, Devicie eliminates manual processes, ensuring endpoints remain secure, up-to-date, and aligned with organizational policies. With multitenant automation and hyperautomation capabilities, organizations can efficiently scale their endpoint management while maintaining a seamless user experience. 

## Benefits for Administrators

 - Monitor **browser extensions** across all managed endpoints  
 - Track **usage behavior and security events** in Microsoft Edge for Business  
 - Gain centralized visibility through the **Devicie console**  
 - Reduce risk from unauthorized or high-risk extensions  
 - Automate response actions via Devicie’s policy framework  
 - Extend the power of **Microsoft Intune** with **automated telemetry insights**  

## Prerequisites

 - **Microsoft 365** licenses with an **Intune-enabled environment**  
 - An active **Devicie subscription**  
 - **Microsoft Edge for Business** installed on all managed devices 
 - Appropriate administrative permissions to deploy and manage policies   

## Configure the Connector in the Devicie Admin Console

  1. **Log in to the Devicie admin console**  
Navigate to your Devicie dashboard and open the **Edge for Business Report** panel.

  2. **Access configuration settings**  
In the **settings tab**, locate your **endpoint name** and **reporting key**.

  3. **Apply settings in the Edge for Business portal**  
Use the retrieved endpoint name and key to configure the Devicie Connector within the Microsoft Edge for Business portal.

  4. **Validate integration**  
Once setup is complete, browser telemetry—including health indicators, extensions, and user behavior will populate automatically in your Devicie Browser Health dashboard.

## Configure the Connector in the Microsoft Edge Management Service

1. Navigate to [Microsoft Admin Center](https://admin.microsoft.com/Adminportal/Home#/Edge/Connectors).
   -   Admins must set up a configuration policy to assign to any Connector configuration. [Follow this guide to create a configuration policy](/deployedge/microsoft-edge-management-service?branch=pr-en-us-5295).
   - Once you have at least one configuration policy created, visit [the Connectors page in the Microsoft Edge Management Service](https://admin.microsoft.com/Adminportal/Home#/Edge/Connectors) to access the Connectors page in the Microsoft Edge Management Service.

2. Under **Discover Connectors**, find the **Devicie Reporting Connector** and select **Set up**.

3. In the **Chosen policy** field, select a policy for your Connector configuration.

4. Enter the following fields:
   - **Host address**
   - **Port**
   - **Token ID**

5. Select **Test Connection** to confirm the Connection is successful.

6. Under **User & Browser events**, select the desired browser events to be sent to the Devicie endpoint.

7. Select the desired **Optional events** and **Devices events**.

8. Select **Save configuration**.


