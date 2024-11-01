---
title: "Microsoft Edge management service and Office MIP labeling"
ms.author: jikong
author: dan-wesley
manager: likuba
ms.date: 11/01/2024
audience: ITPro
ms.topic: conceptual
ms.service: microsoft-edge
ms.localizationpriority: high
ms.collection: M365-modern-desktop
description: "Learn about Office MIP labeling through the Microsoft Edge management service "
---

# Microsoft Edge management service and Office MIP labeling

This article explains how to use the Microsoft Information Protection (MIP) policy and security settings inside the Edge management service to ensure that Office documents are kept secure inside your organization.

## About the use of MIP

MIP supports Data Loss Prevention (DLP) controls in office documents by enabling the use of labels and policies. Sensitivity labels can be applied to different office documents, and policies can be applied to prohibit or limit actions taken on a document based on a specific sensitivity label. This functionality exists today in office applications, but the protections can be bypassed by opening the document in a browser other than Microsoft Edge. Bringing MIP functionality to Edge strengthens DLP. It prohibits the use of other browsers, which prevents users from bypassing these controls by opening documents in alternative browsers where these labels and policies are not honored.  

 

<!----

What is MIP? What business problem does it solve? 

How does blocking alternative browsers make MIP more effective? OR How does access to alternative browsers make MIP ineffective? --->

## How to enable the MIP setting inside a policy

<!-----
Scenarios

The "block alternative browsers" state will be consistent across all pages that contain the setting. We will not have inconsistent states for this setting. 

When Web Content Filtering is configured in any manner, "block alternative browsers" will be automatically enabled and enforced. Users cannot disable this setting on either page. 

When Web Content Filtering is not configured and the MIP label setting is enabled, "block alternative browsers" will be automatically enabled. Users can choose to disable "block alternative browsers" if desired and will see a warning notice if they choose to do so. 

When Web Content Filtering is configured in any manner, "block alternative browsers" will be automatically enabled and enforced on both the Web Content Filtering and MIP label setting pages. Users cannot disable this setting on either page. --->

 

## See also

- [Microsoft Edge management service](microsoft-edge-management-service.md)
