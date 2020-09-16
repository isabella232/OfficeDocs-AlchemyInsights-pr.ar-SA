---
title: تحتوي العناصر المتعددة علي عنوان البريد الكتروني نفسه كهوية
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1834"
- "9000247"
ms.openlocfilehash: 05fb43133bc68b71ccdbab44d28679a1f659e762
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47724602"
---
# <a name="multiple-objects-have-the-same-email-address-as-identity"></a><span data-ttu-id="1cce0-102">تحتوي العناصر المتعددة علي عنوان البريد الكتروني نفسه كهوية</span><span class="sxs-lookup"><span data-stu-id="1cce0-102">Multiple objects have the same email address as identity</span></span>

<span data-ttu-id="1cce0-103">**كائنات متعددة**</span><span class="sxs-lookup"><span data-stu-id="1cce0-103">**Multiple objects**</span></span>

<span data-ttu-id="1cce0-104">لا يمكن لأحد الأسباب الشائعة لهذا الخطا توجيه طلب Outlook Web Access بشكل صحيح في حاله وجود عده كائنات تحتوي علي عنوان البريد الكتروني نفسه كهوية.</span><span class="sxs-lookup"><span data-stu-id="1cce0-104">One of the common reasons of this error is not being able to route an Outlook Web Access request properly in a presence of multiple objects having the same email address as identity.</span></span> <span data-ttu-id="1cce0-105">للعثور علي هذه العناصر ، قم بتشغيل الأوامر التالية:</span><span class="sxs-lookup"><span data-stu-id="1cce0-105">To find these objects, run the following commands:</span></span>

<span data-ttu-id="1cce0-106">· الحصول علي المستلم <email address></span><span class="sxs-lookup"><span data-stu-id="1cce0-106">· Get-Recipient <email address></span></span>

<span data-ttu-id="1cce0-107">· الحصول علي المستخدم <email address></span><span class="sxs-lookup"><span data-stu-id="1cce0-107">· Get-User <email address></span></span>

<span data-ttu-id="1cce0-108">· الحصول علي المستخدم <email address> -سوفتديليتيدوسير</span><span class="sxs-lookup"><span data-stu-id="1cce0-108">· Get-User <email address> -SoftDeletedUser</span></span>

<span data-ttu-id="1cce0-109">· الحصول علي جهة اتصال <email address></span><span class="sxs-lookup"><span data-stu-id="1cce0-109">· Get-Contact <email address></span></span>

<span data-ttu-id="1cce0-110">· الحصول علي علبه بريد <email address> -بوبليكفولدير</span><span class="sxs-lookup"><span data-stu-id="1cce0-110">· Get-Mailbox <email address> -PublicFolder</span></span>

<span data-ttu-id="1cce0-111">· الحصول علي علبه بريد <email address> -إينكلوديسوفتديليتيدمايلبوكس</span><span class="sxs-lookup"><span data-stu-id="1cce0-111">· Get-Mailbox <email address> -IncludeSoftDeletedMailbox</span></span>

<span data-ttu-id="1cce0-112">· الحصول علي علبه بريد <email address> -إيناكتيفيمايلبوكسونلي</span><span class="sxs-lookup"><span data-stu-id="1cce0-112">· Get-Mailbox <email address> -InactiveMailboxOnly</span></span>

<span data-ttu-id="1cce0-113">لحل هذه المشكلة ، قم بازاله كائنات متعددة باستخدام هويه البريد الكتروني نفسها وتاكد من وجود كائن واحد بهويه البريد الكتروني المحددة ومن ان نوع المستلم الخاص به هو أوسيرمايلبوكس.</span><span class="sxs-lookup"><span data-stu-id="1cce0-113">To resolve the issue, remove multiple objects with the same email identity and make sure that there is a single object with the specific email identity and that its recipient type is UserMailbox.</span></span>

<span data-ttu-id="1cce0-114">**يتم استخدام العنوان نفسه لعلب بريد الاعمال والعملاء**</span><span class="sxs-lookup"><span data-stu-id="1cce0-114">**Same address is used for business and consumer mailboxes**</span></span>

<span data-ttu-id="1cce0-115">والسبب الآخر هو عند استخدام العنوان نفسه لعلب بريد العمل والعملاء.</span><span class="sxs-lookup"><span data-stu-id="1cce0-115">Another cause is when the same address is used for business and consumer mailboxes.</span></span> <span data-ttu-id="1cce0-116">في هذه الحالة ، يجب ان يقوم المستخدم بتغيير الاسم المستعار للمستهلك الأساسي الخاص به حتى يعتمد مقهى هذا السيناريو.</span><span class="sxs-lookup"><span data-stu-id="1cce0-116">In this case, the user must change their primary consumer alias until Cafe supports this scenario.</span></span> <span data-ttu-id="1cce0-117">هذا خطا دائم لا يتم الوصول اليه بدون تدخل.</span><span class="sxs-lookup"><span data-stu-id="1cce0-117">This is a permanent error that does not go away without intervention.</span></span>

<span data-ttu-id="1cce0-118">للحصول علي التفاصيل ، راجع [تغيير عنوان البريد الكتروني أو رقم الهاتف لحساب Microsoft الخاص بك](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account).</span><span class="sxs-lookup"><span data-stu-id="1cce0-118">For details, see [Change the email address or phone number for your Microsoft account](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account).</span></span>