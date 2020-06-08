---
title: حل مشكلات مصادقة SMTP
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "5652"
ms.openlocfilehash: 814c49e8e65966a0c9f927b1f7bfb03d3dc3d637
ms.sourcegitcommit: 0e43e19448705f151846e9e9e1e0f47e12938fdf
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/15/2020
ms.locfileid: "44264303"
---
# <a name="solving-smtp-authentication-issues"></a><span data-ttu-id="4894b-102">حل مشكلات مصادقة SMTP</span><span class="sxs-lookup"><span data-stu-id="4894b-102">Solving SMTP authentication issues</span></span>

<span data-ttu-id="4894b-103">إذا كنت تحصل على أخطاء 5.7.57 أو 5.7.3 عند محاولة إرسال البريد الإلكتروني SMTP والمصادقة مع عميل أو تطبيق، هناك عدد قليل من الأشياء التي يجب التحقق منها:</span><span class="sxs-lookup"><span data-stu-id="4894b-103">If you are getting errors 5.7.57 or 5.7.3 when trying to send SMTP email and authenticate with a client or application, there are a few things you should check:</span></span>

- <span data-ttu-id="4894b-104">قد يتم تعطيل إرسال SMTP المصادق عليه في المستأجر، أو على صندوق البريد الذي تحاول استخدامه (تحقق من كلا الإعدادين).</span><span class="sxs-lookup"><span data-stu-id="4894b-104">Authenticated SMTP submission might be disabled in your tenant, or on the mailbox that you are trying to use (check both settings).</span></span> <span data-ttu-id="4894b-105">لقراءة المزيد، راجع [تمكين أو تعطيل إرسال SMTP العميل المصادق عليه](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission).</span><span class="sxs-lookup"><span data-stu-id="4894b-105">To read more, see [Enable or disable authenticated client SMTP submission](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission).</span></span>

- <span data-ttu-id="4894b-106">تحقق مما إذا كانت [إعدادات أمان Azure](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) ممكّنة للمستأجر؛ إذا تم تمكينمصادقة SMTP باستخدام المصادقة الأساسية (المعروفة أيضًا باسم Legacy؛ وهذا سيستخدم اسم المستخدم وكلمة المرور) ستفشل.</span><span class="sxs-lookup"><span data-stu-id="4894b-106">Check whether [Azure Security Defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) are enabled for your tenant; if enabled, SMTP authentication using basic authentication (also known as legacy; this will use username and password) will fail.</span></span>
