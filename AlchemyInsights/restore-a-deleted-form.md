---
title: استعادة نموذج محذوف
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
- "2547"
- "9000672"
ms.openlocfilehash: 48018accc23a504c34b5469c198d6f29929d25c2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51809462"
---
# <a name="restore-a-deleted-form"></a><span data-ttu-id="af1ac-102">استعادة نموذج محذوف</span><span class="sxs-lookup"><span data-stu-id="af1ac-102">Restore a deleted form</span></span>

<span data-ttu-id="af1ac-103">إذا قمت بحذف نموذج في Microsoft Forms عن طريق الخطأ، يمكنك استرداده.</span><span class="sxs-lookup"><span data-stu-id="af1ac-103">If you deleted a form in Microsoft Forms by accident, you can recover it.</span></span> <span data-ttu-id="af1ac-104">سجل الدخول إلى Microsoft Forms بمالك النموذج المحذوف.</span><span class="sxs-lookup"><span data-stu-id="af1ac-104">Sign in to Microsoft Forms as the owner of the deleted form.</span></span> <span data-ttu-id="af1ac-105">حدد **سلة المهملات**، ثم حدد النموذج الذي تريد استرداده وحدد **استعادة**.</span><span class="sxs-lookup"><span data-stu-id="af1ac-105">Select the **Recycle Bin**, then select the form you want to recover and select **Restore**.</span></span> <span data-ttu-id="af1ac-106">بمجرد استعادته، حدد سهم **صفحة الرجوع إلى النماذج.**</span><span class="sxs-lookup"><span data-stu-id="af1ac-106">Once restored, select the **Back to my Forms page** arrow.</span></span>

<span data-ttu-id="af1ac-107">يمكن لمالك النموذج فقط استرداده.</span><span class="sxs-lookup"><span data-stu-id="af1ac-107">Only the owner of the form can recover it.</span></span> <span data-ttu-id="af1ac-108">إذا تم تعطيل حساب مالك النموذج أو إزالته من المستأجر، يمكن للمسؤول العام فقط استرداد النموذج.</span><span class="sxs-lookup"><span data-stu-id="af1ac-108">If form owner's account was disabled or removed from the tenant, only the Global Administrator can recover the form.</span></span> <span data-ttu-id="af1ac-109">يجب أن يكون لدى المسؤول العام ترخيص Forms لإجراء عملية استعادة.</span><span class="sxs-lookup"><span data-stu-id="af1ac-109">The Global Administrator must have a Forms license to perform a restore.</span></span> <span data-ttu-id="af1ac-110">لا يمكن استعادة سوى النماذج التي تم إنشاؤها في غضون 30 يوما من تعطيل حساب المستخدم أو إزالته من نطاق المستأجر.</span><span class="sxs-lookup"><span data-stu-id="af1ac-110">Only forms created within 30 days of the user account being disabled or removed from the tenant can be restored.</span></span>

<span data-ttu-id="af1ac-111">إذا كنت المسؤول العام للمستأجر، وتريد استرداد نموذج من حساب تم حذفه أو تعطيله، فاستبدل [عنوان البريد الإلكتروني] وعنوان البريد الإلكتروني للمستخدم المحذوف أو المعطل في عنوان URL التالي: [عنوان البريد **https://forms.office.com/Pages/delegatepage.aspx?originalowner= الإلكتروني]** على سبيل المثال، إذا كان عنوان بريدك الإلكتروني johndoe@contoso.com، سيكون عنوان URL: **https://forms.office.com/Pages/delegatepage.aspx?originalowner=johndoe@contoso.com** .</span><span class="sxs-lookup"><span data-stu-id="af1ac-111">If you are the Global Administrator of the tenant, and you want to recover a form from an account that was deleted or disabled, replace [email address] with the email address of the deleted or disabled user in the following URL: **https://forms.office.com/Pages/delegatepage.aspx?originalowner=[email address]** For example, if your email address is johndoe@contoso.com, the URL would be: **https://forms.office.com/Pages/delegatepage.aspx?originalowner=johndoe@contoso.com**.</span></span> 

<span data-ttu-id="af1ac-112">بمجرد حصولك على حق الوصول إلى النماذج المحذوفة للمستخدم، حدد النموذج الذي تريد نقله، ثم حدد **المزيد من إجراءات** النموذج  >  **نقل**.</span><span class="sxs-lookup"><span data-stu-id="af1ac-112">Once you have access to the user's deleted forms, select the form you want to move, and then select **More Form Actions** > **Move**.</span></span>

<span data-ttu-id="af1ac-113">إذا كنت تريد استرداد نموذج تم حذفه منه وإزالة المستخدم من المؤسسة، يمكن للمسؤول العام اختيار استرداد المستخدم وإعادة تعيين كلمة المرور لذلك المستخدم، ثم عند تسجيل الدخول كمستخدم، يمكنك الوصول إلى النموذج لنقله إلى مستخدم نشط آخر.</span><span class="sxs-lookup"><span data-stu-id="af1ac-113">If you want to recover a form where it was deleted and the user was removed from the organization, a Global Administrator can choose to recover the user, reset the password for that user, and then while logged in as that user, access the form to move it to another active user.</span></span> 