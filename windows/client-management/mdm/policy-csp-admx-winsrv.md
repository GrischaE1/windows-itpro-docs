---
title: Policy CSP - ADMX_Winsrv
description: Policy CSP - ADMX_Winsrv
ms.author: dansimp
ms.localizationpriority: medium
ms.topic: article
ms.prod: w10
ms.technology: windows
author: manikadhiman
ms.date: 02/25/2021
ms.reviewer: 
manager: dansimp
---

# Policy CSP - ADMX_Winsrv
>[!TIP]
> These are ADMX-backed policies and require a special SyncML format to enable or disable. For details, see [Understanding ADMX-backed policies](./understanding-admx-backed-policies.md).
> 
> You must specify the data type in the SyncML as &lt;Format&gt;chr&lt;/Format&gt;. For an example SyncML, refer to [Enabling a policy](./understanding-admx-backed-policies.md#enabling-a-policy).
> 
> The payload of the SyncML must be XML-encoded; for this XML encoding, there are a variety of online encoders that you can use. To avoid encoding the payload, you can use CDATA if your MDM supports it. For more information, see [CDATA Sections](http://www.w3.org/TR/REC-xml/#sec-cdata-sect).


<hr/>

<!--Policies-->
## ADMX_Winsrv policies  

<dl>
  <dd>
    <a href="#admx-winsrv-allowblockingappsatshutdown">ADMX_Winsrv/AllowBlockingAppsAtShutdown</a>
  </dd>
</dl>


<hr/>

<!--Policy-->
<a href="" id="admx-winsrv-allowblockingappsatshutdown"></a>**ADMX_Winsrv/AllowBlockingAppsAtShutdown**  

<!--SupportedSKUs-->
<table>
<tr>
    <th>Edition</th>
    <th>Windows 10</th>
    <th>Windows 11</th> 
</tr>
<tr>
    <td>Home</td>
    <td>No</td>
    <td>No</td>
</tr>
<tr>
    <td>Pro</td>
    <td>No</td>
    <td>No</td>
</tr>
<tr>
    <td>Business</td>
    <td>No</td>
    <td>No</td>
</tr>
<tr>
    <td>Enterprise</td>
    <td>Yes</td>
    <td>Yes</td>
</tr>
<tr>
    <td>Education</td>
    <td>Yes</td>
    <td>Yes</td>
</tr>
</table>


<!--/SupportedSKUs-->
<hr/>

<!--Scope-->
[Scope](./policy-configuration-service-provider.md#policy-scope):

> [!div class = "checklist"]
> * Device

<hr/>

<!--/Scope-->
<!--Description-->
This policy setting specifies whether Windows will allow console applications and GUI applications without visible top-level windows to block or cancel shutdown.

By default, such applications are automatically terminated if they attempt to cancel shutdown or block it indefinitely.

- If you enable this setting, console applications or GUI applications without visible top-level windows that block or cancel shutdown will not be automatically terminated during shutdown.
- If you disable or do not configure this setting, these applications will be automatically terminated during shutdown, helping to ensure that windows can shut down faster and more smoothly.

> [!NOTE]
> This policy setting applies to all sites in Trusted zones.

<!--/Description-->


<!--ADMXBacked-->
ADMX Info:  
-   GP Friendly name: *Turn off automatic termination of applications that block or cancel shutdown*
-   GP name: *AllowBlockingAppsAtShutdown*
-   GP path: *System\Shutdown Options*
-   GP ADMX file name: *Winsrv.admx*

<!--/ADMXBacked-->
<!--/Policy-->
<hr/>



<!--/Policies-->

