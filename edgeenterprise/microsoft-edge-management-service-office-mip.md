---
title: "Protect Office documents with Microsoft Purview Information Protection labeling"
ms.author: jikong
author: dan-wesley
manager: likuba
ms.date: 11/12/2024
audience: ITPro
ms.topic: conceptual
ms.service: microsoft-edge
ms.localizationpriority: high
ms.collection: M365-modern-desktop
description: "Learn about Office Microsoft Purview Information Protection labeling through the Microsoft Edge management service "
---

# Protect Office documents with Microsoft Purview Information Protection labeling through the Microsoft Edge management service

This article explains how to use the Microsoft Purview Information Protection (MPIP) policy and security settings inside the Edge management service to ensure that Office documents are kept secure inside your organization.

## About the use of MPIP

[Microsoft Purview Information Protection (MPIP)](/purview/information-protection) enables data loss prevention (DLP) controls in Microsoft 365 documents by limiting or preventing certain actions on documents with specific sensitivity levels. After a sensitivity label is applied to a document, an admin can prevent actions such as editing, printing, copying/pasting, taking screenshots, and more. This functionality, previously only available in Microsoft 365 desktop applications, is extended to online Office documents via Microsoft Edge to help protect sensitive information.  

When an admin chooses to enable Microsoft Purview Information Protection in the Edge management service, that action will simultaneously disable other browsers that don't respect Microsoft Word, Excel, and PowerPoint rights restrictions. An admin can choose to re-enable other browsers, by using the following instructions. However, the result is a security loophole, where users can avoid rights restrictions simply by opening the Microsoft Word, Excel and PowerPoint documents in another browser.

## Turning on MPIP and managing access to other browsers

You can turn on MPIP in a policy and allow the use of other browsers if MPIP is turned on.

### How to enable the MPIP setting inside a policy

To enable this setting in the Edge management service, navigate within a configuration profile to the **Customization Settings** tab. From there, navigate to the **Security settings** page. If you would like to turn on this setting, check the box that is labeled "Apply sensitivity labels to Microsoft 365 online" and then select "Save changes." For users assigned to this configuration profile, Microsoft 365 online will now be able to access labels managed by MPIP.

### How to allow the use of other browsers while MPIP setting is enabled

The "block other browsers" state is turned on by default when the box labeled "Apply sensitivity labels to Microsoft 365 online" is checked. To allow the use of other browsers, uncheck "Block other browsers" and then select "Save changes." For users assigned to this configuration profile, other browsers remain available.

## See also

- [Microsoft Edge management service](microsoft-edge-management-service.md)
