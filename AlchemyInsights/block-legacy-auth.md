---
title: BlockLegacyAuth
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3154"
- "9001194"
ms.openlocfilehash: 06ded694893c020f862864215700853b19d35f08
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820165"
---
# <a name="blocking-legacy-authentication"></a><span data-ttu-id="aa0c8-102">حظر المصادقة القديمة</span><span class="sxs-lookup"><span data-stu-id="aa0c8-102">Blocking legacy authentication</span></span>

<span data-ttu-id="aa0c8-103">المصادقة القديمة عبارة عن مصطلح يشير إلى طلب مصادقة تم تقديمه من خلال:</span><span class="sxs-lookup"><span data-stu-id="aa0c8-103">Legacy authentication is a term that refers to an authentication request made by:</span></span>

- <span data-ttu-id="aa0c8-104">عملاء Office الأقدم الذين لا يستخدمون المصادقة الحديثة (على سبيل المثال، عميل Office 2010).</span><span class="sxs-lookup"><span data-stu-id="aa0c8-104">Older Office clients that do not use modern authentication (for example, Office 2010 client).</span></span>

- <span data-ttu-id="aa0c8-105">أي عميل يستخدم بروتوكولات البريد القديمة مثل IMAP/SMTP/POP3.</span><span class="sxs-lookup"><span data-stu-id="aa0c8-105">Any client that uses legacy mail protocols such as IMAP/SMTP/POP3.</span></span>

<span data-ttu-id="aa0c8-106">لمزيد من المعلومات حول حظر المصادقة القديمة وتمكين المصادقة الحديثة، راجع [حظر المصادقة القديمة](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span><span class="sxs-lookup"><span data-stu-id="aa0c8-106">For more information on blocking legacy authentication and enabling modern authentication, refer to [Blocking legacy authentication](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span></span>

<span data-ttu-id="aa0c8-107">تجعل إعدادات الأمان الافتراضية في Azure Active Directory (Azure AD) من السهل أن تكون آمنا وتساعد على حماية مؤسستك.</span><span class="sxs-lookup"><span data-stu-id="aa0c8-107">Security defaults in Azure Active Directory (Azure AD) make it easier to be secure and help protect your organization.</span></span> <span data-ttu-id="aa0c8-108">تحتوي إعدادات الأمان الافتراضية على إعدادات أمان تم تكوينها مسبقا للهجمات الشائعة.</span><span class="sxs-lookup"><span data-stu-id="aa0c8-108">Security defaults contain preconfigured security settings for common attacks.</span></span>
<span data-ttu-id="aa0c8-109">لمزيد من المعلومات حول إعدادات الأمان الافتراضية، راجع [ما هي إعدادات الأمان الافتراضية؟](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span><span class="sxs-lookup"><span data-stu-id="aa0c8-109">For more information about security defaults, refer to [What are security defaults?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span></span> 

<span data-ttu-id="aa0c8-110">**ملاحظة:** إذا تم إنشاء المستأجر في 22 أكتوبر 2019 أو بعده، فمن المحتمل أنك تواجه سلوك الأمان الافتراضي الجديد وقد تم تمكين إعدادات الأمان الافتراضية بالفعل في المستأجر.</span><span class="sxs-lookup"><span data-stu-id="aa0c8-110">**Note**:  If your tenant was created on or after October 22nd, 2019, it's possible you are experiencing the new secure-by-default behavior and already have security defaults enabled in your tenant.</span></span>  <span data-ttu-id="aa0c8-111">في محاولة لحماية جميع المستخدمين، يتم طرح إعدادات الأمان الافتراضية لجميع المستأجرين الجدد الذين تم إنشاؤهم.</span><span class="sxs-lookup"><span data-stu-id="aa0c8-111">In an effort to protect all of our users, security defaults is being rolled out to all new tenants created.</span></span>
