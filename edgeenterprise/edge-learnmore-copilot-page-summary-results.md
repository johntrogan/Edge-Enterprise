---
title: "Copilot in Edge webpage summarization behavior"
ms.author: prithviokade
author: dan-wesley
manager: likuba
ms.date: 11/07/2024
audience: ITPro
ms.topic: reference
ms.service: microsoft-edge
ms.localizationpriority: medium
ms.collection: M365-modern-desktop
description: "This article shows the results of Copilot page summary tests."
---

# Copilot in Edge webpage summarization behavior

The charts below illustrate scenarios in which Copilot in Edge for Business may access page content across different document types. This information will be updated when support for summarization increases. This chart covers the behavior of Microsoft 365 Copilot Chat in Edge for Business which is accessible in the sidepane.  

> [!NOTE]
> Contextual grounding in Copilot in Edge: This is the ability to ground a chat conversation in the current webpage context. It applies to prompts such as "Summarize this document" or "What does this page say about…" in reference to the tab currently being viewed by the user in the main Edge window. Contextual grounding only applies to instances of chat when using Copilot in the Edge sidebar, because desktop/full-screen instances do not allow for simultaneous web context.

| Document type                    | Copilot access to page content                                     |
|----------------------------------|---------------------------------------------------------------------|
| Microsoft 365 Copilot Chat       | Copilot access to page content is supported                        |
| Intranet Sites such as SharePoint| Copilot access to page content is supported  <br> *Embedded Office docs in SharePoint aren't supported* |
| Public Sites such as Wikipedia   | Copilot access to page content is supported                        |
| Outlook Web App                  | Copilot access to page content is supported                        |
| PDFs                             | Copilot access to page content is supported                        |
| Office Documents                 | Copilot access to page content isn't supported                     |


## Blocking Copilot Chat in Edge for Business Access to Page Content through DLP

Edge for Business is integrated with Microsoft Purview and Intune MAM to provide Copilot blocking mechanisms through DLP. The table below outlines all the policies and their setting value for which Copilot will be **BLOCKED** from accessing page content.

| DLP Provider                            | Policy             | Policy Value |
|----------------------------------------|--------------------|--------------|
| **Microsoft Purview**                  | Copy               | Block or override |
|                                        | Print              | Block or override |
|                                        | Save Webpage As    | Block or override |
| **Intune MAM**                          | Clipboard          | Block |
|                                        | Print              | Block |
|                                        | Upload             | Block |
|                                        | Download           | Block |
| **Microsoft Purview Session Policies** | Download           | Block |
|                                        | Copy               | Block |
|                                        | Print              | Block |
|                                        | Dev tools          | Block |
| **Microsoft Purview Information Protection (MIP)***For Office documents* |  Extract | Block |

---

## Blocking Copilot Chat in Edge Access to Page Content through Group Policy

Please use our [EdgeEntraCopilotPageContext](/deployedge/microsoft-edge-browser-policies/edgeentracopilotpagecontext) group policy to block Copilot’s access to page content in your tenant.  


## See also

- [Microsoft Edge Enterprise landing page](https://aka.ms/EdgeEnterprise)
