---
title: تم رفض الوصول عند عرض سير العمل
ms.author: kirks
author: Techwriter40
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 43369c600687d6ac253f70a8535dc2bd0d41687e
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/12/2019
ms.locfileid: "29918808"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="b101f-102">تم رفض الوصول عند عرض سير العمل</span><span class="sxs-lookup"><span data-stu-id="b101f-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="b101f-103">قد يفشل SharePoint 2013 مهام سير العمل التي تحاول إرسال بريد إلكتروني لمجموعة SharePoint مع رسالة خطأ "تم رفض الوصول" إذا لم يتم تعيين عضوية مجموعة SharePoint للجميع.</span><span class="sxs-lookup"><span data-stu-id="b101f-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="b101f-104">**لحل هذه المشكلة، قم بالخطوات التالية:**</span><span class="sxs-lookup"><span data-stu-id="b101f-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="b101f-105">السماح للجميع لرؤية أعضاء مجموعة SharePoint.</span><span class="sxs-lookup"><span data-stu-id="b101f-105">Allow everybody to see the members of the SharePoint group.</span></span> 
  
 2. <span data-ttu-id="b101f-106">إزالة مجموعة SharePoint من "إلى" أو "نسخة" سطر رسالة البريد الإلكتروني.</span><span class="sxs-lookup"><span data-stu-id="b101f-106">Remove the SharePoint group from the To or CC line of the email.</span></span> 
  
 3. <span data-ttu-id="b101f-107">إضافة المستخدمين بشكل صريح إلى المربع إلى أو نسخة خطية إذا لا يمكن تغيير رؤية العضوية لمجموعة SharePoint.</span><span class="sxs-lookup"><span data-stu-id="b101f-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span> 
  
<span data-ttu-id="b101f-108">لعرض مزيد من التفاصيل يرجى الرجوع إلى [HTTP غير المخول ل/_vti_bin/client.svc/sp.utilities.utility.SendEmail ](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="b101f-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail ](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  

