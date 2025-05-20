---
title: "Configure Web Content Filtering on Edge"
ms.author: ssatti
author: vmliramichael
manager: vesesha
ms.date: 05/20/2025
audience: ITPro
ms.topic: reference
ms.service: microsoft-edge
ms.localizationpriority: high
ms.collection: M365-modern-desktop
ms.custom:
description: "Configure Web Content Filtering on Edge using Edge management service "
---

# Configure Web Content Filtering on Edge

This article describes how to configure Web Content Filtering (WCF) for Microsoft Edge.

## Introduction

Microsoft Edge is already one of the most secure browsers with features like phishing protection, typosquatting, and more to protect users when they're browsing online. Adding to these security features, Microsoft Edge is introducing Web Content Filtering (WCF) for EDU and SMB Institutions to help them keep students and employees safe online. Using this feature, you can choose [categories of websites](edge-learnmore-wcf-supported-categories.md) that users aren't allowed to access while using Microsoft Edge.

To use this feature, set it up via the Microsoft Edge management service using the following the steps.

> [!NOTE]
> The feature is in public preview.

## Prerequisites

Before you can set up WCF you must meet or exceed the following prerequisites.

1. On managed Windows devices where WCF policy needs to be applied:  
   - Be signed in with school account on a device running Windows 10 or later.
   - Have Microsoft Edge Version 135 or higher installed.
2. You must be a [Microsoft Edge Administrator](https://learn.microsoft.com/en-us/entra/identity/role-based-access-control/permissions-reference#edge-administrator) or a [Global Administrator](https://learn.microsoft.com/en-us/entra/identity/role-based-access-control/permissions-reference#global-administrator) to access this experience in Microsoft 365 Admin Center.
3. Your organisation must have a M365 A1/A3/A5 license, Business Premium license, or Business Basic or Standard license with Intune Plan 1 or 2.

> [!NOTE]
> Make sure you update Microsoft Edge to latest version on all the managed devices where you want to run Web Content Filtering (WCF).

## Setup steps

This section describes and illustrates the six basic steps for setting up WCF:

- [Create a security group to enable WCF](#create-a-security-group-to-enable-wcf)
- [Enable WCF for a Security group](#enable-wcf-for-a-security-group)
- [Manage exceptions via Allowlist and Blocklist](#manage-exceptions-via-allowlist-and-blocklist)
- [Enable Diagnostic data (Optional)](#enable-diagnostic-data-optional)
- [Assign the WCF policy to a group](#assign-the-wcf-policy-to-a-group)
- [Verify that the WCF policy got applied](#verify-that-the-wcf-policy-got-applied)

### Create a security group to enable WCF

> [!TIP]
> If you have pre-existing groups in Intune, they will be automatically imported to the Edge management service. You can reuse them here without any additional work.

To create a group on the Edge management service, open the Microsoft 365 admin center.

1. Go to **Active teams & groups** > **Security groups**, and then select **Add a security group**.

![Add a security group under Active teams & groups.](media/microsoft-edge-web-content-filtering/edge-wcf1-teams-and-groups.png)

2. Under **Set up the basics**, enter a **Name** and **Description** for the group and then select **Next** to create the group.

![Provide name and description in Setup the basics.](media/microsoft-edge-web-content-filtering/edge-wcf2-basics-name-description.png)

3. Under **Active teams and groups**, select the  group you created and then go the **Members** section. Select **View all and manage members** to add **Owners** and **Members** to the group.

![Under Active teams & groups select the group you created.](media/microsoft-edge-web-content-filtering/edge-wcf3-view-manage-members.png)

4. On the **Members** panel, select **Add members**. 

![Select Add members on Members panel.](media/microsoft-edge-web-content-filtering/edge-wcf4-add-members.png)

5. On the **Add members** panel, under **Display name**, check the members you want to add. Select the **Add** button, which displays the number of members you picked.

![Pick members on the Add members list.](media/microsoft-edge-web-content-filtering/edge-wcf5-pick-members.png)

> [!TIP]
> We recommend that you test the policy on a small set of user groups before organisation wide rollout.

> [!NOTE]
> Microsoft Edge management service currently only supports assignment of policies to user groups and not device groups.

### Enable WCF for a Security group

To enable WCF for a security group:

1. From the Microsoft 365 admin center, navigateGo to Settings -> Microsoft Edge -> Configuration policies.

2. If you don’t yet have a configuration policy in the Edge management service assigned to your target security group, create one by following these steps: [Create a configuration policy.](https://learn.microsoft.com/en-us/deployedge/microsoft-edge-management-service#create-a-configuration-policy)

3. Navigate to your desired configuration policy by clicking on it. 
 
![Add name and description for configuration policy.](media/microsoft-edge-web-content-filtering/edge-wcf6-create-cfg-policy.png)

4. From the configuration policy, navigate to Customization Settings -> Web content filtering.  

5. Under Web content filtering there is a list of categories that you can block. Under Blocked categories, check all the categories that you want to  block and then select Save changes. 

![Pick blocked categories for Web content filtering.](media/microsoft-edge-web-content-filtering/edge-wcf7-filter-blocked-categories.png)

> [!IMPORTANT]
> To ensure full safety for students, enabling this policy will block all third-party browsers because they do not have a web content filtering feature.

Users with configured security settings may still be at risk on other browsers. To mitigate this risk, enabling web content filtering through the Edge management service also blocks user access to other browsers. When WCF is enabled, a new configuration policy will be created in Intune. Any modifications you make to this new policy in Intune or in a configuration policy with identical groups in the Microsoft Edge management service may lead to unexpected behaviors. 

### Manage exceptions via Allow and Blocklist

With the necessary categories blocked, you can check the behavior for the top used URLs in your institution and use the Allow and Blocklist capabilities to manage any exceptions.

If you want to allow a particular URL that is part of a blocked category, then you can add the URL to the list of Allowed Sites by the following steps.

1. Under Web content filtering, select **Allowed Sites**.
2. Type in the URL of the site you want to allow and then select "**+**" to add the site.
3. Select **Save Changes**.

![Enter URL for allowed sites in Web content filtering.](media/microsoft-edge-web-content-filtering/edge-wcf8-allowed-urls.png)

> [!TIP]
> Instead of adding the URLs manually, you can import them in bulk using a .csv or .json file with the **Import** option. You could also bulk export the list if you want to re-use it for a different group/policy. 

Similarly, if you want to block a particular URL or list of URLs, you can repeat the previous steps in the **Blocked sites** section.
 
![Enter URL for blocked sites in Web content filtering.](media/microsoft-edge-web-content-filtering/edge-wcf9-blocked-urls.png)

> [!NOTE]
> In addition to specific URLs you can use URL patterns with supported wildcard characters. Refer to this [page](/DeployEdge/edge-learnmmore-url-list-filter%20format)

> [!IMPORTANT]
> URLs added to the Allowed sites list takes will take precedence over the Blocked sites list and Blocked categories. You can read more about this [here](/deployedge/microsoft-edge-policies#urlallowlist).

### Enable Diagnostic data (Optional)

Web Content Filtering (WCF) on Microsoft Edge is in preview and our aim is to make it as safe and seamless as possible. For us to be able to watch the behavior of this feature and diagnose any issues that might arise during the preview, we recommend that you enable **Optional data** on the devices that you're enabling WCF on. Microsoft values your privacy, and we won't collect or use personal data.

1. To enable **Diagnostic data** open the policy configuration page and go to **Settings**.
2. Select **Add setting**.
  
![Open policy configuration page to add a setting.](media/microsoft-edge-web-content-filtering/edge-wcf10-policy-add-setting.png)

3. Search for "DiagnosticData" and on the **Configure a setting** panel, under **Required data**, set the value to **Optional data**.
4. Select **Save**.
 
![Search for DiagnosticData and configure Optional data as Required.](media/microsoft-edge-web-content-filtering/edge-wcf11-required-optional-data.png)

### Assign the WCF policy to a group

Now that the policy has WCF, Allowlist & Blocklist, and Diagnostic data settings configured you can assign this policy to a group.

1. On the policy page, select **Assignment**.
2. Click **+ Select Group** and then click **Select group** to add the groups.

![Pick Assignment on policy page to select a group.](media/microsoft-edge-web-content-filtering/edge-wcf12-assignment-select-group.png)

3. On the **Select a security group** panel, add the groups you want to assign the policy to and then click **Select**.
  
![Enter group name for groups to add.](media/microsoft-edge-web-content-filtering/edge-wcf13-security-add-group-name.png)

### Verify that the WCF policy was applied correctly

You can check whether the policy was applied to a user's Edge browser by navigating to edge://settings/privacy. Under **Privacy, search, and services** you should see that **Web content filtering** is enabled.
 
![Check Web content filtering in Edge Settings.](media/microsoft-edge-web-content-filtering/edge-wcf14-edge-settings-verify-wcf.png)

When you try to access a site that WCF blocks, you should see a screen like the one in the next screenshot.
 
![Prompt to get permission to access blocked site.](media/microsoft-edge-web-content-filtering/edge-wcf15-site-perm-prompt.png)

> [!NOTE]
> It can take up to 90 minutes for policies set via Edge management service to be applied to user devices.

> [!TIP]
> If you have the same policy setup via Intune and EMX, Intune policy takes precedence by default. You can override this default behavior using the [EdgeManagementPolicyOverridesPlatformPolicy](/deployedge/microsoft-edge-policies#edgemanagementpolicyoverridesplatformpolicy) and the  [EdgeManagementUserPolicyOverridesCloudMachinePolicy](/deployedge/microsoft-edge-policies#edgemanagementuserpolicyoverridescloudmachinepolicy) settings in the browser policy documentation.

## See also

- [Microsoft Edge management service](/deployedge/microsoft-edge-management-service)
- [Microsoft Edge Enterprise landing page](https://aka.ms/EdgeEnterprise)