---
title: "Omnissa"
ms.author: stmoody
author: vmliramichael
manager: venkatk
ms.date: 04/15/2025
audience: ITPro
ms.topic: reference
ms.service: microsoft-edge
ms.localizationpriority: high
ms.collection: M365-modern-desktop
ms.custom: generated
description: "Omnissa"
---

# Set up an Omnissa Device Trust Connector 

## Overview
Microsoft Edge for Business integrates with Omnissa Access to verify the posture of unmanaged or third-party managed devices prior to granting access to company resources. A managed Edge browser can collect device posture information and share it with Omnissa Access, enabling real-time, posture-informed access decisions.

## Prerequisites
- Omnissa Access SaaS tenant
- Microsoft Entra tenant ID
- Managed profiles
- Subscription plan:
  - Education: Microsoft 365 A3, A5
  - Business: Microsoft 365 Business Standard, Premium
  - Enterprise: Office 365 E3, E5, Microsoft 365 E3, E5

## Set Up Edge for Business Device Signals Adapter in Omnissa Access

### 1. Enable the Adapter
- Navigate to: **Omnissa Access Console > Integrations > Authentication Methods**
- Select: **Edge for Business Device Signals**
- Click **Configure**

### 2. Configuration Fields
| Option | Description |
|--------|-------------|
| Enable Microsoft Edge for Business Device Signal Adapter | Set to **Yes** to enable |
| URLs matcher to trigger Microsoft Edge inline flow | Copy and save this URL for use in the Edge management service |
| IDP Service Principal | Copy and save this value for the Edge management service |
| Microsoft Tenant ID | Enter your Microsoft Entra ID tenant ID |
| Allow access if not a managed Edge browser | Leave disabled (recommended). If enabled, configure an alternative strong fallback authentication |
| Verify device's disk encryption status | Choose from:<br>- Encrypted<br>- Encrypted \| Unspecified<br>- Encrypted \| Unknown<br>- Encrypted \| Unspecified \| Unknown |
| Verify device's firewall status | Choose from:<br>- Enabled<br>- Enabled \| Unspecified<br>- Enabled \| Unknown<br>- Enabled \| Unspecified \| Unknown |
| Verify device's screen lock status | Choose from:<br>- Enabled<br>- Enabled \| Unspecified<br>- Enabled \| Unknown<br>- Enabled \| Unspecified \| Unknown |

![screenshot1S hypr edge API.](media/microsoft-edge-connectors-omnissa/1.png)  

### 3. Click **Save**.

### 4. Next Steps
- Copy the **URL matcher** and **IDP Service Principal**
- Use them to configure the Edge Device Trust Connector in the Microsoft Edge management console

## Integrate with Microsoft Edge Management Console
The Microsoft Edge Device Trust Connector must be configured to receive signals from Edge and share them with Omnissa Access.

1. **Navigate to the Microsoft Admin Center**  
   Go to [https://admin.microsoft.com/Adminportal/Home#/Edge/Connectors](https://admin.microsoft.com/Adminportal/Home#/Edge/Connectors)

2. **Discover the Connector**  
   Under **Discover Connectors**, locate the **Omnissa Device Trust Connector** and select **Set up**.

3. **Select a Policy**  
   In the **Choose policy** field, select a policy appropriate for your Connector configuration.

4. **Enter URL Patterns**  
   In the **URL patterns to allow, one per line** field, input the URL for your configuration.

5. **Save the Configuration**  
   Select **Save configuration** to apply your changes.

## Add Device Signals as a Secondary Authentication Method

### 1. Link Method to Identity Provider
- Go to: **Omnissa Access Console > Integrations > Identity Providers**
- Select the Identity Provider
- Enable: **Microsoft Edge for Business Device Signals** under Authentication Methods
- Click **Save**

### 2. Add to Access Policy
- Go to: **Resources > Policies**
- Add or edit a policy
- Click **Next** to open Configuration
- Create or edit a rule:

| Field | Description |
|-------|-------------|
| If user's network range is | Select network range |
| and user accessing content from | Select **Windows 10+** |
| and user belongs to groups | Choose target group (or leave blank for all users) |
| Then perform this action | **Authenticate using...** |
| then the user may authenticate using | Select primary authentication method |
| ADD AUTHENTICATION | Select **Microsoft Edge for Business Device Signals** as the secondary method |

Click **Next** and then **Save**.

### 3. Authentication Flow
- User signs in with primary authentication
- Edge checks device security status using configured signals
- Omnissa Access approves/denies access based on compliance

## Audit and Reporting
- Go to: **Monitor > Reports** in Omnissa Access Console
- Select **Audit Events** report type
- Configure parameters and click **Show Results**
- Report logs include signal status and authentication success/failure
