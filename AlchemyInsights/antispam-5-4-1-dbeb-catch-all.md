---
title: مكافحة البريد المزعج 5.4.1 DBEB الصيد للجميع
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: ad0f4c691a5e06306dbb408f4d66a4e00609e4d5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43707898"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a><span data-ttu-id="4abd5-102">إصلاح مشكلات التسليم لرمز الخطأ 550 5.4.1 ترحيل الوصول رفض</span><span class="sxs-lookup"><span data-stu-id="4abd5-102">Fix delivery issues for error code 550 5.4.1 Relay Access Denied</span></span>

<span data-ttu-id="4abd5-103">تحدث هذه المشكلة عند [التحقق لمعرفة ما إذا كان عنوان البريد الإلكتروني صالحلمنع الارتدادعند](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) إدخال شبكة Microsoft.</span><span class="sxs-lookup"><span data-stu-id="4abd5-103">This problem occurs when [checking to see if an email address is valid to prevent bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) when entering the Microsoft network.</span></span> <span data-ttu-id="4abd5-104">جرّب ما يلي:</span><span class="sxs-lookup"><span data-stu-id="4abd5-104">Try the following:</span></span>

1. <span data-ttu-id="4abd5-105">تحديد ما إذا كانت المشكلة خاصة بنطاق بأكمله أو عنوان بريد إلكتروني واحد:</span><span class="sxs-lookup"><span data-stu-id="4abd5-105">Determine whether the problem is specific to an entire domain or a single email address:</span></span>
    - <span data-ttu-id="4abd5-106">المجال بأكمله: في بعض الأحيان يجب مزامنة المجال; حاول [تعيين المجال إلى داخلي ثم العودة إلى "موثوقة".](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains)</span><span class="sxs-lookup"><span data-stu-id="4abd5-106">Entire domain: Sometimes the domain needs to be synchronized; try [setting the domain to Internal and then back to Authoritative](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span></span>
    - <span data-ttu-id="4abd5-107">عنوان بريد إلكتروني واحد: في بعض الأحيان يجب مزامنة العنوان. تغيير عنوان وكيل smtp ومن ثم تغييره مرة أخرى يمكن أن يساعد.</span><span class="sxs-lookup"><span data-stu-id="4abd5-107">Single email address: Sometimes the address needs to be synchronized; changing the smtp proxy address and then changing it back can help.</span></span>
2. <span data-ttu-id="4abd5-108">تحديد ما إذا كانت المشكلة خاصة بمجموعة أو مجلد عام.</span><span class="sxs-lookup"><span data-stu-id="4abd5-108">Determine whether the problem is specific to a group or public folder.</span></span> <span data-ttu-id="4abd5-109">بالنسبة لبعض أنواع الكائنات، قد تحتاج الكائنات إلى إنشاء يدوياً في Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="4abd5-109">For some object types, the objects may need to be manually created in Azure Active Directory.</span></span>

<span data-ttu-id="4abd5-110">إذا كنت بحاجة إلى مساعدة إضافية، يرجى فتح تذكرة دعم وتحديد نطاق المشكلة (بما في ذلك نوع الكائن الذي ترسل إليه) حتى نتمكن من مساعدتك بشكل أفضل.</span><span class="sxs-lookup"><span data-stu-id="4abd5-110">If you need additional help, please open a support ticket and specify the scope of the issue (including the type of object you're sending to) so we can assist you better.</span></span>