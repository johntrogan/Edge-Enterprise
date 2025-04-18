---
title: "Microsoft Edge Data Loss Prevention"
ms.author: stmoody
author: vmliramichael
manager: venkatk
ms.date: 04/16/2025
audience: ITPro
ms.topic: reference
ms.service: microsoft-edge
ms.localizationpriority: high
ms.collection: M365-modern-desktop
ms.custom: generated
description: "Data Loss Prevention Connectors"
---

# Data Loss Prevention Connectors

Microsoft Edge for Business Data Loss Prevention connectors enable Microsoft Edge for Business to natively enforce DLP (Data Loss Prevention) verdicts from on-device agents.  
When enabled, Microsoft Edge sends content from specific user actions to the on-device agent and waits for the verdict before proceeding.

## User Actions

The following user actions can send content to the Data Loss Prevention connector:

- Paste  
- Print  
- Upload  

## Set up a Data Loss Prevention Connector

Admins must set up a configuration policy to assign to any connector configuration. [Follow this guide to create a configuration profile](https://review.learn.microsoft.com/en-us/deployedge/microsoft-edge-management-service?branch=pr-en-us-5295).

Once you have at least one configuration policy created, visit [the Connectors page in the Edge Management Service](https://admin.microsoft.com/Adminportal/Home#/Edge/Connectors) to access the Connectors page in the Edge Management Service.


## Data Loss Providers

| Connector         | Documentation Link                                                                 |
|-------------------|-------------------------------------------------------------------------------------|
| Symantec DLP   | [Set up a Symantec DLP Data Loss Connector](https://review.learn.microsoft.com/en-us/deployedge/microsoft-edge-connectors-duo?branch=pr-en-us-52955) |    

