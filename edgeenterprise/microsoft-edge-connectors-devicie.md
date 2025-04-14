---
title: "Devicie"
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
description: "Devicie"
---

# Devicie Connector Overview

The **Devicie Reporting Connector for Microsoft Edge for Business** enables deep visibility into browser health indicators, user activity, and security events across your organization’s managed devices. By combining **browser telemetry** with **endpoint health reporting**, Devicie provides IT administrators with a unified view of user behavior, security risks, and compliance — all within Microsoft 365.

Whether you're managing a large enterprise or a multi-tenant MSP environment, Devicie automates endpoint management with policy enforcement, compliance, and configuration aligned to Microsoft Intune — while adding valuable browser-level insights.

## Benefits of Browser Health Integration

 - Monitor **browser extensions** across all managed endpoints  
 - Track **usage behavior and security events** in Microsoft Edge for Business  
 - Gain centralized visibility through the **Devicie console**  
 - Reduce risk from unauthorized or high-risk extensions  
 - Automate response actions via Devicie’s policy framework  
 - Extend the power of **Microsoft Intune** with **automated telemetry insights**  

## System Requirements

Before setting up the Devicie Reporting Connector, ensure your environment meets the following prerequisites:

 - **Microsoft 365** licenses with an **Intune-enabled environment**  
 - An active **Devicie subscription**  
 - **Microsoft Edge for Business** installed on all managed devices  

## How to Configure the Devicie Edge for Business Reporting Connector

Setting up the Devicie Reporting Connector for Microsoft Edge for Business is quick and seamless. Follow these steps:

  1. **Log in to the Devicie admin console**  
Navigate to your Devicie dashboard and open the Edge for Business Report panel.

  2. **Access configuration settings**  
In the settings tab, locate your endpoint name and reporting key.

  3. **Apply settings in the Edge for Business portal**  
Use the retrieved endpoint name and key to configure the Devicie connector within the Microsoft Edge for Business portal.

  4. **Validate integration**  
Once setup is complete, browser telemetry — including health indicators, extensions, and user behavior — will automatically populate in your Devicie Browser Health dashboard.
 

## Connector Setup and Configuration Steps

### Edge Management Service

### Instructions

1. Navigate to [Microsoft Admin Center](https://admin.microsoft.com/Adminportal/Home#/Edge/Connectors).

2. Under **Discover Connectors**, find the **Devicie Reporting Connector** and select **Set up**.

3. In the **Choose policy** field, select a policy for your connector configuration.

4. Enter the following fields:
   - **Host address**
   - **Port**
   - **Token ID**

5. Select **Test connection** to confirm the connection is successful.

6. Under **User & Browser events**, select the desired browser events to be sent to the Devicie endpoint.

7. Select the desired **Optional events** and **Devices events**.

8. Select **Save configuration**.


