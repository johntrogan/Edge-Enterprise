---
title: "Microsoft Edge Data Loss Prevention"
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
description: "Data Loss Prevention"
---

# Content Data Loss Prevention Connectors

Microsoft Edge for Business Data Loss Prevention connectors enable Microsoft Edge for Business to natively enforce DLP (Data Loss Prevention) verdicts from on-device agents.  
When enabled, Microsoft Edge sends content from specific user actions to the on-device agent and waits for the verdict before proceeding.

## User Actions

The following user actions can send content to the Data Loss Prevention connector:

- Paste  
- Print  
- Upload  

## Create a Configuration Policy

Admins must have a configuration profile set up as a prerequisite for configuring a connector. [Follow this guide to create a configuration profile](https://review.learn.microsoft.com/en-us/deployedge/microsoft-edge-management-service?branch=pr-en-us-5295).

## Set Up a Data Loss Prevention Connector
Visit https://admin.microsoft.com/Adminportal/Home#/Edge/Connectors to access the connectors page in the Edge Management service.

- [Symantec DLP](https://review.learn.microsoft.com/en-us/deployedge/microsoft-edge-connectors-duo?branch=pr-en-us-5295)
