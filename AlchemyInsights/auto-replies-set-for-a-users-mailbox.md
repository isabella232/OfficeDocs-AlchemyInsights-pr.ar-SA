---
title: تعيين الردود التلقائية لعبة البريد
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000761"
- "3514"
ms.openlocfilehash: aeeb2e1e76fe602d2767b422797452fd1155fdd5
ms.sourcegitcommit: fdfd41c2bfb2d45003b3906e6469377384a91cb5
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2020
ms.locfileid: "43509474"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a><span data-ttu-id="13d5e-102">تعيين الردود التلقائية لعلبة بريد المستخدم</span><span class="sxs-lookup"><span data-stu-id="13d5e-102">Set auto replies for a user's mailbox</span></span>

<span data-ttu-id="13d5e-103">**الطريقة 1**</span><span class="sxs-lookup"><span data-stu-id="13d5e-103">**Method 1**</span></span>

1. <span data-ttu-id="13d5e-104">سجّل الدخول إلى مدخل Office 365.</span><span class="sxs-lookup"><span data-stu-id="13d5e-104">Sign in to the Office 365 portal.</span></span>

2. <span data-ttu-id="13d5e-105">انتقل إلى **المستخدمون > المستخدمون النشطاء** (أو **المجموعات > علب البريد المشتركة** إذا قمت بتعيين ذلك في علبة بريد مشتركة).</span><span class="sxs-lookup"><span data-stu-id="13d5e-105">Go to **Users > Active users** (or **Groups > Shared mailboxes** if you set this on a shared mailbox).</span></span>

3. <span data-ttu-id="13d5e-106">حدد المستخدم الذي يمتلك علبة بريد Microsoft Exchange.</span><span class="sxs-lookup"><span data-stu-id="13d5e-106">Select a user who has a Microsoft Exchange mailbox.</span></span>

4. <span data-ttu-id="13d5e-107">في القائمة الثانوية على اليسار، انتقل إلى **إعدادات البريد > الردود التلقائية** (إذا كانت علبة البريد مشتركة، فما عليك سوى النقر فوق **الردود التلقائية** في القائمة الثانوية).</span><span class="sxs-lookup"><span data-stu-id="13d5e-107">On the fly-out menu on the right, go to **Mail settings > Automatic replies** (if it's a shared mailbox, just click **Automatic replies** on the fly-out).</span></span>

<span data-ttu-id="13d5e-108">**الطريقة 2**</span><span class="sxs-lookup"><span data-stu-id="13d5e-108">**Method 2**</span></span>

1. <span data-ttu-id="13d5e-109">سجّل الدخول إلى مدخل مسؤول Office 365 باستخدام بيانات اعتماد المسؤول.</span><span class="sxs-lookup"><span data-stu-id="13d5e-109">Sign in to the Office 365 admin portal by using administrator credentials.</span></span>

2. <span data-ttu-id="13d5e-110">قم بتوسيع **مراكز المسؤولين** ثم انقر فوق **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="13d5e-110">Expand **Admin Centers**, and then click **Exchange**.</span></span>

3. <span data-ttu-id="13d5e-111">انقر فوق الصورة الموجودة أعلى الزاوية اليسرى وانقر فوق **مستخدم آخر** ثم حدد علبة بريد المستخدم المراد تغييرها.</span><span class="sxs-lookup"><span data-stu-id="13d5e-111">Click the picture in the upper-right corner, click **Another User**, and then select the user mailbox that you want to change.</span></span>

4. <span data-ttu-id="13d5e-112">على الجانب الأيمن، حدد **الخيارات** وانقر فوق **تنظيم البريد الإلكتروني** ثم انقر فوق **الردود التلقائية.**</span><span class="sxs-lookup"><span data-stu-id="13d5e-112">On the left side, select **Options**, click **Organize E-mail**, and then click **Automatic replies.**</span></span>

<span data-ttu-id="13d5e-113">**الطريقة 3**</span><span class="sxs-lookup"><span data-stu-id="13d5e-113">**Method 3**</span></span>

<span data-ttu-id="13d5e-114">قم بتشغيل أمر cmdlet التالي في Exchange Online PowerShell:</span><span class="sxs-lookup"><span data-stu-id="13d5e-114">Run the following cmdlet in Exchange Online PowerShell:</span></span>

<span data-ttu-id="13d5e-115">PowerShellCopy</span><span class="sxs-lookup"><span data-stu-id="13d5e-115">PowerShellCopy</span></span>

```
    Set-MailboxAutoReplyConfiguration
```

<span data-ttu-id="13d5e-116">للحصول على مزيد من المعلومات حول أمر cmdlet هذا، اطلع على [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).</span><span class="sxs-lookup"><span data-stu-id="13d5e-116">For more information about this cmdlet, see [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).</span></span>
