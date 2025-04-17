---
title: "Ping Identity"
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
description: "Ping"
---

# Setup a Ping Identity Connector 

The Microsoft Edge for Business connector lets you use Microsoft Edge for Business to improve authentication security in your PingOne DaVinci flow.

Microsoft Edge for Business is a secure, high-performance browser built for enterprise needs, offering enhanced productivity, AI-powered features, and native integration with Microsoft 365—designed to protect corporate data while supporting modern workplace demands.

You can use the Microsoft Edge for Business connector to include operating system device signals collected by Microsoft Edge for Business in a PingOne DaVinci flow.

## Connector Setup and Configuration Steps

### Resources

For information and setup help, see the following:

- Microsoft Edge for Business documentation  
  https://www.microsoft.com/en-us/edge/business/?form=MA13FJ

- Register an application with the Microsoft identity platform

- DaVinci documentation:
  - Adding a connector
  - Using connectors securely
  - Using DaVinci flow templates

## Requirements

To use the Microsoft Edge for Business PingOne DaVinci connector you must have access to register an application through Microsoft Entra and assigning it the required Device Trust permissions. As well, access to the Microsoft 365 admin center is required to configure the Edge for Business Policies.

## Setting up Microsoft Edge for Business

To use the connector, you’ll need:

- Administrator access to Microsoft Azure
- An Azure App Registration for the Microsoft Edge for Business Device Trust integration.
- Administrator access to Microsoft 365 admin center for Microsoft Edge for Business policy configuration.

### Setting up Azure App Registration

1. Sign on to the Azure portal.
2. Create the application:
   - Search for and select Azure Active Directory.
   - Under Manage, select **App registrations** → **New registration**.
   - Register a new Application and select the newly registered application.
   - Configure the required permissions on the newly created App Registration to give the application permissions to access the Device Trust API.
   - Search for the **Microsoft Edge management service** in the *APIs my organization uses* tab.
   - Select **Application permissions** and add the `DeviceTrust.Read.All` permission.
   - Once added, click the **Grant admin consent** confirmation.
   - Click **Register**.

On your app’s Overview page, note the **Application (client) ID** and **Directory (tenant) ID**. You’ll use these in the connector configuration.  
*A screen capture of the application details page in Microsoft Azure.*

### Create a client secret:

- Under Manage, click **Certificates & secrets**. On the *Client secrets* tab, click **New client secret**.
- Enter a name and select an expiry time. Click **Add**.
- Note the **Value** of the secret. You’ll use this in the connector configuration.  
*A screen capture of the client secret in Microsoft Azure.*

## Configuring Edge for Business for PingOne DaVinci

1. Sign on to **Microsoft 365 admin center**.
2. Navigate to the **Microsoft Edge configuration**.
3. Navigate to the **Connectors** tab and click **Set up** under the **Ping Identity Device Trust** feature.
4. In the right panel put in the following PingOne DaVinci domains:
   - auth.pingone.com
   - auth.pingone.ca
   - auth.pingone.eu
   - auth.pingone.asia
   - auth.pingone.au
5. Click **Save Configuration**

The Microsoft Edge for Business Device Trust is now configured.

## Configuring the Microsoft Edge for Business connector

Add the connector in DaVinci as shown in *Adding a connector*, then configure it as follows.

### Connector configuration

- **Azure Tenant ID**  
  The tenant ID of your Microsoft Azure Tenant.

- **Client ID**  
  The client ID you created in *Setting up Microsoft Edge for Business*.

- **Client Secret**  
  The client secret you created in *Setting up Microsoft Edge for Business*.

## Using the connector in a flow

### Device Trust

The Device Trust capability allows PingOne DaVinci to receive the Microsoft Edge for Business Device Signals which include the device attributes such as Serial Number, MAC Addresses, and Hostname. Also, the CrowdStrike agent ID is included if the CrowdStrike agent is installed.

See below for an example of a PingOne DaVinci flow which blocks access to users who are not using the expected Microsoft Edge for Business enrolled browser:


## Configure the Connector in the Edge Management Service   

1. **Navigate to the Microsoft Admin Center**  
   Go to [https://admin.microsoft.com/Adminportal/Home#/Edge/Connectors](https://admin.microsoft.com/Adminportal/Home#/Edge/Connectors)

2. **Discover the Connector**  
   Under **Discover Connectors**, locate the **Ping Identity Connector** and select **Set up**.

3. **Select a Policy**  
   In the **Choose policy** field, select a policy appropriate for your connector configuration.

4. **Enter URL Patterns**  
   In the **URL patterns to allow, one per line** field, input. 
   - auth.pingone.com
   - auth.pingone.ca
   - auth.pingone.eu
   - auth.pingone.asia
   - auth.pingone.au

5. **Save the Configuration**  
   Select **Save configuration** to apply your changes.



