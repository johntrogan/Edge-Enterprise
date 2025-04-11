---
title: "Cisco Duo"
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
description: "Duo"
---
# Cisco Duo Connector Overview

The Microsoft Edge for Business connector works with Cisco Duo to strengthen security by enabling device trust verification without the need for additional agents. Simplify your security management with easy Duo implementation, ensuring secure application access and enhanced browser protections.

## Connector Setup and Configuration Steps

### Configuration Steps – Edge Management Service

#### 1. Create a New Profile Policy in Microsoft 365
- Log in to the Microsoft 365 Admin Center and navigate to the Settings -> Microsoft Edge page.
- Navigate to the “Configuration profilespolicies” tab, click “Add a profileCreate policy”.
- (Optional) After saving, click on your newly created profilepolicy, navigate to the “Group assignment” tab, and select a group that your profile policy will be assigned to.

#### 2. Configure the Cisco Duo Connector in the Admin Center
- After creating a profilepolicy, navigate to the “Connectors” tab on the Microsoft Edge settings page and click on the “Set up” button under the Cisco Duo Device Trust connector.
- Search for the profile policy you’ve created at in step 2 in the “Choose Policy“ dropdown and paste “https://duosecurity.com“ in the “URL patterns to allow”.
- Click the “Save configuration” button. You should now see the Cisco Duo Device Trust connector appear under the “Installed Connectors” section.

## Cisco Duo Configuration 

### Admin Portal Setup
#### 1. Create the Edge Device Trust Connector Integration
- Log in to the Duo Admin Panel and navigate to Trusted Endpoints under the Devices section.
- If this is your first management integration, click the Get started button at the bottom of the Trusted Endpoints introduction page. If you're adding another management integration, click the Add Integration button you see at the top of the page instead.
- On the "Add Management Tools Integration" page, locate Microsoft Edge for Business Device Trust Connector in the list of "Device Management Tools" and click the Add this integration selector.
- Choose Windows from the "Recommended" options, and then click the Add button.
- The new Microsoft Edge for Business Device Trust Connector integration is created in the "Disabled" state. You'll turn it on when you're ready to apply your Duo trusted endpoints policy. If the Edge for Business Device Trust Connector trust check fails any active Duo Desktop based integrations will run a trust check as a fallback.
- During setup, keep the Duo Admin Panel open in your browser. You'll need to refer back to the Edge for Business Device Trust Connector integration page to complete the Microsoft Entra configuration steps.

#### 2. Register your Microsoft Entra Application with Duo
- Return to your Edge for Business Device Trust Connector management integration details page in the Duo Admin Panel. Scroll down to the section labeled “Register Microsoft Entra Application with Duo”.
- Enter the Tenant ID, Client ID, and Client Secret values from the application you created earlier.
- Click the Test Configuration button to verify your setup. If you do not receive a "Configuration Successful!" message, double-check that you provided the right application information.
- If testing your configuration was successful, click Save & Configure.

#### 3. Finish Trusted Endpoints Deployment
- After creating the Edge for Business Device Trust Connector Trusted Endpoints integration, set the Trusted Endpoints policy to start checking for Edge for Business browser enrollment as users authenticate to Duo-protected services and applications.
- When your trusted endpoints policy is applied to your Duo applications, return to the Edge for Business Device Trust Connector Trusted Endpoints integration in the Admin Panel. The "Change Integration Status" section of the page shows the current integration status (disabled by default after creation). You can choose to either activate this integration only for members of a specified test group or groups, or activate for all users.
- The Device Insight and Endpoints pages in the Duo Admin Panel show which access devices are verified.

#### 4. Verify Your Setup
- Authenticate to a protected application using a managed Edge for Business browser.
- When the Trusted Endpoints policy is set to “Allow all endpoints” ,”, users receive access to the application (assuming the managed Edge browser passes all other policy verification), and Duo records the trusted or untrusted status of that browser.
- If the Trusted Endpoints policy is set to “Require endpoints to be trusted”, Duo blocks access from unmanaged devices and Duo successfully verifies the managed Edge for Business browser's management status and configuration against the required policy settings, then the user receives access to the protected application.
- If the managed Edge for Business browser fails the configuration and policy checks, then Duo denies will deny application accessaccess to the application from the unmanaged browser.


