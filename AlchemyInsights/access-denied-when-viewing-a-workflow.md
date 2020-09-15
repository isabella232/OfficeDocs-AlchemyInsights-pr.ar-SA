---
title: رفض الوصول عند عرض سير عمل
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 710775e8b2dee98969df7a4c8410a3e61181aaf6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47688789"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="e281a-102">رفض الوصول عند عرض سير عمل</span><span class="sxs-lookup"><span data-stu-id="e281a-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="e281a-103">يمكن ان تفشل مهام سير عمل SharePoint 2013 التي تحاول إرسال رسالة بريد الكتروني إلى مجموعه SharePoint مع ظهور رسالة الخطا "رفض الوصول" إذا لم يتم تعيين عضويه مجموعه SharePoint إلى الجميع.</span><span class="sxs-lookup"><span data-stu-id="e281a-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="e281a-104">**لحل هذه المشكلة ، قم بتنفيذ الخطوات التالية:**</span><span class="sxs-lookup"><span data-stu-id="e281a-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="e281a-105">اسمح لجميع برؤية أعضاء مجموعه SharePoint.</span><span class="sxs-lookup"><span data-stu-id="e281a-105">Allow everybody to see the members of the SharePoint group.</span></span>
  
 2. <span data-ttu-id="e281a-106">أزاله مجموعه SharePoint من السطر "إلى" أو "نسخه" في البريد الكتروني.</span><span class="sxs-lookup"><span data-stu-id="e281a-106">Remove the SharePoint group from the To or CC line of the email.</span></span>
  
 3. <span data-ttu-id="e281a-107">أضف المستخدمين بشكل صريح إلى السطر إلى أو نسخه إذا تعذر تغيير امكانيه رؤية العضوية لمجموعه SharePoint.</span><span class="sxs-lookup"><span data-stu-id="e281a-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span>
  
<span data-ttu-id="e281a-108">لعرض المزيد من التفاصيل يرجى الاشاره إلى [HTTP غير مرخص ل/_vti_bin/client.svc/sp.utilities.utility.sendemail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="e281a-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  