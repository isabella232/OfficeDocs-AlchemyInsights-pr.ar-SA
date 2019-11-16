---
title: مضاد البريد المزعج 5.4.1 DBEB القبض علي جميع
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
ms.openlocfilehash: 4f531a063d63aff239ef7dead869bb526e17fb35
ms.sourcegitcommit: 2591e1f56e8943bddb9d3b77ba5b494ac49d4f30
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 11/15/2019
ms.locfileid: "38672420"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a><span data-ttu-id="a6cd6-102">إصلاح مشكلات التسليم لرمز الخطا 550 5.4.1 رفض الوصول ترحيل</span><span class="sxs-lookup"><span data-stu-id="a6cd6-102">Fix delivery issues for error code 550 5.4.1 Relay Access Denied</span></span>

<span data-ttu-id="a6cd6-103">تحدث هذه [المشكلة عند التحقق لمعرفه ما إذا كان عنوان البريد الكتروني صالح لمنع الحالات الاحتياطية](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) عند إدخال شبكه 365 Office.</span><span class="sxs-lookup"><span data-stu-id="a6cd6-103">This problem occurs when [checking to see if an email address is valid to prevent bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) when entering the Office 365 network.</span></span> <span data-ttu-id="a6cd6-104">جرب ما يلي:</span><span class="sxs-lookup"><span data-stu-id="a6cd6-104">Try the following:</span></span>

1. <span data-ttu-id="a6cd6-105">تحديد ما إذا كانت المشكلة محدده إلى مجال بأكمله أو عنوان بريد الكتروني واحد:</span><span class="sxs-lookup"><span data-stu-id="a6cd6-105">Determine whether the problem is specific to an entire domain or a single email address:</span></span>
    - <span data-ttu-id="a6cd6-106">المجال بأكمله: في بعض الأحيان يحتاج المجال إلى مزامنة; حاول [تعيين المجال إلى داخلي ثم العودة إلى مخول](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span><span class="sxs-lookup"><span data-stu-id="a6cd6-106">Entire domain: Sometimes the domain needs to be synchronized; try [setting the domain to Internal and then back to Authoritative](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span></span>
    - <span data-ttu-id="a6cd6-107">عنوان البريد الكتروني المفرد: في بعض الأحيان يجب ان تتم مزامنة العنوان; تغيير عنوان الوكيل smtp ثم تغييره مره أخرى يمكن ان تساعد.</span><span class="sxs-lookup"><span data-stu-id="a6cd6-107">Single email address: Sometimes the address needs to be synchronized; changing the smtp proxy address and then changing it back can help.</span></span>
2. <span data-ttu-id="a6cd6-108">تحديد ما إذا كانت المشكلة محدده إلى مجموعه أو مجلد عمومي.</span><span class="sxs-lookup"><span data-stu-id="a6cd6-108">Determine whether the problem is specific to a group or public folder.</span></span> <span data-ttu-id="a6cd6-109">بالنسبة لبعض أنواع الكائنات ، قد تحتاج إلى إنشاء يدويا في Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="a6cd6-109">For some object types, the objects may need to be manually created in Azure Active Directory.</span></span>

<span data-ttu-id="a6cd6-110">إذا كنت بحاجه إلى مساعده اضافيه ، يرجى فتح تذكره دعم وتحديد نطاق المشكلة (بما في ذلك نوع الكائن الذي ترسله اليه) حتى نتمكن من مساعدتك بشكل أفضل.</span><span class="sxs-lookup"><span data-stu-id="a6cd6-110">If you need additional help, please open a support ticket and specify the scope of the issue (includidng the type of object you're sending to) so we can assist you better.</span></span>