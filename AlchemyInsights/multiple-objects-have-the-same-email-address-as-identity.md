---
title: تحتوي الكائنات المتعددة على نفس عنوان البريد الإلكتروني كـ الهوية
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1834"
- "9000247"
ms.openlocfilehash: cc932aa7ecbd1e338c409a7a6525e2c4e673b232
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 07/28/2020
ms.locfileid: "45438673"
---
# <a name="multiple-objects-have-the-same-email-address-as-identity"></a><span data-ttu-id="48a9f-102">تحتوي الكائنات المتعددة على نفس عنوان البريد الإلكتروني كـ الهوية</span><span class="sxs-lookup"><span data-stu-id="48a9f-102">Multiple objects have the same email address as identity</span></span>

<span data-ttu-id="48a9f-103">**كائنات متعددة**</span><span class="sxs-lookup"><span data-stu-id="48a9f-103">**Multiple objects**</span></span>

<span data-ttu-id="48a9f-104">أحد الأسباب الشائعة لهذا الخطأ هو عدم القدرة على توجيه طلب Outlook Web Access بشكل صحيح في وجود كائنات متعددة لها نفس عنوان البريد الإلكتروني كهوية.</span><span class="sxs-lookup"><span data-stu-id="48a9f-104">One of the common reasons of this error is not being able to route an Outlook Web Access request properly in a presence of multiple objects having the same email address as identity.</span></span> <span data-ttu-id="48a9f-105">للبحث عن هذه الكائنات، قم بتشغيل الأوامر التالية:</span><span class="sxs-lookup"><span data-stu-id="48a9f-105">To find these objects, run the following commands:</span></span>

<span data-ttu-id="48a9f-106">· الحصول على مستلم<email address></span><span class="sxs-lookup"><span data-stu-id="48a9f-106">· Get-Recipient <email address></span></span>

<span data-ttu-id="48a9f-107">· الحصول على المستخدم<email address></span><span class="sxs-lookup"><span data-stu-id="48a9f-107">· Get-User <email address></span></span>

<span data-ttu-id="48a9f-108">· الحصول على المستخدم <email address> -SoftDeletedUser</span><span class="sxs-lookup"><span data-stu-id="48a9f-108">· Get-User <email address> -SoftDeletedUser</span></span>

<span data-ttu-id="48a9f-109">· الحصول على الاتصال<email address></span><span class="sxs-lookup"><span data-stu-id="48a9f-109">· Get-Contact <email address></span></span>

<span data-ttu-id="48a9f-110">· الحصول على علبة البريد <email address> -PublicFolder</span><span class="sxs-lookup"><span data-stu-id="48a9f-110">· Get-Mailbox <email address> -PublicFolder</span></span>

<span data-ttu-id="48a9f-111">· الحصول على علبة البريد <email address> -IncludeSoftDeletedميلبوك</span><span class="sxs-lookup"><span data-stu-id="48a9f-111">· Get-Mailbox <email address> -IncludeSoftDeletedMailbox</span></span>

<span data-ttu-id="48a9f-112">· الحصول على علبة البريد <email address> -غير نشطالبريد الإلكتروني فقط</span><span class="sxs-lookup"><span data-stu-id="48a9f-112">· Get-Mailbox <email address> -InactiveMailboxOnly</span></span>

<span data-ttu-id="48a9f-113">لحل هذه المشكلة، إزالة كائنات متعددة بنفس هوية البريد الإلكتروني وتأكد من وجود كائن واحد مع هوية البريد الإلكتروني المحدد وأن نوع المستلم الخاص به هو UserMailbox.</span><span class="sxs-lookup"><span data-stu-id="48a9f-113">To resolve the issue, remove multiple objects with the same email identity and make sure that there is a single object with the specific email identity and that its recipient type is UserMailbox.</span></span>

<span data-ttu-id="48a9f-114">**يستخدم نفس العنوان لصناديق البريد الخاصة بالعمل والمستهلك**</span><span class="sxs-lookup"><span data-stu-id="48a9f-114">**Same address is used for business and consumer mailboxes**</span></span>

<span data-ttu-id="48a9f-115">سبب آخر هو عند استخدام نفس العنوان لصناديق البريد الأعمال والمستهلك.</span><span class="sxs-lookup"><span data-stu-id="48a9f-115">Another cause is when the same address is used for business and consumer mailboxes.</span></span> <span data-ttu-id="48a9f-116">في هذه الحالة، يجب على المستخدم تغيير الاسم المستعار المستهلك الأساسي حتى يدعم Cafe هذا السيناريو.</span><span class="sxs-lookup"><span data-stu-id="48a9f-116">In this case, the user must change their primary consumer alias until Cafe supports this scenario.</span></span> <span data-ttu-id="48a9f-117">هذا خطأ دائم لا يذهب بعيدا دون تدخل.</span><span class="sxs-lookup"><span data-stu-id="48a9f-117">This is a permanent error that does not go away without intervention.</span></span>

<span data-ttu-id="48a9f-118">للحصول على التفاصيل، راجع [تغيير عنوان البريد الإلكتروني أو رقم الهاتف لحساب Microsoft الخاص بك](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account).</span><span class="sxs-lookup"><span data-stu-id="48a9f-118">For details, see [Change the email address or phone number for your Microsoft account](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account).</span></span>