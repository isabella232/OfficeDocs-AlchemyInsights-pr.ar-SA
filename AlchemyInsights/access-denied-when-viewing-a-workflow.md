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
ms.openlocfilehash: 53bd9285e49e220f880eea21923f261302003127
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/22/2019
ms.locfileid: "36495810"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="58ffd-102">تم رفض الوصول عند عرض سير العمل</span><span class="sxs-lookup"><span data-stu-id="58ffd-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="58ffd-103">قد يفشل SharePoint 2013 مهام سير العمل التي تحاول إرسال بريد إلكتروني لمجموعة SharePoint مع رسالة خطأ "تم رفض الوصول" إذا لم يتم تعيين عضوية مجموعة SharePoint للجميع.</span><span class="sxs-lookup"><span data-stu-id="58ffd-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="58ffd-104">**لحل هذه المشكلة، قم بالخطوات التالية:**</span><span class="sxs-lookup"><span data-stu-id="58ffd-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="58ffd-105">السماح للجميع لرؤية أعضاء مجموعة SharePoint.</span><span class="sxs-lookup"><span data-stu-id="58ffd-105">Allow everybody to see the members of the SharePoint group.</span></span>
  
 2. <span data-ttu-id="58ffd-106">إزالة مجموعة SharePoint من "إلى" أو "نسخة" سطر رسالة البريد الإلكتروني.</span><span class="sxs-lookup"><span data-stu-id="58ffd-106">Remove the SharePoint group from the To or CC line of the email.</span></span>
  
 3. <span data-ttu-id="58ffd-107">إضافة المستخدمين بشكل صريح إلى المربع إلى أو نسخة خطية إذا لا يمكن تغيير رؤية العضوية لمجموعة SharePoint.</span><span class="sxs-lookup"><span data-stu-id="58ffd-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span>
  
<span data-ttu-id="58ffd-108">لعرض مزيد من التفاصيل يرجى الرجوع إلى [HTTP غير المخول ل/_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="58ffd-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  