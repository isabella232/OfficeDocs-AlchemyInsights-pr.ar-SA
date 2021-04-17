---
title: AntiSpam 5.4.1 DBEB catch-all
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
- "9001209"
- "3167"
ms.openlocfilehash: c6ce26a133428dc7351912d8250ef096dfc7521a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821434"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a><span data-ttu-id="ecc9b-102">إصلاح مشاكل التسليم لرمز الخطأ 550 5.4.1 رفض الوصول إلى الترحيل</span><span class="sxs-lookup"><span data-stu-id="ecc9b-102">Fix delivery issues for error code 550 5.4.1 Relay Access Denied</span></span>

<span data-ttu-id="ecc9b-103">تحدث هذه المشكلة عند التحقق لمعرفة ما إذا كان عنوان البريد الإلكتروني [صالحا](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) لمنع حدوث ارتداد عند الدخول إلى شبكة Microsoft.</span><span class="sxs-lookup"><span data-stu-id="ecc9b-103">This problem occurs when [checking to see if an email address is valid to prevent bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) when entering the Microsoft network.</span></span> <span data-ttu-id="ecc9b-104">جرب ما يلي:</span><span class="sxs-lookup"><span data-stu-id="ecc9b-104">Try the following:</span></span>

1. <span data-ttu-id="ecc9b-105">تحديد ما إذا كانت المشكلة خاصة لمجال بأكمله أو عنوان بريد إلكتروني واحد:</span><span class="sxs-lookup"><span data-stu-id="ecc9b-105">Determine whether the problem is specific to an entire domain or a single email address:</span></span>
    - <span data-ttu-id="ecc9b-106">المجال بأكمله: يحتاج المجال في بعض الأحيان إلى مزامنة؛ حاول [تعيين المجال إلى داخلي ثم العودة إلى موثوق](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span><span class="sxs-lookup"><span data-stu-id="ecc9b-106">Entire domain: Sometimes the domain needs to be synchronized; try [setting the domain to Internal and then back to Authoritative](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span></span>
    - <span data-ttu-id="ecc9b-107">عنوان بريد إلكتروني واحد: في بعض الأحيان يجب مزامنة العنوان؛ قد يساعدك تغيير عنوان وكيل smtp ثم تغييره مرة أخرى.</span><span class="sxs-lookup"><span data-stu-id="ecc9b-107">Single email address: Sometimes the address needs to be synchronized; changing the smtp proxy address and then changing it back can help.</span></span>
2. <span data-ttu-id="ecc9b-108">تحديد ما إذا كانت المشكلة خاصة ب مجموعة أو مجلد عمومي.</span><span class="sxs-lookup"><span data-stu-id="ecc9b-108">Determine whether the problem is specific to a group or public folder.</span></span> <span data-ttu-id="ecc9b-109">بالنسبة لبعض أنواع العناصر، قد تحتاج الكائنات إلى إنشاء يدويا في Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="ecc9b-109">For some object types, the objects may need to be manually created in Azure Active Directory.</span></span>

<span data-ttu-id="ecc9b-110">إذا كنت بحاجة إلى مساعدة إضافية، فيرجى فتح تذكرة دعم وتحديد نطاق المشكلة (بما في ذلك نوع الكائن الذي ترسل إليه) حتى يمكننا مساعدتك بشكل أفضل.</span><span class="sxs-lookup"><span data-stu-id="ecc9b-110">If you need additional help, please open a support ticket and specify the scope of the issue (including the type of object you're sending to) so we can assist you better.</span></span>