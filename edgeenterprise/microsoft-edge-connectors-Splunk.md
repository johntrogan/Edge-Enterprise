---
title: "Microsoft Edge Splunk"
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
description: "Splunk"
---

# Set up a Splunk Connector Overview

Integrating Splunk with Edge for Business enables organizations to better collect, analyze, and extract insights from security events. Send browser events directly to Splunk for more visibility across managed browsers to make better-informed security decisions.  

## Set up an HTTP Event Collector 

Follow the steps [here](https://docs.splunk.com/Documentation/Splunk/9.4.1/Data/UsetheHTTPEventCollector) to set up an HTTP event collector in Splunk.  

## Configure the Connector in the Edge Management Service

1. Navigate to [Microsoft Admin Center](https://admin.microsoft.com/Adminportal/Home#/Edge/Connectors).

2. Under **Discover Connectors**, find the **Splunk Reporting Connector** and select **Set up**.

3. In the **Choose policy** field, select a policy for your Connector configuration.

4. Enter the following fields:
   - **Host address**
   - **Port**
   - **Token ID**

5. Select **Test Connection** to confirm the Connection is successful.

6. Under **User & Browser events**, select the desired browser events to be sent to the Devicie endpoint.

7. Select the desired **Optional events** and **Devices events**.

8. Select **Save configuration**.

## See the Events in Splunk

Once you have set up the HTTP event collector and have configured the connector in the Edge Management Service, you will start to see the events show up in Splunk.
