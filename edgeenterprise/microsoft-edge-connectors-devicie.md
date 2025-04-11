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

The Devicie Reporting Connector for Microsoft Edge for Business integrates browser performance and security information with endpoint telemetry to provide a complete view of the device. Correlation across the endpoint and the browser provides clarity to the IT technician enabling faster resolution of issues and visibility of browser based activity health across the whole fleet.  

## Connector Setup and Configuration Steps

### Configuration Steps – Edge Management Service

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

## Devicie Configuration 

### Admin Portal Setup

#### 1. Create the Report Connector Integration
- Log in to the Devicie Admin Panel and navigate to Trusted Endpoints under the Devices section.
- If this is your first management integration, click the Get started button at the bottom of the Trusted Endpoints introduction page. If you're adding another management integration, click the Add Integration button you see at the top of the page instead.
- On the "Add Management Tools Integration" page, locate Microsoft Edge for Business Device Trust Connector in the list of "Device Management Tools" and click the Add this integration selector.
- Choose Windows from the "Recommended" options, and then click the Add button.
- The new Microsoft Edge for Business Device Trust Connector integration is created in the "Disabled" state. You'll turn it on when you're ready to apply your Devicie trusted endpoints policy. If the Edge for Business Device Trust Connector trust check fails any active Devicie Desktop based integrations will run a trust check as a fallback.
- During setup, keep the Devicie Admin Panel open in your browser. You'll need to refer back to the Edge for Business Device Trust Connector integration page to complete the Microsoft Entra configuration steps.

#### 2. Register your Microsoft Entra Application with Devicie
- Return to your Edge for Business Device Trust Connector management integration details page in the Devicie Admin Panel. Scroll down to the section labeled “Register Microsoft Entra Application with Devicie”.
- Enter the Tenant ID, Client ID, and Client Secret values from the application you created earlier.
- Click the Test Configuration button to verify your setup. If you do not receive a "Configuration Successful!" message, double-check that you provided the right application information.
- If testing your configuration was successful, click Save & Configure.

#### 3. Finish Trusted Endpoints Deployment
- After creating the Edge for Business Device Trust Connector Trusted Endpoints integration, set the Trusted Endpoints policy to start checking for Edge for Business browser enrollment as users authenticate to Devicie-protected services and applications.
- When your trusted endpoints policy is applied to your Devicie applications, return to the Edge for Business Device Trust Connector Trusted Endpoints integration in the Admin Panel. The "Change Integration Status" section of the page shows the current integration status (disabled by default after creation). You can choose to either activate this integration only for members of a specified test group or groups, or activate for all users.
- The Device Insight and Endpoints pages in the Devicie Admin Panel show which access devices are verified.

#### 4. Verify Your Setup
- Authenticate to a protected application using a managed Edge for Business browser.
- When the Trusted Endpoints policy is set to “Allow all endpoints”, users receive access to the application (assuming the managed Edge browser passes all other policy verification), and Devicie records the trusted or untrusted status of that browser.
- If the Trusted Endpoints policy is set to “Require endpoints to be trusted”, Devicie blocks access from unmanaged devices and Devicie successfully verifies the managed Edge for Business browser's management status and configuration against the required policy settings, then the user receives access to the protected application.
- If the managed Edge for Business browser fails the configuration and policy checks, then Devicie will deny access to the application from the unmanaged browser.
