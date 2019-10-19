---
title: رمز الخطا 550 5.7.501 تم رفض الوصول ، الكشف عن أساءه استخدام البريد الكتروني العشوائي
ms.author: chrisda
author: chrisda
ms.date: 6/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "351"
- "3100015"
ms.assetid: 3105905c-e7a0-42a7-9c5a-61dc56a1d6fc
ms.openlocfilehash: 545cab07cc7c49def849be20bb6363da228a5393
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/18/2019
ms.locfileid: "36740128"
---
# <a name="550-57501-access-denied-spam-abuse-detected"></a><span data-ttu-id="2de75-102">550 5.7.501 الوصول مرفوض ، تم الكشف عن أساءه استخدام البريد المزعج</span><span class="sxs-lookup"><span data-stu-id="2de75-102">550 5.7.501 Access denied, spam abuse detected</span></span>

<span data-ttu-id="2de75-103">عاده ما تحدث هذه الرسالة عندما يقوم المستخدمون بإرسال رسائل البريد الكتروني من عناوين IP باستخدام المجال *onmicrosoft.com* الذي تم تعيينه إلى المستاجرين الجدد في Office 365.</span><span class="sxs-lookup"><span data-stu-id="2de75-103">Typically, this message occurs when users send email messages from IP addresses using the initial *.onmicrosoft.com* domain that's assigned to new tenants in Office 365.</span></span> <span data-ttu-id="2de75-104">أسهل طريقه لحل هذه المشكلة هي:</span><span class="sxs-lookup"><span data-stu-id="2de75-104">The easiest way to resolve this problem is to:</span></span>

1. <span data-ttu-id="2de75-105">[أضافه مجال إلى المستاجر الخاص بك](https://docs.microsoft.com//office365/admin/setup/add-domain).</span><span class="sxs-lookup"><span data-stu-id="2de75-105">[Add a domain to your tenant](https://docs.microsoft.com//office365/admin/setup/add-domain).</span></span>

2. <span data-ttu-id="2de75-106">[تغيير عنوان البريد الكتروني الأساسي للمستخدمين](https://docs.microsoft.com//office365/admin/add-users/change-a-user-name-and-email-address) إلى المجال المخصص الجديد الذي أضفته للتو.</span><span class="sxs-lookup"><span data-stu-id="2de75-106">[Change your users' primary email address](https://docs.microsoft.com//office365/admin/add-users/change-a-user-name-and-email-address) to the new custom domain you just added.</span></span>
