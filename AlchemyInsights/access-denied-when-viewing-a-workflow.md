---
title: تم رفض الوصول عند عرض سير عمل
ms.author: pebaum
author: Techwriter40
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 4ca65583fbd98867026e9e3cc8f36fe38798aa85
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/25/2019
ms.locfileid: "36747735"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="30f7f-102">تم رفض الوصول عند عرض سير عمل</span><span class="sxs-lookup"><span data-stu-id="30f7f-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="30f7f-103">يمكن ان تفشل مهام سير العمل 2013 SharePoint التي تحاول إرسال بريد الكتروني إلى مجموعه SharePoint مع رسالة خطا "تم رفض الوصول" إذا لم يتم تعيين عضويه مجموعه SharePoint إلى Everyone.</span><span class="sxs-lookup"><span data-stu-id="30f7f-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="30f7f-104">**لحل هذه المشكلة ، قم بالخطوات التالية:**</span><span class="sxs-lookup"><span data-stu-id="30f7f-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="30f7f-105">السماح للجميع بمشاهده أعضاء مجموعه SharePoint.</span><span class="sxs-lookup"><span data-stu-id="30f7f-105">Allow everybody to see the members of the SharePoint group.</span></span>
  
 2. <span data-ttu-id="30f7f-106">أزاله مجموعه SharePoint من سطر إلى أو نسخه من البريد الكتروني.</span><span class="sxs-lookup"><span data-stu-id="30f7f-106">Remove the SharePoint group from the To or CC line of the email.</span></span>
  
 3. <span data-ttu-id="30f7f-107">قم باضافه المستخدمين بشكل صريح إلى السطر "إلى" أو "نسخه" إذا تعذر تغيير رؤية العضوية لمجموعه SharePoint.</span><span class="sxs-lookup"><span data-stu-id="30f7f-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span>
  
<span data-ttu-id="30f7f-108">لعرض مزيد من التفاصيل يرجى الرجوع إلى [HTTP غير مصرح به إلى/_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="30f7f-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  