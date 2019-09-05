---
title: تم رفض استخدام رمز الخطأ 550 5.7.501، تم الكشف عن إساءة استخدام الرسائل غير المرغوب فيها
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
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/04/2019
ms.locfileid: "36740128"
---
# <a name="550-57501-access-denied-spam-abuse-detected"></a><span data-ttu-id="2b67f-102">550 5.7.501 تم رفض الوصول، تم الكشف عن إساءة استخدام الرسائل غير المرغوب فيها</span><span class="sxs-lookup"><span data-stu-id="2b67f-102">550 5.7.501 Access denied, spam abuse detected</span></span>

<span data-ttu-id="2b67f-103">بشكل عام، تحدث هذه الرسالة عند إرسال المستخدمين رسائل البريد الإلكتروني من عناوين IP باستخدام مجال *.onmicrosoft.com* الأولي الذي تم تعيينه إلى المستأجرين الجدد في Office 365.</span><span class="sxs-lookup"><span data-stu-id="2b67f-103">Typically, this message occurs when users send email messages from IP addresses using the initial *.onmicrosoft.com* domain that's assigned to new tenants in Office 365.</span></span> <span data-ttu-id="2b67f-104">أسهل طريقة لحل هذه المشكلة هي:</span><span class="sxs-lookup"><span data-stu-id="2b67f-104">The easiest way to resolve this problem is to:</span></span>

1. <span data-ttu-id="2b67f-105">[إضافة مجال إلى المستأجر الخاص بك](https://docs.microsoft.com//office365/admin/setup/add-domain).</span><span class="sxs-lookup"><span data-stu-id="2b67f-105">[Add a domain to your tenant](https://docs.microsoft.com//office365/admin/setup/add-domain).</span></span>

2. <span data-ttu-id="2b67f-106">[قم بتغيير عنوان البريد الإلكتروني الأساسي للمستخدمين](https://docs.microsoft.com//office365/admin/add-users/change-a-user-name-and-email-address) إلى المجال المخصص الجديد الذي قمت بإضافته للتو.</span><span class="sxs-lookup"><span data-stu-id="2b67f-106">[Change your users' primary email address](https://docs.microsoft.com//office365/admin/add-users/change-a-user-name-and-email-address) to the new custom domain you just added.</span></span>
