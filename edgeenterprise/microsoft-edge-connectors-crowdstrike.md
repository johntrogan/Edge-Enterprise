---
title: "Microsoft Edge Crowdstrike"
ms.author: stmoody
author: vmliramichael
manager: venkatk
ms.date: 04/03/2025
audience: ITPro
ms.topic: reference
ms.service: microsoft-edge
ms.localizationpriority: high
ms.collection: M365-modern-desktop
ms.custom: generated
description: "Crowdstrike"
---

# Crowdstrike Connector Overview

Easily ingest Microsoft Edge for Business data into CrowdStrike Falcon® Next-gen SIEM for unified visibility across endpoints, browsers, and beyond. View browser security insights alongside other threat indicators to accelerate detection, minimize context switching, and improve triage accuracy.  

## Connector Setup and Configuration Steps

### Configuration Steps – Microsoft Edge Management Service

### Instructions

1. Navigate to [Microsoft Admin Center](https://admin.microsoft.com/Adminportal/Home#/Edge/Connectors).

2. Under **Discover Connectors**, find the **Crowdstrike Reporting Connector** and select **Set up**.

3. In the **Choose policy** field, select a policy for your connector configuration.

4. Enter the following fields:
   - **Host address**
   - **Port**
   - **Token ID**

5. Select **Test connection** to confirm the connection is successful.

6. Under **User & Browser events**, select the desired browser events to be sent to the Crowdstrike endpoint.

7. Select the desired **Optional events** and **Devices events**.

8. Select **Save configuration**.

## Crowdstrike Configuration 

### Admin Portal Setup

#### 1. Create the Report Connector Integration
- Log in to the Crowdstrike Admin Panel and navigate to Trusted Endpoints under the Devices section.
- If this is your first management integration, click the Get started button at the bottom of the Trusted Endpoints introduction page. If you're adding another management integration, click the Added Integration button you see at the top of the page instead.
- On the "Add Management Tools Integration" page, locate Microsoft Edge for Business Device Trust Connector in the list of "Device Management Tools" and click the Add this integration selector.
- Choose Windows from the "Recommended" options, and then click the Add button.
- The new Microsoft Edge for Business Device Trust Connector integration is created in the "Disabled" state. You'll turn it on when you're ready to apply your Crowdstrike trusted endpoints policy. If the Microsoft Edge for Business Device Trust Connector trust check fails any active Crowdstrike Desktop based integrations will run a trust check as a fallback.
- During setup, keep the Crowdstrike Admin Panel open in your browser. You need to refer back to the Microsoft Edge for Business Device Trust Connector integration page to complete the Microsoft Entra configuration steps.

#### 2. Register your Microsoft Entra Application with Crowdstrike
- Return to your Microsoft Edge for Business Device Trust Connector management integration details page in the Crowdstrike Admin Panel. Scroll down to the section labeled “Register Microsoft Entra Application with Crowdstrike”.
- Enter the Tenant ID, Client ID, and Client Secret values from the application you created earlier.
- Click the Test Configuration button to verify your setup. If you don't receive a "Configuration Successful!" message, double-check that you provided the right application information.
- If testing your configuration was successful, click Save & Configure.

#### 3. Finish Trusted Endpoints Deployment
- After creating the Microsoft Edge for Business Device Trust Connector Trusted Endpoints integration, set the Trusted Endpoints policy to start checking for Microsoft Edge for Business browser enrollment as users authenticate to Crowdstrike-protected services and applications.
- When your trusted endpoints policy is applied to your Crowdstrike applications, return to the Microsoft Edge for Business Device Trust Connector Trusted Endpoints integration in the Admin Panel. The "Change Integration Status" section of the page shows the current integration status (disabled by default after creation). You can choose to either activate this integration only for members of a specified test group or groups, or activate for all users.
- The Device Insight and Endpoints pages in the Crowdstrike Admin Panel show which access devices are verified.

#### 4. Verify Your Setup
- Authenticate to a protected application using a managed Microsoft Edge for Business browser.
- When the Trusted Endpoints policy is set to “Allow all endpoints”, users receive access to the application (assuming the managed Microsoft Edge browser passes all other policy verification), and Crowdstrike records the trusted or untrusted status of that browser.
- If the Trusted Endpoints policy is set to “Require endpoints to be trusted”, Crowdstrike blocks access from unmanaged devices and Crowdstrike successfully verifies the managed Microsoft Edge for Business browser's management status and configuration against the required policy settings, then the user receives access to the protected application.
- If the managed Microsoft Edge for Business browser fails the configuration and policy checks, then Crowdstrike will deny access to the application from the unmanaged browser.
