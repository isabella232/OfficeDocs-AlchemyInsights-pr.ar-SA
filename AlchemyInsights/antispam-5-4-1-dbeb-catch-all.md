---
title: أنتيسبام 5.4.1 دبيب catch-الكل
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
- "9001209"
- "3167"
ms.openlocfilehash: f9d613457ae33dc7e00f20391bbdff029500a123
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717348"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a><span data-ttu-id="461f4-102">إصلاح مشاكل التسليم لرمز الخطا 550 5.4.1 الوصول إلى الناقل الكهربائي</span><span class="sxs-lookup"><span data-stu-id="461f4-102">Fix delivery issues for error code 550 5.4.1 Relay Access Denied</span></span>

<span data-ttu-id="461f4-103">تحدث هذه [المشكلة عند التحقق مما إذا كان عنوان البريد الكتروني صالحا لمنع البونسيباكس](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) عند إدخال شبكه Microsoft.</span><span class="sxs-lookup"><span data-stu-id="461f4-103">This problem occurs when [checking to see if an email address is valid to prevent bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) when entering the Microsoft network.</span></span> <span data-ttu-id="461f4-104">جرب ما يلي:</span><span class="sxs-lookup"><span data-stu-id="461f4-104">Try the following:</span></span>

1. <span data-ttu-id="461f4-105">تحديد ما إذا كانت المشكلة خاصه بمجال كامل أو عنوان بريد الكتروني واحد:</span><span class="sxs-lookup"><span data-stu-id="461f4-105">Determine whether the problem is specific to an entire domain or a single email address:</span></span>
    - <span data-ttu-id="461f4-106">المجال بالبالكامل: يجب ان تتم مزامنة المجال في بعض الأحيان ؛ حاول [تعيين المجال إلى داخلي ثم عد إلى مخول](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span><span class="sxs-lookup"><span data-stu-id="461f4-106">Entire domain: Sometimes the domain needs to be synchronized; try [setting the domain to Internal and then back to Authoritative](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span></span>
    - <span data-ttu-id="461f4-107">عنوان البريد الكتروني الفردي: يجب ان تتم مزامنة العنوان في بعض الأحيان ؛ يمكنك تغيير عنوان وكيل smtp ثم تغييره مره أخرى.</span><span class="sxs-lookup"><span data-stu-id="461f4-107">Single email address: Sometimes the address needs to be synchronized; changing the smtp proxy address and then changing it back can help.</span></span>
2. <span data-ttu-id="461f4-108">تحديد ما إذا كانت المشكلة خاصه بمجموعه أو مجلد عمومي.</span><span class="sxs-lookup"><span data-stu-id="461f4-108">Determine whether the problem is specific to a group or public folder.</span></span> <span data-ttu-id="461f4-109">بالنسبة إلى بعض أنواع الكائنات ، قد تحتاج إلى إنشاء الكائنات يدويا في Azure Active directory.</span><span class="sxs-lookup"><span data-stu-id="461f4-109">For some object types, the objects may need to be manually created in Azure Active Directory.</span></span>

<span data-ttu-id="461f4-110">إذا كنت بحاجه إلى مزيد من المساعدة ، يرجى فتح بطاقة دعم وتحديد نطاق المشكلة (بما في ذلك نوع الكائن الذي ترسله اليه) بحيث يمكننا مساعدتك بشكل أفضل.</span><span class="sxs-lookup"><span data-stu-id="461f4-110">If you need additional help, please open a support ticket and specify the scope of the issue (including the type of object you're sending to) so we can assist you better.</span></span>