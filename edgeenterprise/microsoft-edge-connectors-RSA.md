---
title: "RSA Documentation"
ms.author: stmoody
author: vmliramichael
manager: venkatk
ms.date: 04/21/2025
audience: ITPro
ms.topic: reference
ms.service: microsoft-edge
ms.localizationpriority: high
ms.collection: M365-modern-desktop
ms.custom: generated
description: "RSA"
---

# Set up a RSA Connector 

Take control with the RSA Device Trust Connector for Microsoft Edge for Business. This connector leverages device signals from Microsoft Edge so only verified, managed endpoints can access critical apps. By coupling strong identity authentication with device posture checks, you extend protection far beyond just who logs in, accelerating Zero Trust maturity without complex setups. 

## Configure the RSA Connector

Visit [this page](https://community.rsa.com/s/product-integration/a9HPO0000000eWv2AI/edge-for-business) to learn how to enable an RSA Device Trust Connector.

### Configure the Connector in the Edge Management Service

1. **Navigate to the Microsoft Admin Center**  
   Go to [https://admin.microsoft.com/Adminportal/Home#/Edge/Connectors](https://admin.microsoft.com/Adminportal/Home#/Edge/Connectors)
   -   Admins must set up a configuration policy to assign to any Connector configuration. [Follow this guide to create a configuration policy](/deployedge/microsoft-edge-management-service).
   - Once you have at least one configuration policy created, visit [the Connectors page in the Edge Management Service](https://admin.microsoft.com/Adminportal/Home#/Edge/Connectors) to access the Connectors page in the Edge Management Service.

2. **Discover the Connector**  
   Under **Discover Connectors**, locate the **RSA Device Trust Connector** and select **Set up**.

3. **Select a Policy**  
   In the **Choose policy** field, select a policy appropriate for your connector configuration.

4. **Enter URL Patterns**  
   In the **URL patterns to allow, one per line** field, input the URL for your configuration.

5. **Save the Configuration**  
   Select **Save configuration** to apply your changes.


