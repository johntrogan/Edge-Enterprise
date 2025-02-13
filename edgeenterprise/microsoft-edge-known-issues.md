---
title: "Microsoft Edge known issues"
ms.author: archandr
author: dan-wesley
manager: likuba
ms.date: 01/17/2025
audience: ITPro
ms.topic: conceptual
ms.service: microsoft-edge
ms.localizationpriority: high
ms.collection: M365-modern-desktop
description: "Microsoft Edge known issues, workarounds, and fixes"
---

# Microsoft Edge known issues

This article tracks the known issues, workarounds, and fixes for Microsoft Edge.

## High impact issues

These issues are high impact as identified by Customer Service & Support. Check this article often as the Microsoft Edge team provides workarounds and fixes.

The following table lists the issues that the Microsoft Edge team is tracking closely, working on, or resolved.

<!--------------------------------->
<!------ TAB 1 OPEN --------------->
<!--------------------------------->

## [**Open issues**](#tab/Open)

|  Version  | Symptom | Workaround | Comment |
| --- | --- | --- | --- |
| 133 | Customers may not be able to start the sync functionality or open AIP-protected PDF files in Microsoft Edge. A bug in Microsoft Edge version 133 is causing excessive traffic to the MIP service, which has resulted in the temporary blocking of sync functionality and the inability to open AIP-protected PDF files in Edge. | For sync functionality to resume, users can "sign-out (keeping locally saved data)"and then "sign-in" again.  For AIP-protected PDF files, please use other tools such as the Azure Information Protection Viewer. | We are working to release a fix for Microsoft Edge as soon as possible. |
| 130 | In Microsoft Edge Stable Version 130.0.2849.46, non-special scheme URL handling was updated to become compliant with the URL Standard ([https://url.spec.whatwg.org/](https://url.spec.whatwg.org/)). This change has site compatibility impacts which may require changes to your web sites. For more information and web developer guidance, see [http://bit.ly/url-non-special](http://bit.ly/url-non-special). | Ensure your clients receive configuration payloads by either not configuring the [ExperimentationAndConfigurationServiceControl](/deployedge/microsoft-edge-policies#experimentationandconfigurationservicecontrol) policy or setting the policy to "FullMode" or "ConfigurationsOnlyMode". Alternatively, roll back to Microsoft Edge to version 129.0.2792.89. |  Recognizing the broad impact this issue is having, Microsoft decided to temporarily disable this feature through the [Experimentation and Configuration Service (ECS)](/deployedge/edge-configuration-and-experiments). This feature disablement is now fully rolled out to Edge 130 Stable (100%), so it is expected that this will take effect after a browser restart.<br><br>In addition, for enterprises [where ECS is disabled through policy](/deployedge/microsoft-edge-policies#experimentationandconfigurationservicecontrol), a code change to temporarily disable this feature is included in Microsoft Edge stable release 130.0.2849.80 and later.<br><br>**Note:** This feature is turned on again in Microsoft Edge version 133.0.3065.10 and higher. Customers are encouraged to test the impact of this feature and prepare for the change in behavior.|
| 124    |  Specific HTTPS websites are no longer accessible, with the error:<br>ERR_CONNECTION_ABORTED or ERR_SSL_PROTOCOL_ERROR.<br>This error might also occur when fetching resources on the page, causing display or delay issues.<br><br> The "TLS 1.3 hybridized Kyber support" feature causes this error.  | To verify if the issue is related the Kyber key encapsulation in TLS, you can disable the feature through its flag in `edge://flags/#enable-tls13-kyber`.<br><br>Enterprise administrators who need more time to update their certificates can set the **PostQuantumKeyAgreementEnabled** enterprise policy as a temporary workaround. Note:<br>- This fix is a temporary measure that will be removed in future versions of Microsoft Edge.<br>- Disabling this policy means that user traffic is unprotected from decryption by quantum computers.<br>The registry-key for the  policy is:<br>[HKEY_LOCAL_MACHINE\Software\Policies\Microsoft\Edge] <br>(DWORD) "PostQuantumKeyAgreementEnabled"=0 |     |
| 121    |  Specific HTTPS websites are no longer accessible, with the error:<br>ERR_SSL_KEY_USAGE_INCOMPATIBLE<br><br>This issue is caused by enforcing X.509 key usage extensions for RSA keys in TLS 1.2 and earlier versions.  |  Enterprise administrators who need more time to update their certificates can set the **RSAKeyUsageForLocalAnchorsEnabled enterprise** policy as a temporary workaround. This policy was temporarily available for administrators who needed more time to update their certificates to meet the new RSA key usage requirements. Note: This policy is removed in Microsoft Edge version 124 and later.<br>The registry-key for the policy is:<br>[HKEY_LOCAL_MACHINE\Software\Policies\Microsoft\Edge]<br>(DWORD)"RSAKeyUsageForLocalAnchorsEnabled"=0 |      |
| 120    |  When Microsoft Edge starts with an external HTTP-URL (for example,  `http://www.example.com`), Microsoft Edge opens the page directly with HTTPS, in case the server also enabled HTTPS. The same thing happens if you follow a hyperlink like this `http://www.example.com` in a new tab.<br><br>This change in behavior is due to the feature "HttpsDefault", which was enabled by default.   | With Microsoft Edge 120.0.2210.89, the policy **AutomaticHttpsDefault** can be used to disable the automatic switch from HTTP to HTTPS.<br>If you need to turn off the automatic switch from HTTP to HTTPS, deploy this policy:<br>"Configure Automatic HTTPS" -> "Automatic HTTPS functionality is disabled." (value 0)<br>The registry-key for the policy is:<br>[HKEY_LOCAL_MACHINE\Software\Policies\Microsoft\Edge]<br>(DWORD) "AutomaticHttpsDefault"=0<br><br>In a scenario where you only want to disable the automatic switch for specific websites, you can use the policy **InsecureContentAllowedForUrls** to configure these sites. |     |
| 119    |  Specific HTTPS websites are no longer accessible, with the error: ERR_SSL_PROTOCOL_ERROR.<br><br>This issue is caused by removing support for signature algorithms using SHA-1 for server signatures during the TLS handshake. | Enterprise administrators who need more time can set the **InsecureHashesInTLSHandshakesEnabled** enterprise policy as a temporary workaround. Note:<br>- This policy is temporary. It was removed in Microsoft Edge version 124 and later.<br>- Because this allows an insecure hash function in a critical part of the TLS handshake, enabling this policy increases the risk of attackers impersonating servers in an enterprise deployment.<br>The registry-key for the policy is:<br>[HKEY_LOCAL_MACHINE\Software\Policies\Microsoft\Edge]<br>(DWORD) "InsecureHashesInTLSHandshakesEnabled"=1 |  |

<!--------------------------------->
<!--------- TAB 2 FIXED ----------->
<!--------------------------------->

## [**Fixed issues**](#tab/Fixed)

|  Version  | Symptom | Workaround | Comment |
| --- | --- | --- | --- |
| 131 | Starting with Microsoft Edge Stable version 131.0.2903.48, some text is not displayed, and rendering is broken when viewing certain PDF files containing Japanese fonts. | This issue doesn't occur with the new Adobe Acrobat powered built-in PDF reader. Enterprise administrators can avoid the issue by enabling the [NewPDFReaderEnabled](/deployedge/microsoft-edge-policies#newpdfreaderenabled) policy. Each user can also avoid the issue by enabling the New PDF Viewer in *edge://flags/#edge-new-pdf-viewer*.<br><br>**Note:**<br>When you set NewPDFReaderEnabled to 1, the PDF is displayed correctly in Edge. However, the same issue occurs in the print preview. Some text does not display correctly in the print preview, but the actual printout is correct.  | This issue on Windows is fixed in Microsoft Edge stable release 131.0.2903.70.<br><br>This issue on macOS is fixed in Microsoft Edge stable release 132.0.2957.115. |
| 130 | Starting with Microsoft Edge Stable version 130.0.2849.46, some browser extensions are no longer working if they are using the chrome.storage.managed API. | Roll back Microsoft Edge to version 129.0.2792.89. | This issue is fixed in Microsoft Edge stable release 130.0.2849.56. |
| 128    | Starting with Microsoft Edge Stable version 128.0.2739.42, pages may fail to fully load when retrieving resources from the HTTP cache. When the issue is encountered, DevTools shows the requests failing with net::ERR_FAILED.| Roll back Microsoft Edge to version 127.0.2651.105 for Edge Stable or version 126.0.2592.137 for Edge Extended Stable.<br><br>A force reload (Ctrl+Reload button) can mitigate individual page loads.<br><br>Site owners may also consider reducing the use of HTTP caching for impacted resources until the issue is addressed. |Microsoft is collaborating with the Chromium project via [Chromium bug 362788339]( https://issues.chromium.org/issues/362788339) to address the issue. This issue is fixed in Microsoft Edge stable release 128.0.2739.63. |
| 128    | Starting with Microsoft Edge Stable version 128.0.2739.42, custom configured start pages appear to be stuck in the loading state. | Roll back Microsoft Edge to version 127.0.2651.105 for Edge Stable or version 126.0.2592.137 for Edge Extended Stable.<br><br>Use the command line argument: `"C:\Program Files (x86)\Microsoft\Edge\Application\msedge.exe" --disable-features="msIrm, msIrmv2, msEndpointDLp"`<br>**Note:** Command line args are case sensitive. | The fix is included in Stable version 128.0.2739.54.  |


## See also

- [Microsoft Edge Enterprise landing page](https://aka.ms/EdgeEnterprise)
