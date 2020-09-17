---
title: هل تحتاج إلى وضع علامة علي المجال أو مرسل البريد الكتروني بأمان ؟
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
- "9002921"
- "5673"
ms.openlocfilehash: 0ea089b95ad7de25e77017196fb2db895d4d0178
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47803232"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a><span data-ttu-id="1314b-102">هل تحتاج إلى وضع علامة علي المجال أو مرسل البريد الكتروني بأمان ؟</span><span class="sxs-lookup"><span data-stu-id="1314b-102">Need to mark a domain or email sender safe?</span></span>

- <span data-ttu-id="1314b-103">**لا يوصي باستخدام قوائم المرسلين الموثوق** بها لأنها تفتح المؤسسة الخاصة بك بالبريد العشوائي والفيش وهجمات الانتحال.</span><span class="sxs-lookup"><span data-stu-id="1314b-103">Use of **safe sender lists is not recommended** since it opens up your organization to spam, phish, and spoofing attacks.</span></span>
- <span data-ttu-id="1314b-104">ومع ذلك ، إذا كان هناك متطلب شركه ، **فنوصي** باستخدام **[قواعد تدفق البريد](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** لهذا الاجراء.</span><span class="sxs-lookup"><span data-stu-id="1314b-104">However, if there is a business requirement, we **recommend** using **[Mail Flow Rules](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** for this.</span></span> <span data-ttu-id="1314b-105">تضمن الإرشادات الخاصة بنا مصادقه المرسل (التحقق من ان المجال لم يتم الآن الانتحال).</span><span class="sxs-lookup"><span data-stu-id="1314b-105">Our guidance ensures sender authentication (verifies sending domain is not being spoofed).</span></span> <span data-ttu-id="1314b-106">**ملاحظه**: لا نوصي باداره بوسيتيفيس false باستخدام قوائم المرسلين الموثوق بهم ، لأنه بإمكان الاستثناءات لتصفيه البريد العشوائي فتح مؤسستك في هجمات الأمان.</span><span class="sxs-lookup"><span data-stu-id="1314b-106">**Note**: We don't recommend managing false positives by using safe sender lists, because exceptions to spam filtering can open your organization to security attacks.</span></span> <span data-ttu-id="1314b-107">إذا تلقي المستخدمون الرسائل التي تم وضع علامة عليها بشكل غير صحيح أو بريد الكتروني غير هام ، فالرجاء **[الإبلاغ عن الرسائل والملفات إلى Microsoft](https://protection.office.com/reportsubmission)**.</span><span class="sxs-lookup"><span data-stu-id="1314b-107">If your user(s) receive messages incorrectly marked as spam or junk email, please **[Report messages and files to Microsoft](https://protection.office.com/reportsubmission)**.</span></span>
- <span data-ttu-id="1314b-108">**يجب تجنب** المرسلين الموثوق بهم في Outlook أو قائمه المرسلين المسموح بهم أو قائمه المجالات المسموح بها في نهج الحماية من البريد العشوائي لان المرسلين يقومون بتجاوز كل البريد العشوائي والسبووف والحماية الفيشة ومصادقه المرسل (SPF و DKIM و DMARC).</span><span class="sxs-lookup"><span data-stu-id="1314b-108">Safe Senders in Outlook, Allowed sender list, or allowed domain list in anti-spam policies **should be avoided** because senders bypass all spam, spoof, and phish protection, and sender authentication (SPF, DKIM, DMARC).</span></span> <span data-ttu-id="1314b-109">يفضل استخدام هذه الطريقة للاختبار المؤقت فقط.</span><span class="sxs-lookup"><span data-stu-id="1314b-109">This method is best used for temporary testing only.</span></span>
