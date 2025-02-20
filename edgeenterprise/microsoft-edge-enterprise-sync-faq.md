---
title: "Microsoft Edge enterprise sync FAQ"
ms.author: archandr
author: dan-wesley
manager: likuba
ms.date: 01/28/2025
audience: ITPro
ms.topic: conceptual
ms.service: microsoft-edge
ms.localizationpriority: medium
ms.collection: M365-modern-desktop
description: "Frequently asked questions about Microsoft Edge enterprise sync."
---

# Microsoft Edge enterprise sync FAQ

This article answers frequently asked questions about enterprise sync for Microsoft Edge version 77 or later.

## Security and Server/Data compliance

### Is the synced data encrypted?

Yes, the data is encrypted in transport using TLS 1.2 or greater. All data types are additionally encrypted at rest in Microsoft's service using AES128. All data types except the data used for open tab and history sync are additionally encrypted before leaving the user's device with keys managed via the [Azure Information Protection](./microsoft-edge-policies.md#restrictsignintopattern) policy.

### Why isn't there more client-side encryption on open tab and history data?

To reduce resource utilization on end-user devices, history data is generated server-side based on open tab roaming data. This process wouldn't be possible with client-side encryption of this data. To disable open tab and history sync, apply the [SavingBrowserHistoryDisabled](./microsoft-edge-policies.md#savingbrowserhistorydisabled) or [SyncTypesListDisabled](./microsoft-edge-policies.md#synctypeslistdisabled) policies.

### Can tenant admins bring their own key?

Yes, through [Microsoft Purview Information Protection | Microsoft Security](https://www.microsoft.com/en-us/security/business/information-protection/microsoft-purview-information-protection).

### Where is Microsoft Edge sync data stored?

Synced data for Microsoft Entra accounts is stored on secure servers according to the tenant ID. For example, the data for a tenant that is registered in the United States is stored in servers geo-located for that region and uses the same storage solution as Office applications.

### Does the data ever leave Microsoft's cloud, aside from syncing to Microsoft Edge?

No.

### What terms of service does enterprise sync fall under?

Terms of service for Microsoft Edge sync fall under the Microsoft software license viewable in Microsoft Edge at *edge://terms*. Your Microsoft Entra subscription and terms of service ultimately fall under Microsoft's [Online Service Terms](https://www.microsoft.com/licensing/product-licensing/products).

### Does Microsoft Edge support Government Community Cloud (GCC) High and Azure Government Department of Defense (DoD) Cloud compliance?

Not today. For customers in the GCC High cloud and Azure Government DoD cloud, Microsoft Edge sync is disabled.

### Does Microsoft Edge sync support Microsoft Azure operated by 21Vianet?

Not today. For customers in Microsoft Azure operated by 21Vianet, Microsoft Edge sync is not supported.

## Applying Sync

### Is Microsoft Edge sync based on Enterprise State Roaming?

No. ESR can be used to enable sync, but Microsoft Edge sync isn't a part of ESR. For more information, see [Microsoft Edge Sync](/DeployEdge/microsoft-edge-enterprise-sync) and [Microsoft Edge and Enterprise State Roaming](/DeployEdge/microsoft-edge-enterprise-state-roaming).

### Will Microsoft Edge ever support syncing between Microsoft Edge and IE?

There are no plans to support this syncing. If you still need IE in your environment to support legacy apps, consider our [new IE mode](./edge-ie-mode.md).

### Will Microsoft Edge sync with Microsoft Edge Legacy?

No, it won't. We believe connecting these two ecosystems will lead to compromises in the reliability of sync in the Microsoft Edge. We'll ensure that existing data is migrated to the Microsoft Edge. Users will also be able to import data from browser of their choice, which also means that Microsoft Edge won't have a way to sync with IE.

## Managing Sync

### Is it possible to stop my users from syncing with a personal tenant?

Not directly, but you can determine which profiles can sign on to Microsoft Edge using the [RestrictSigninToPattern](./microsoft-edge-policies.md#restrictsignintopattern) policy.

### Is it possible to prevent sign-in and sync with an enterprise account on an unmanaged/non-compliant device?

Currently it's not possible to prevent Microsoft Entra sign-in to Microsoft Edge on unmanaged devices without disrupting your other Conditional Access (CA) protected applications. However, enterprise sync can be blocked on such devices by adding the "Microsoft Azure Information Protection" app to the CA policy.

## See also

- [Microsoft Edge Enterprise Sync](microsoft-edge-enterprise-sync.md)
- [Microsoft Edge and Enterprise State Roaming](microsoft-edge-enterprise-state-roaming.md)
- [Microsoft Edge Enterprise landing page](https://aka.ms/EdgeEnterprise)
