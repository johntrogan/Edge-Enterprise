---
title: "Trellix"
ms.author: stmoody
author: vmliramichael
manager: venkatk
ms.date: 07/18/2025
audience: ITPro
ms.topic: reference
ms.service: microsoft-edge
ms.localizationpriority: high
ms.collection: M365-modern-desktop
ms.custom: generated
description: "Trellix"
---

Trellix Data Loss Prevention (DLP) is designed to help customers confidently secure
their sensitive data. As organizations increasingly adopt cloud-based applications
and services, Trellix has partnered with Microsoft Edge for Business to deploy a
specialized content analysis connector that enhances web security. This connector
ensures a secure browsing experience through an API integration between Edge for
Business and Trellix Data Loss Prevention (DLP) Endpoint for Windows.

Organizations concerned with safeguarding sensitive data, complying with
mandates, and addressing the growing concern of potential data leakage through
web-based AI will benefit from implementing this protection. This integration is
offered as an advanced feature within Trellix DLP Endpoint Windows version 11.12.

## Edge Connector Configuration

### Using the Microsoft Edge Management Service

1. **Navigate to the Microsoft Admin Center**  
   Go to [https://admin.microsoft.com/Adminportal/Home#/Edge/Connectors](https://admin.microsoft.com/Adminportal/Home#/Edge/Connectors)
   -   Admins must set up a configuration policy to assign to any Connector configuration. [Follow this guide to create a configuration policy](/deployedge/microsoft-edge-management-service).
   - Once you have at least one configuration policy created, visit [the Connectors page in the Microsoft Edge Management Service](https://admin.microsoft.com/Adminportal/Home#/Edge/Connectors) to access the Connectors page in the Microsoft Edge Management Service.

2. **Discover the Connector**  
   Under **Discover Connectors**, locate the **Trellix DLP Connector** and select **Set up**.

3. **Select a Policy**  
   In the **Chosen policy** field, select a policy appropriate for your connector configuration.

4. **Enable data loss prevention for browser actions**  
   **Select** the user actions you want to be scanned by Trellix's DLP agent. 

5. **When the data loss prevention verdict is not received in time**  
   Choose to **‘Allow file access’** or **‘Block file access’**. This determines the default verdict if a communication error between Edge and the DLP agent occurs.   

6. **Save the Configuration**  
   Select **Save configuration** to apply your changes.



## Trellix Configuration 
The Edge for Business content analysis connector is not enabled by default in DLP
Endpoint Windows version 11.12.0. It needs to be enabled using advanced parameters.
Customers can contact Trellix Customer Support through their online portal or by
calling their designated contact to enable this capability.

Customers can find contact information for regional technical support call centers
here https://thrive.trellix.com/s/article/KB95597?language=en_US.

  
