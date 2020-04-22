---
title: تعيين أذونات المجلد العمومي أو تغييرها
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cffdf9bf-34ce-40f6-a69e-d02f17d9caef
ms.openlocfilehash: cf891a4db05b8a2bdb223cc86693f5072faca494
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43681091"
---
# <a name="permissions-and-public-folders"></a><span data-ttu-id="2ed16-102">الأذونات والمجلدات العامة</span><span class="sxs-lookup"><span data-stu-id="2ed16-102">Permissions and Public Folders</span></span>

<span data-ttu-id="2ed16-103">يمكنك تغيير الأذونات على المجلدات العامة باستخدام Outlook أو مركز إدارة Exchange (EAC) أو PowerShell:</span><span class="sxs-lookup"><span data-stu-id="2ed16-103">You can change the permissions on your Public Folders using Outlook, the Exchange admin center (EAC), or PowerShell:</span></span>
  
- <span data-ttu-id="2ed16-104">للحصول على تعليمات Outlook، [انقر هنا](https://support.office.com/article/Set-or-change-permissions-for-a-public-folder-b2e0440c-7873-48ec-9ff2-b1a20b723005.aspx).</span><span class="sxs-lookup"><span data-stu-id="2ed16-104">For Outlook instructions, [click here](https://support.office.com/article/Set-or-change-permissions-for-a-public-folder-b2e0440c-7873-48ec-9ff2-b1a20b723005.aspx).</span></span>
    
- <span data-ttu-id="2ed16-105">بالنسبة لـ EAC، راجع [هذه المقالة](https://technet.microsoft.com/library/jj651147%28v=exchg.150%29.aspx.aspx#Anchor_1) للحصول على إرشادات.</span><span class="sxs-lookup"><span data-stu-id="2ed16-105">For EAC, refer to [this article](https://technet.microsoft.com/library/jj651147%28v=exchg.150%29.aspx.aspx#Anchor_1) for instructions.</span></span> 
    
- <span data-ttu-id="2ed16-106">لPowershell، راجع [هذه المقالة](https://technet.microsoft.com/library/bb124743%28v=exchg.160%29.aspx.aspx) للحصول على إرشادات حول استخدام الأمر إضافة-PublicFolderClientPermission.</span><span class="sxs-lookup"><span data-stu-id="2ed16-106">For Powershell, refer to [this article](https://technet.microsoft.com/library/bb124743%28v=exchg.160%29.aspx.aspx) for instructions on using the Add-PublicFolderClientPermission commandlet.</span></span> <span data-ttu-id="2ed16-107">إذا كنت بحاجة إلى تعليمات للاتصال Exchange Powershell، انقر [هنا](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx.aspx).</span><span class="sxs-lookup"><span data-stu-id="2ed16-107">If you need instructions to connect to Exchange Powershell, click [here](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx.aspx).</span></span>
    
<span data-ttu-id="2ed16-108">إذا **لم يتمكن المستخدمون الخارجيون من إرسال رسائل البريد الإلكتروني إلى مجلد عام ممكّن بالبريد،** فقد يكون السبب هو أن المجلد العام يفتقد الأذونات المطلوبة لتسليم البريد الإلكتروني الخارجي.</span><span class="sxs-lookup"><span data-stu-id="2ed16-108">If **external users can't send emails to a mail-enabled Public Folder**, the reason might be that the public folder is missing permissions required for external email delivery.</span></span> <span data-ttu-id="2ed16-109">يمكنك إصلاح هذا باستخدام تعليمات Outlook [هنا](https://technet.microsoft.com/library/aa997560%28v=exchg.150%29.aspx.aspx#Anchor_1)، أو تعليمات PowerShell [هنا](https://support.microsoft.com/help/2984402/-5.7.1-smtp-550-5.7.1-resolver.rst.authrequired-nondelivery-report-when-external-users-try-to-send-mail-to-mail-enabled-public-folders-in-office-365.aspx).</span><span class="sxs-lookup"><span data-stu-id="2ed16-109">You can fix this using the Outlook instructions [here](https://technet.microsoft.com/library/aa997560%28v=exchg.150%29.aspx.aspx#Anchor_1), or the PowerShell instructions [here](https://support.microsoft.com/help/2984402/-5.7.1-smtp-550-5.7.1-resolver.rst.authrequired-nondelivery-report-when-external-users-try-to-send-mail-to-mail-enabled-public-folders-in-office-365.aspx).</span></span>
  

