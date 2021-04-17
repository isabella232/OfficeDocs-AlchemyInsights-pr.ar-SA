---
title: حل مشاكل مصادقة SMTP
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "5652"
ms.openlocfilehash: 2d3f0f6b700c3e4485c9064fbaa4bcc165e92e17
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826402"
---
# <a name="solving-smtp-authentication-issues"></a><span data-ttu-id="4c53c-102">حل مشاكل مصادقة SMTP</span><span class="sxs-lookup"><span data-stu-id="4c53c-102">Solving SMTP authentication issues</span></span>

<span data-ttu-id="4c53c-103">إذا كنت تحصل على أخطاء 5.7.57 أو 5.7.3 عند محاولة إرسال بريد SMTP الإلكتروني والمصادقة مع عميل أو تطبيق، فهناك بعض الأمور التي يجب التحقق من صحتها:</span><span class="sxs-lookup"><span data-stu-id="4c53c-103">If you are getting errors 5.7.57 or 5.7.3 when trying to send SMTP email and authenticate with a client or application, there are a few things you should check:</span></span>

- <span data-ttu-id="4c53c-104">قد يتم تعطيل إرسال SMTP المصادق عليه في المستأجر أو في علبة البريد التي تحاول استخدامها (تحقق من الإعدادين).</span><span class="sxs-lookup"><span data-stu-id="4c53c-104">Authenticated SMTP submission might be disabled in your tenant, or on the mailbox that you are trying to use (check both settings).</span></span> <span data-ttu-id="4c53c-105">لقراءة المزيد، راجع [تمكين إرسال SMTP](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission)للعميل المصادق عليه أو تعطيله .</span><span class="sxs-lookup"><span data-stu-id="4c53c-105">To read more, see [Enable or disable authenticated client SMTP submission](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission).</span></span>

- <span data-ttu-id="4c53c-106">تحقق مما إذا [كانت إعدادات أمان Azure الافتراضية](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) تم تمكينها للمستأجر الخاص بك؛ إذا تم تمكينها، ستفشل مصادقة SMTP باستخدام المصادقة الأساسية (المعروفة أيضا باسم القديمة؛ حيث سيستخدم هذا اسم المستخدم وكلمة المرور).</span><span class="sxs-lookup"><span data-stu-id="4c53c-106">Check whether [Azure Security Defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) are enabled for your tenant; if enabled, SMTP authentication using basic authentication (also known as legacy; this will use username and password) will fail.</span></span>
