---
title: بلوكليجاسياوث
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3154"
- "9001194"
ms.openlocfilehash: baf3ee808cce1e4da362dd0841c0138d7d9268d1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47685585"
---
# <a name="blocking-legacy-authentication"></a><span data-ttu-id="d91f0-102">حظر المصادقة القديمة</span><span class="sxs-lookup"><span data-stu-id="d91f0-102">Blocking legacy authentication</span></span>

<span data-ttu-id="d91f0-103">المصادقة القديمة هي مصطلح يشير إلى طلب مصادقه تم إنشاؤه بواسطة:</span><span class="sxs-lookup"><span data-stu-id="d91f0-103">Legacy authentication is a term that refers to an authentication request made by:</span></span>

- <span data-ttu-id="d91f0-104">عملاء Office الأقدم الذين لا يستخدمون المصادقة الحديثة (علي سبيل المثال ، Office 2010 client).</span><span class="sxs-lookup"><span data-stu-id="d91f0-104">Older Office clients that do not use modern authentication (for example, Office 2010 client).</span></span>

- <span data-ttu-id="d91f0-105">اي عميل يستخدم بروتوكولات البريد القديمة مثل IMAP/SMTP/POP3.</span><span class="sxs-lookup"><span data-stu-id="d91f0-105">Any client that uses legacy mail protocols such as IMAP/SMTP/POP3.</span></span>

<span data-ttu-id="d91f0-106">للحصول علي مزيد من المعلومات حول حظر المصادقة القديمة وتمكين المصادقة الحديثة ، راجع [حظر المصادقة القديمة](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span><span class="sxs-lookup"><span data-stu-id="d91f0-106">For more information on blocking legacy authentication and enabling modern authentication, refer to [Blocking legacy authentication](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span></span>

<span data-ttu-id="d91f0-107">تسهل إعدادات الأمان الافتراضية في Azure Active directory (Azure AD) أمانا والمساعدة في حماية مؤسستك.</span><span class="sxs-lookup"><span data-stu-id="d91f0-107">Security defaults in Azure Active Directory (Azure AD) make it easier to be secure and help protect your organization.</span></span> <span data-ttu-id="d91f0-108">تحتوي الافتراضيات الامنه علي إعدادات أمان مكونه مسبقا للهجمات الشائعة.</span><span class="sxs-lookup"><span data-stu-id="d91f0-108">Security defaults contain preconfigured security settings for common attacks.</span></span>
<span data-ttu-id="d91f0-109">لمزيد من المعلومات حول الإعدادات الافتراضية للامان ، يمكنك الرجوع إلى [ما هو افتراضيات الأمان ؟](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span><span class="sxs-lookup"><span data-stu-id="d91f0-109">For more information about security defaults, refer to [What are security defaults?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span></span> 

<span data-ttu-id="d91f0-110">**ملاحظه**: إذا تم إنشاء المستاجر الخاص بك في أو بعد أكتوبر 22nd 2019 ، فمن المحتمل انك تواجه السلوك الافتراضي الجديد الأمن والذي تم تمكينه بالفعل في المستاجر الخاص بك.</span><span class="sxs-lookup"><span data-stu-id="d91f0-110">**Note**:  If your tenant was created on or after October 22nd, 2019, it's possible you are experiencing the new secure-by-default behavior and already have security defaults enabled in your tenant.</span></span>  <span data-ttu-id="d91f0-111">في اي جهد لحماية كل المستخدمين ، يتم الآن سحب الإعدادات الافتراضية للامان لكل المستاجرين الجدد التي تم إنشاؤها.</span><span class="sxs-lookup"><span data-stu-id="d91f0-111">In an effort to protect all of our users, security defaults is being rolled out to all new tenants created.</span></span>
