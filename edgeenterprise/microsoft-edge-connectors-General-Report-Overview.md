---
title: "Reporting Connectors"
ms.author: stmoody
author: vmliramichael
manager: venkatk
ms.date: 04/18/2025
audience: ITPro
ms.topic: reference
ms.service: microsoft-edge
ms.localizationpriority: high
ms.collection: M365-modern-desktop
ms.custom: generated
description: "Reporting Connectors"
---

# Reporting Connectors

Microsoft Edge for Business Reporting Connectors enable admins to gain insights into browser-based security events with a direct Connection between Edge for Business and your preferred security solution

## Security Events

The following security events can be enabled in a reporting Connector:

| Event Value               | Event Description                                                                                   |
|---------------------------|------------------------------------------------------------------------------------------------------|
| Browser crash             | Browser or tab crashed (only reported when device-level reporting is available).                    |
| Browser extension install | Extensions are installed, updated, or removed.                                                       |
| Malware transfer (download) | Download blocked by SmartScreen, or download block bypassed/opened by user.                     |
| Unsafe site visit         | SmartScreen blocking page is shown or bypassed.                                                     |
| URL filtering interstitial| Web Content Filtering interstitial is shown (can be from SmartScreen's E5/MCAS or Edge management). |
| Content transfer          | This event will be enabled after V1 of the reporting connector launch.                              |
| Content unscanned         | Content failed to scan for DLP (requires Analysis connector to be configured).                      |
| Sensitive data transfer   | Content marked as sensitive by DLP scan (requires Analysis connector to be configured).             |
| Password changed          | A password is changed in response to a password reuse warning.                                      |
| Password reuse            | A password is detected as reused between an enterprise account and an account on an external site.  |
| Login                     | A sign-in to a domain in the specified list is successful.                                           |
| Password breach           | A password is detected as compromised as part of a known data breach.                               |


## Reporting Providers

| Connector     | Documentation Link                                                                 |
|---------------|-------------------------------------------------------------------------------------|
| Splunk        | [Set up a Splunk Reporting Connector](/deployedge/microsoft-edge-connectors-splunk?branch=pr-en-us-5295)        |
| Devicie       | [Set up a Devicie Reporting Connector](/deployedge/microsoft-edge-connectors-devicie?branch=pr-en-us-5295)       |
| Crowdstrike   | [Set up a Crowdstrike Reporting Connector](/deployedge/microsoft-edge-connectors-crowdstrike?branch=pr-en-us-5295)   |




