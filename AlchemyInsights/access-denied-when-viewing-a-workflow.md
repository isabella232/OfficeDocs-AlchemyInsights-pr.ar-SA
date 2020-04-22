---
title: تم رفض الوصول عند عرض سير عمل
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: c576bf88225582f2577e0b59506a7482cf9f38d5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43687317"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="0ba7a-102">تم رفض الوصول عند عرض سير عمل</span><span class="sxs-lookup"><span data-stu-id="0ba7a-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="0ba7a-103">يمكن أن تفشل سير عمل SharePoint 2013 التي تحاول إرسال بريد إلكتروني إلى مجموعة SharePoint مع رسالة خطأ "رفض الوصول" إذا لم يتم تعيين عضوية مجموعة SharePoint إلى الجميع.</span><span class="sxs-lookup"><span data-stu-id="0ba7a-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="0ba7a-104">**لحل هذه المشكلة، قم بالخطوات التالية:**</span><span class="sxs-lookup"><span data-stu-id="0ba7a-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="0ba7a-105">السماح للجميع برؤية أعضاء مجموعة SharePoint.</span><span class="sxs-lookup"><span data-stu-id="0ba7a-105">Allow everybody to see the members of the SharePoint group.</span></span>
  
 2. <span data-ttu-id="0ba7a-106">قم بإزالة مجموعة SharePoint من سطر To أو CC من البريد الإلكتروني.</span><span class="sxs-lookup"><span data-stu-id="0ba7a-106">Remove the SharePoint group from the To or CC line of the email.</span></span>
  
 3. <span data-ttu-id="0ba7a-107">إضافة المستخدمين بشكل صريح إلى سطر إلى أو نسخة إذا تعذر تغيير رؤية العضوية لمجموعة SharePoint.</span><span class="sxs-lookup"><span data-stu-id="0ba7a-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span>
  
<span data-ttu-id="0ba7a-108">للاطلاع على مزيد من التفاصيل يرجى الرجوع إلى [HTTP غير مصرح به إلى / _vti_bin/client.svc/sp.utility.utility.SendEmail.](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409)</span><span class="sxs-lookup"><span data-stu-id="0ba7a-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  