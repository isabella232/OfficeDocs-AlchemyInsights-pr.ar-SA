---
title: حل مشاكل مصادقه SMTP
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "5652"
ms.openlocfilehash: 3eaab2c601f78e20f2ee67bc21a9598cb45a24f9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47737976"
---
# <a name="solving-smtp-authentication-issues"></a><span data-ttu-id="948cf-102">حل مشاكل مصادقه SMTP</span><span class="sxs-lookup"><span data-stu-id="948cf-102">Solving SMTP authentication issues</span></span>

<span data-ttu-id="948cf-103">إذا كنت تتلقي أخطاء 5.7.57 أو 5.7.3 عند محاولة إرسال بريد SMTP الكتروني والمصادقة مع عميل أو تطبيق ، فهناك بعض الأمور التي يجب التحقق منها:</span><span class="sxs-lookup"><span data-stu-id="948cf-103">If you are getting errors 5.7.57 or 5.7.3 when trying to send SMTP email and authenticate with a client or application, there are a few things you should check:</span></span>

- <span data-ttu-id="948cf-104">قد يتم تعطيل إرسال SMTP المصادق عليه في نطاق المستاجر أو علي علبه البريد التي تحاول استخدامها (تحقق من الإعدادين).</span><span class="sxs-lookup"><span data-stu-id="948cf-104">Authenticated SMTP submission might be disabled in your tenant, or on the mailbox that you are trying to use (check both settings).</span></span> <span data-ttu-id="948cf-105">لقراءه المزيد ، راجع [تمكين إرسال SMTP للعميل المصدق أو تعطيله](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission).</span><span class="sxs-lookup"><span data-stu-id="948cf-105">To read more, see [Enable or disable authenticated client SMTP submission](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission).</span></span>

- <span data-ttu-id="948cf-106">تحقق مما إذا كانت [الإعدادات الافتراضية لامان Azure](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) ممكنة للمستاجر لديك ؛ إذا كان ممكنا ، فان مصادقه SMTP باستخدام المصادقة الاساسيه (المعروفة أيضا بالقديمة ؛ سيؤدي ذلك إلى استخدام اسم المستخدم وكلمه المرور).</span><span class="sxs-lookup"><span data-stu-id="948cf-106">Check whether [Azure Security Defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) are enabled for your tenant; if enabled, SMTP authentication using basic authentication (also known as legacy; this will use username and password) will fail.</span></span>
