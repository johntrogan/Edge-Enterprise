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

## Cisco Duo Configuration 

### Admin Portal Setup

#### 1. Create the Edge Device Trust Connector Integration

1. Log in to the **Duo Admin Panel** and navigate to **Trusted Endpoints** under the **Devices** section.
2. If this is your first management integration:
   - Click **Get started** at the bottom of the Trusted Endpoints introduction page.
3. If you're adding another management integration:
   - Click **Add Integration** at the top of the page.
4. On the **Add Management Tools Integration** page:
   - Find **Microsoft Edge for Business Device Trust Connector** under **Device Management Tools**.
   - Click **Add this integration**.
5. Choose **Windows** from the "Recommended" options and click **Add**.
6. The integration is created in a **Disabled** state.
   - You’ll activate it when ready to apply your Duo Trusted Endpoints policy.
   - If the Edge for Business trust check fails, fallback to Duo Desktop integrations will occur.
7. Keep the Duo Admin Panel open — you’ll refer back to complete Microsoft Entra setup.
![screenshot of duo admin.](media/microsoft-edge-connectors-duo/image1.png)

#### 2. Register Your Microsoft Entra Application with Duo

1. In the Duo Admin Panel, scroll to **Register Microsoft Entra Application with Duo** on the integration details page.
2. Enter the following values from your Entra application:
   - **Tenant ID**
   - **Client ID**
   - **Client Secret**
3. Click **Test Configuration** to verify your setup.
   - If the test fails, recheck the entered values.
4. If successful, click **Save & Configure**.

#### 3. Finish Trusted Endpoints Deployment

1. Apply the **Trusted Endpoints** policy to begin checking Edge for Business browser enrollment during authentication.
2. Return to the **Edge for Business Device Trust Connector** integration page.
3. In the **Change Integration Status** section:
   - Choose to activate for test groups or all users.
4. Use the **Device Insight** and **Endpoints** pages to confirm which devices are verified.

#### 4. Verify Your Setup

1. Authenticate to a Duo-protected app using a **managed Edge for Business** browser.
2. If the policy is set to **Allow all endpoints**:
   - The user receives access if all other verifications pass.
   - Duo logs the browser as trusted or untrusted.
3. If the policy is set to **Require endpoints to be trusted**:
   - Duo **blocks** unmanaged browsers.
   - If verification succeeds, access is granted.
   - If verification fails, access is **denied**.

## Edge Management Service

#### Step-by-step Instructions

1. **Navigate to the Microsoft Admin Center**  
   Go to [https://admin.microsoft.com/Adminportal/Home#/Edge/Connectors](https://admin.microsoft.com/Adminportal/Home#/Edge/Connectors)

2. **Discover the Connector**  
   Under **Discover Connectors**, locate the **Cisco Duo Device Trust Connector** and select **Set up**.

3. **Select a Policy**  
   In the **Choose policy** field, select a policy appropriate for your connector configuration.

4. **Enter URL Patterns**  
   In the **URL patterns to allow, one per line** field, input the required URL patterns.

5. **Save the Configuration**  
   Select **Save configuration** to apply your changes.

   ![screenshot of duo connector.](media/microsoft-edge-connectors-duo/image2.png)
