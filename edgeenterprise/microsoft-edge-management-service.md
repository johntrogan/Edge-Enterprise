---
title: "Get started with configuration policies"
ms.author: katherinegan
author: vmliramichael
manager: archandr
ms.date: 04/07/2025
audience: ITPro
ms.topic: get-started
ms.service: microsoft-edge
ms.localizationpriority: medium
ms.collection: M365-modern-desktop
description: "Provides steps for configuring the Microsoft Edge management service."
---

# Get started with configuration policies

The Microsoft Edge management service is a platform in the Microsoft 365 admin center that enables admins to easily configure Microsoft Edge browser settings for their organization. These configurations are stored in the cloud and the settings can be applied to a user's browser through group assignment or group policy. Users must be logged into Microsoft Edge to retrieve these settings.

<!-- ====================================================================== -->
## Prerequisites

- You must have Microsoft Edge 115.0.1901.7 or greater installed.
- You must be a [Microsoft Edge Administrator](/azure/active-directory/roles/permissions-reference#edge-administrator) to access the experience in Microsoft 365 Admin Center (Note: GDAP roles are currently not fully supported).
- You must be using one of the following supported operating systems: Windows 10/11 or Windows Server 2016 or later. See [Microsoft Edge Supported Operating Systems](/deployedge/microsoft-edge-supported-operating-systems) for specifics.

> [!IMPORTANT]
>  The Microsoft Edge management service is currently not available to customers with GCC plans and supports management of Windows 10 and 11 devices only.

<!-- ====================================================================== -->
## Access the experience

Use these steps to access the experience:

1. Go to the [Microsoft 365 admin center](https://admin.microsoft.com/Adminportal/Home#/homepage) and sign in.

1. In the main left navigation bar, go to **Settings** > **Microsoft Edge**.  
<!-- ====================================================================== -->

## Get started with configuration policies

A configuration policy file contains all the browser policy configurations, including extension settings.

Each configuration policy can be assigned to multiple Microsoft Entra groups, and a group can be assigned to multiple configuration policies. When a group is assigned to multiple configuration policies, the settings merge if there are no conflicting settings. If a user is a member of multiple Microsoft Entra groups with conflicting policy settings, then the policy priority is used to determine which policy setting is applied. The highest priority is applied, with "0" being the highest priority that you can assign. Please note that Intune configuration policies do not have priority, and any conflicting settings will not be automatically resolved.

#### Cloud policies 

A configuration policy that has been created using the Cloud Policy service will only be available to manage in the Edge management service. The following features are currently only available using a Cloud policy: 

- **Prioritization:** Configuration policies with conflicting settings will - take the value of the policy with the highest priority.  

- **Extension requests:** Admins will be able to view the extensions that users have requested and take action to approve or deny these requests. 

- **Organization branding:** Admins will be able to apply their organization’s branding to customize the look and feel of the browser  

#### Intune policies 

A configuration policy that is created as an Intune policy will be available to manage in both the Edge management service and Intune portal. Within Intune, the policy will appear inside the Configuration section within Devices. The policy details on both platforms will sync, though there are currently some existing limitations: 

- ***Scope tags:*** While configuration policies created in Intune will be able to set scope tags, Intune policies created in the Edge management service will not be able to set these. 

- ***Detailed assignment:*** Configuration policies created in the Edge management service will only be able to be assigned to target user groups. If created in Intune, the configuration policy can target devices as well as exclude certain user groups. Assignment filters can also be applied when created in the Intune portal. 

- **Role-based access control (RBAC):** In Intune, RBAC controls which users can perform actions and make changes to configuration policies. There are no role restrictions in the Edge management service. 

#### Create a configuration policy

Follow these steps to create a configuration policy:

1. Navigate to the ***Configuration policies*** tab.  

2. Select **Create policy**. This takes you through the following wizard flow to create a new configuration policy.  

   a. **Basics:** Give your configuration policy a name. You may also add an optional description. Choose whether you would like to create an Intune type policy or Cloud. You must have an Intune license to be able to create an Intune policy. 

   b. **Settings:** Select **Add setting** to browse through the list of Edge settings that you can configure. Choose the settings you would like to configure for this policy and set their appropriate value. 

   c. **Extensions:** In the **Default extension** settings section, you can modify the default settings that apply to all extensions in this configuration policy. In the **Managed extensions** section, select **Add extension** to add individual extensions (Edge add-on, Sidebar app, or External extension) that you want to manage. Once added, select each extension to edit its specific settings. 

   d. **Assignments:** Choose **Select group** to search for Microsoft Entra groups that you would like to assign this configuration policy to. (Note: If you don't have any existing groups, follow [these instructions](/microsoft-365/admin/email/create-edit-or-delete-a-security-group) to create one). You may also choose to assign this configuration policy to all users in your tenant by selecting **Add all users**. If you create a tenant-wide policy, this cannot be changed after the policy is created. 
 
   e. **Finish:** Make sure that everything on this page looks correct, and then select **Review and create** to create your new configuration policy. 

3. Your new policy should now be visible in the **Configuration policies** list. Select it to view and edit its details on the **Properties** page. 

   a. On the Managed extensions page, you can continue to easily add and configure settings for individual extensions. 

   b. On the Customization settings page, you can also configure specific settings that have been grouped together to help create a secure and productive user experience. Editing settings on any of these pages adds them to the Settings section in the Properties page. 

If you've chosen to create an Intune policy, you can navigate to **intune.microsoft.com > Devices > Configuration** where you should see your newly created configuration policy in this list. 

- **Note:** Any edits you make to settings in Intune or the Edge management service for the same Intune configuration policy should sync. 

 [!Note]
>Any policies you apply with Microsoft Edge management service will be overridden if they conflict with an existing Group Policy Object (GPO) or Mobile Device Management (MDM) policy that's set on the device. 

#### Export a configuration policy

You can export a configuration policy as a JSON file. This export can be used to save a copy of your configurations and can be imported to a different policy.

Follow these steps to export a policy:

1. Select the policy you want to export.

2. Select **Export policy**.

3. Select **Export**.

#### Copy a configuration policy

Follow these steps to copy a configuration policy:

1. Select the ***policy*** you want to make a copy of. 

2. Select **Copy policy**.

3. Under **Copy configuration policy**, enter a policy name and description and then select **Create**.

After confirmation, the new policy is created with the same configurations as the policy you copied.

#### Reorder priority of configuration policy

Follow these steps to reorder the priority of a configuration policy:

1. Select the policy you want to change the priority of and select **Reorder priority.**

2. In the **Reorder policy** priority panel, pick a priority number from the dropdown list. 

3. Select **Save** after you are finished making your changes.  

> [!NOTE]
> Any policies you apply with Microsoft Edge management service will be overridden if they conflict with an existing Group Policy Object (GPO) or Mobile Device Management (MDM) policy that's set on the device.

### Enable the Microsoft Edge management service

Use the following sections as a guide to enable the Microsoft Edge management service.

#### For Microsoft Edge version 115.1935 and later

Microsoft Edge management service is enabled by default. Work policy signed in with Microsoft Entra accounts will check with the Edge management service for any policies assigned to them. If an enrollment token is configured through device management, that token will be used. To disable the checking in with the Edge management service you can set the [EdgeManagementEnabled](/deployedge/microsoft-edge-policies#edgemanagementenabled) policy to 0 or disabled.

### Set an enrollment token

Use the following sections as a guide to setting an enrollment token.

#### For Microsoft Edge version 115.1935 and later

If you don't want to assign the policy using group assignment in the Microsoft 365 Admin Center, then you can assign it through group policy. Each policy has a unique policy ID which is the value you can use for the [EdgeManagementEnrollmentToken](/deployedge/microsoft-edge-policies#edgemanagementenrollmenttoken) policy to assign the policy. After assignment, the users will receive the policy and the settings will be applied when they're signed into the Edge browser. These policies will be applied in addition to any from group assignment in the Microsoft 365 Admin Center.

Use these steps as a guide for setting an enrollment token:

1. Sign in to the Microsoft 365 Admin Center. Go to **Settings** > **Microsoft Edge**. Under the **Configuration policies** pivot, select the policy you want to assign and then click **Deploy** to select **Copy policy ID**.

2. Set the [EdgeManagementEnrollmentToken](/deployedge/microsoft-edge-policies#edgemanagementenrollmenttoken) policy value to the token ID. 

3. If Microsoft Edge is open, restart it.

#### Control policy source precedence

As stated previously, if policy is set in MDM or GPM, that value will override any value provided by Microsoft Edge management service. If you want the Microsoft Edge management service policy to override MDM/GPM policy you can set the override in the  [EdgeManagementPolicyOverridesPlatformPolicy](/deployedge/microsoft-edge-policies#edgemanagementpolicyoverridesplatformpolicy) policy. This is a private policy and must be set via the registry.

Set the value of [EdgeManagementPolicyOverridesPlatformPolicy](/deployedge/microsoft-edge-policies#edgemanagementpolicyoverridesplatformpolicy) under the key `SOFTWARE\Policies\Microsoft\Edge` in either `HKLM` or `HKCU`. If the key isn't there you can create it. In the following command line example, remember to use your token ID and restart Microsoft Edge if it's open.

```
reg add HKLM\Software\Policies\Microsoft\Edge /v EdgeManagementPolicyOverridesPlatformPolicy /t REG_ DWORD /d 1 
```

#### Control user/device policy precedence

Microsoft Edge policy has the concept of the audience that the policy is meant to apply to, this can be either "User" or "Device". In Microsoft Edge management service, the policy applied via Group Assignment is applied as User Policy, while policy pulled down via [EdgeManagementEnrollmentToken](/deployedge/microsoft-edge-policies#edgemanagementenrollmenttoken) is applied as Device Policy.

If there's a conflict with policy that User and Device are both trying to set, Device Policy takes precedence over User Policy. If you want to give User Policy precedence you can change precedence in [EdgeManagementUserPolicyOverridesCloudMachinePolicy](/deployedge/microsoft-edge-policies#edgemanagementuserpolicyoverridescloudmachinepolicy) policy.

1. You can set precedence via the registry by setting the value of "EdgeManagementUserPolicyOverridesCloudMachinePolicy" under the key `SOFTWARE\Policies\Microsoft\Edge` in either `HKLM` or `HKCU`. If the key isn't there, create it.
2. Add the reg key using the following command line example as a guide. (Remember to use your policy ID.)

   ```
   reg add HKLM\Software\Policies\Microsoft\Edge /v EdgeManagementUserPolicyOverridesCloudMachinePolicy /t REG_ DWORD /d 1 
   ```

3. If Microsoft Edge is open, restart it.

#### How the configuration policy is applied

Once a configuration policy is created and applied, Microsoft Edge checks with Cloud Policy regularly to see if there are any configuration policies that pertain to the user. If there are, then the appropriate policy settings are applied and take effect the next time the user opens Microsoft Edge.

**Here's a summary of what happens:**

- When a user signs into Microsoft Edge on a device for the first time, a check is immediately made to see if there's a configuration policy that pertains to the user.
- If the user isn't a member of a Microsoft Entra group that's assigned a configuration policy, then another check is made again in 24 hours.
- If the user is a member of a Microsoft Entra group that's assigned a configuration policy, then the appropriate policy settings are applied. A check is made again in 90 minutes.
- If there are any changes to the configuration policy since the last check, then the appropriate policy settings are applied and another check is made again in 90 minutes.
- If there aren't any changes to the configuration policy since the last check, another check is made again in 24 hours.
- If there's an error, a check is made when the user opens Microsoft Edge.
- If Microsoft Edge isn't running when the next check is scheduled, then the check will be made the next time the user opens Microsoft Edge.

> [!NOTE]
>
> - Policies from Cloud Policy are only applied when Microsoft Edge is restarted. The behavior is the same as with Group Policy. For Windows devices, policies are enforced based on the primary user that is signed into Microsoft Edge. If there are multiple accounts signed in, only policies for the primary account are applied. If the primary account is switched, most of the policies assigned to that account will not apply until Microsoft Edge is restarted. Some policies related to [privacy controls](/deployoffice/privacy/overview-privacy-controls) will apply without restarting Microsoft Edge.
> - If users are located in nested groups and the parent group is targeted for policies, the users in the nested groups will receive the policies. The nested groups and the users in those nested groups must be created in or synchronized to Microsoft Entra ID.
> - If the user is a member of multiple Microsoft Entra groups with conflicting policy settings, priority is used to determine which policy setting is applied. The highest priority is applied, with "0" being the highest priority that you can assign. You can set the priority by choosing **Reorder priority** on the **Configuration policy** page.

<!-- ====================================================================== -->
## Feedback and support

This experience is supported by [Microsoft Support](https://support.microsoft.com/microsoft-edge). You can reach out to Microsoft Support to report issues or give feedback. You can also leave feedback in our [TechCommunity forum](https://techcommunity.microsoft.com/t5/enterprise/bd-p/EdgeInsiderEnterprise).
<!-- ====================================================================== -->
## See also

- [Microsoft Edge Enterprise landing page](https://aka.ms/EdgeEnterprise)
