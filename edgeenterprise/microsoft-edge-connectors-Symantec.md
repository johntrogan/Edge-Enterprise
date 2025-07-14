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

# Set up a Symantec DLP Connector

Prevent data loss with Microsoft Edge for Business and Symantec Data Loss Prevention Endpoint. This integration delivers a more secure browsing experience as it allows customers to identify, monitor and protect sensitive, confidential or regulated data.  This includes controlling data that is uploaded, pasted, or printed from the web.  

## Edge Connector Configuration

### Using the Microsoft Edge Management Service

1. **Navigate to the Microsoft Admin Center**  
   Go to [https://admin.microsoft.com/Adminportal/Home#/Edge/Connectors](https://admin.microsoft.com/Adminportal/Home#/Edge/Connectors)
   -   Admins must set up a configuration policy to assign to any Connector configuration. [Follow this guide to create a configuration policy](/deployedge/microsoft-edge-management-service).
   - Once you have at least one configuration policy created, visit [the Connectors page in the Microsoft Edge Management Service](https://admin.microsoft.com/Adminportal/Home#/Edge/Connectors) to access the Connectors page in the Microsoft Edge Management Service.

2. **Discover the Connector**  
   Under **Discover Connectors**, locate the **Symatec DLP Connector** and select **Set up**.

3. **Select a Policy**  
   In the **Chosen policy** field, select a policy appropriate for your connector configuration.

4. **Enable data loss prevention for browser actions**  
   **Select** the user actions you want to be scanned by Symantec’s DLP agent. 

5. **When the data loss prevention verdict is not received in time**  
   Choose to **‘Allow file access’** or **‘Block file access’**. This determines the default verdict if a communication error between Edge and the DLP agent occurs.   

6. **Save the Configuration**  
   Select **Save configuration** to apply your changes.

In addition to using the Microsoft Edge Management Service, you can now enable the Symantec DLP Connector using either Group Policy or Microsoft Intune.

### Using Group Policy (GPO)

You can enable the Symantec DLP Connector using Group Policy:

1. Install the Microsoft Edge administrative template, see https://learn.microsoft.com/en-us/DeployEdge/configure-microsoft-edge
2. Configure any combination of the following 3 settings depending on which user actions you want to be scanned by Symantec's DLP agent
   - **Paste**: `Administrative Templates > Microsoft Edge > Configuration policy for bulk data entry for Microsoft Edge for Business Data Loss Prevention Connectors`
   - **Upload**: `Administrative Templates > Microsoft Edge > Configuration policy for files attached for Microsoft Edge for Business Data Loss Prevention Connectors`
   - **Print**: `Administrative Templates > Microsoft Edge > Configuration policy for print for Microsoft Edge for Business Data Loss Prevention Connectors`
3. Configure the following fields in the policy:
   - Set the `service_provider` to `brcm_edge_cas`.
   - Set `enable` to `[{"tags":["dlp"],"url_list":["*"]}]` to allow all URLs to be scanned.
   - Set the remaining fields as desired.

### Using Microsoft Intune
You can also enable the Symantec DLP Connector using Microsoft Intune via Administrative Templates.

1. Sign in to the [Intune Admin Center](https://intune.microsoft.com).
2. Create or modify an existing policy, see https://learn.microsoft.com/en-us/DeployEdge/configure-edge-with-intune
3. Under the `Configuration settings`, set any combination of the following 3 settings depending on which user actions you want to be scanned by Symantec's DLP agent
   - **Paste**: `Microsoft Edge > Configuration policy for bulk data entry for Microsoft Edge for Business Data Loss Prevention Connectors`
   - **Upload**: `Microsoft Edge > Configuration policy for files attached for Microsoft Edge for Business Data Loss Prevention Connectors`
   - **Print**: `Microsoft Edge > Configuration policy for print for Microsoft Edge for Business Data Loss Prevention Connectors`
4. Configure the following fields in the policy:
   - Set the `service_provider` to `brcm_edge_cas`.
   - Set `enable` to `[{"tags":["dlp"],"url_list":["*"]}]` to allow all URLs to be scanned.
   - Set the remaining fields as desired.
5. Assign the policy to the relevant device group and save.

## Symantec Configuration 

### 1. **Verify** that the Configuration Policy was Deployed Successfully

1. On a Windows endpoint, **sign in** to Microsoft Edge for Business with a valid Microsoft Entra ID.

2. **Navigate** to edge://policy, and **verify** that the following policies are listed and that their **Status is OK**:
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

