---
title: "Data Loss Prevention - Symantec"
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
description: "Symantec"
---

# Set up a Symantec Connector

Prevent data loss with Microsoft Edge for Business and Symantec Data Loss Prevention Endpoint. This integration delivers a more secure browsing experience as it allows customers to identify, monitor and protect sensitive, confidential or regulated data.  This includes controlling data that is uploaded, pasted or printed from the web.  

## Configure the Connector in the Edge Management Service

1. **Navigate to the Microsoft Admin Center**  
   Go to [https://admin.microsoft.com/Adminportal/Home#/Edge/Connectors](https://admin.microsoft.com/Adminportal/Home#/Edge/Connectors)

2. **Discover the Connector**  
   Under **Discover Connectors**, locate the **Symatec DLP Connector** and select **Set up**.

3. **Select a Policy**  
   In the **Choose policy** field, select a policy appropriate for your connector configuration.

4. **Enable data loss prevention for browser actions**  
   **Select** the user actions you want to be scanned by Symantec’s DLP agent. 

5. **When the data loss prevention verdict is not received in time**  
   Choose to **‘Allow file access’** or **‘Block file access’**. This determines the default verdict if a communication error between Edge and the DLP agent occurs.   

6. **Save the Configuration**  
   Select **Save configuration** to apply your changes.

## Symantec Configuration 

### 1. **Verify** that the Configuration Policy was Deployed Successfully

1. On a Windows endpoint, **sign in** to Microsoft Edge for Business with a valid Microsoft Entra ID.

2. **Navigate** to edge://management, and **verify** that the browser is managed by your organization.

3. **Navigate** to edge://policy, and **verify** that the following policies are listed and that their **Status is OK**:
   - OnBulkDataEntryEnterpriseConnector  
   - OnFileAttachedEnterpriseConnector  
   - OnPrintEnterpriseConnector

### 2. **Enable** Monitoring for Microsoft Edge for Business in the Agent Configuration

1. In the Enforce Server administration console, **navigate** to:  
   System > Agents > Agent Configuration  
   and **select** the agent configuration that you want to modify.  
   - *See* Adding and editing agent configurations

2. In the **Channels** tab:
   - **Make sure** that the Edge (HTTPS) monitoring channel is checked.  
     This enables the DLP Agent to monitor file and folder uploads and also clipboard Paste actions.
   - Depending on your security needs, you can also **enable** monitoring for the Printer/Fax channel.  
     **Make sure** that the corresponding option is enabled in the connector settings at the Microsoft 365 admin center.

3. **Save** your changes.

4. For more information about configuring print monitoring, **see** Printer/Fax settings.

### 3. **Enable** Monitoring using the Symantec Content Analysis Connector in the Advanced Agent Settings

1. In the Enforce Server administration console, **navigate** to:  
   System > Agents > Agent Configuration  
   and **select** the agent configuration that you want to modify.  
   - *See* Adding and editing agent configurations

2. In the **Advanced Settings** tab of the agent configuration:
   - **Set** the value of the ContentAnalysisSDK.EDGE_MONITORING.int advanced agent setting to 1.  
     - *The default value is 0, which indicates that monitoring is active through the Symantec DLP browser extension.*

3. **Save** your changes.

### 4. **Configure** and **Deploy** a DLP Policy

1. If you have not already done so, **configure** a DLP policy to specify which confidential information you want to detect in Microsoft Edge for Business.

2. For more information, **see** Workflow for implementing policies.

### 5. **Ensure** that End-Users are Signed In to Microsoft Edge for Business

1. **Ensure** that end-users **sign in** to Microsoft Edge for Business with a valid Microsoft Entra ID.

