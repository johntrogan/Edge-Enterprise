---
title: "Microsoft Edge in your environment"
ms.author: archandr
author: dan-wesley
manager: likuba
ms.date: 11/25/2024
audience: ITPro
ms.topic: conceptual
ms.service: microsoft-edge
ms.localizationpriority: medium
ms.collection: M365-modern-desktop
description: "Microsoft Edge in your environment"
---

# Microsoft Edge in your environment

> [!IMPORTANT]
> This article applies to Microsoft Edge Legacy. Support for the Microsoft Edge Legacy desktop application ended on March 9, 2021. For more information, see [Microsoft Edge Legacy - Microsoft Lifecycle | Microsoft Learn](/lifecycle/products/microsoft-edge-legacy). We’re no longer updating "Microsoft Edge in your environment" regularly.  

This article describes how to prepare to deploy Microsoft Edge when Microsoft Edge Legacy reaches its end of service.

As per the Microsoft Edge Product Team's [blog post](https://aka.ms/EdgeLegacyEOS), support for the Microsoft Edge Legacy desktop application will end on March 9, 2021. When you apply the Update Tuesday (or "B") release in April, it will remove Microsoft Edge Legacy from devices running Windows 10 April 2018 Update through Windows 10 April 2020 Update and replace it with Microsoft Edge.

## How to Prepare

To prepare for Microsoft Edge being installed on Windows 10 April 2018 Update through Windows 10 April 2020 Update devices with the Update Tuesday release in April, we recommend reading [Plan your deployment of Microsoft Edge](deploy-edge-plan-deployment.md).

After you plan your deployment, use one of the following approaches to prepare to deploy Microsoft Edge.

- **Install group policies to customize your Microsoft Edge update approach**. For more information, see [Configure Microsoft Edge policy settings on Windows](configure-microsoft-edge.md), and pay special attention to the [Update Policy reference](microsoft-edge-update-policies.md) material. If you install group policies to manage your updates before installing April's Update Tuesday release, Microsoft Edge will immediately start respecting your policy. If there isn't any installed group policy, Microsoft Edge will automatically update itself.

- **Remove the Microsoft Edge Legacy desktop application before its end of service date of March 9, 2021, and deploy Microsoft Edge**. For Windows 10 April 2018 Update through Windows 10 April 2020 Update, you can do this by using Windows Updates. For more information, see [Deploy Microsoft Edge with Windows 10 updates](deploy-edge-with-windows-10-updates.md).

## See also

- [Microsoft Edge Enterprise landing page](https://aka.ms/EdgeEnterprise)
- [Plan your deployment of Microsoft Edge](deploy-edge-plan-deployment.md)