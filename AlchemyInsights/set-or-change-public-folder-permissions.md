---
title: تعيين أو تغيير الأذونات على المجلد العمومي
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 8/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: cffdf9bf-34ce-40f6-a69e-d02f17d9caef
ms.openlocfilehash: 8e6a51bcc47eac7e76f55700091ecd86bc1634d7
ms.sourcegitcommit: 5dee2fcb492bd922092a6de8045a95febe57b97e
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/06/2019
ms.locfileid: "29759807"
---
# <a name="permissions-and-public-folders"></a><span data-ttu-id="4fa9d-102">الأذونات والمجلدات العمومية</span><span class="sxs-lookup"><span data-stu-id="4fa9d-102">Permissions and Public Folders</span></span>

<span data-ttu-id="4fa9d-103">يمكنك تغيير الأذونات على "المجلدات العمومية" باستخدام Outlook، مركز مسؤولي Exchange (شرق)، أو PowerShell:</span><span class="sxs-lookup"><span data-stu-id="4fa9d-103">You can change the permissions on your Public Folders using Outlook, the Exchange admin center (EAC), or PowerShell:</span></span>
  
- <span data-ttu-id="4fa9d-104">للحصول على تعليمات Outlook، [انقر هنا](https://support.office.com/article/Set-or-change-permissions-for-a-public-folder-b2e0440c-7873-48ec-9ff2-b1a20b723005.aspx).</span><span class="sxs-lookup"><span data-stu-id="4fa9d-104">For Outlook instructions, [click here](https://support.office.com/article/Set-or-change-permissions-for-a-public-folder-b2e0440c-7873-48ec-9ff2-b1a20b723005.aspx).</span></span>
    
- <span data-ttu-id="4fa9d-p101">لمجموعة شرق أفريقيا، أرجع إلى [هذه المقالة](https://technet.microsoft.com/library/jj651147%28v=exchg.150%29.aspx.aspx#Anchor_1) للحصول على إرشادات. يمكنك النقر [هنا](https://support.office.com/article/ https://outlook.office365.com/ecp/.aspx) للانتقال إلى مجموعة شرق أفريقيا.</span><span class="sxs-lookup"><span data-stu-id="4fa9d-p101">For EAC, refer to [this article](https://technet.microsoft.com/library/jj651147%28v=exchg.150%29.aspx.aspx#Anchor_1) for instructions. You can click [here](https://support.office.com/article/ https://outlook.office365.com/ecp/.aspx) to navigate to EAC.</span></span> 
    
- <span data-ttu-id="4fa9d-p102">ل Powershell، أرجع إلى [هذه المقالة](https://technet.microsoft.com/library/bb124743%28v=exchg.160%29.aspx.aspx) للحصول على إرشادات حول استخدام commandlet بوبليكفولديركلينتبيرميشن إضافة. إذا كنت تحتاج إرشادات للاتصال Exchange Powershell، انقر [هنا](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx.aspx).</span><span class="sxs-lookup"><span data-stu-id="4fa9d-p102">For Powershell, refer to [this article](https://technet.microsoft.com/library/bb124743%28v=exchg.160%29.aspx.aspx) for instructions on using the Add-PublicFolderClientPermission commandlet. If you need instructions to connect to Exchange Powershell, click [here](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx.aspx).</span></span>
    
<span data-ttu-id="4fa9d-p103">إذا كان **المستخدمون الخارجيون لا يمكن إرسال رسائل البريد الإلكتروني إلى "مجلد عمومي" تمكينها لاستخدام البريد**، السبب قد المجلد العمومي مفقود أذونات تلزم لتسليم البريد الإلكتروني الخارجي. يمكنك تصحيح ذلك باستخدام تعليمات Outlook [هنا](https://technet.microsoft.com/library/aa997560%28v=exchg.150%29.aspx.aspx#Anchor_1)أو إرشادات PowerShell [هنا](https://support.microsoft.com/help/2984402/-5.7.1-smtp-550-5.7.1-resolver.rst.authrequired-nondelivery-report-when-external-users-try-to-send-mail-to-mail-enabled-public-folders-in-office-365.aspx).</span><span class="sxs-lookup"><span data-stu-id="4fa9d-p103">If **external users can't send emails to a mail-enabled Public Folder**, the reason might be that the public folder is missing permissions required for external email delivery. You can fix this using the Outlook instructions [here](https://technet.microsoft.com/library/aa997560%28v=exchg.150%29.aspx.aspx#Anchor_1), or the PowerShell instructions [here](https://support.microsoft.com/help/2984402/-5.7.1-smtp-550-5.7.1-resolver.rst.authrequired-nondelivery-report-when-external-users-try-to-send-mail-to-mail-enabled-public-folders-in-office-365.aspx).</span></span>
  

