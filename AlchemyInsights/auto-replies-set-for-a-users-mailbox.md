---
title: تعيين الردود التلقائية لعبة البريد
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
- "9000761"
- "3514"
ms.openlocfilehash: 03c530e7ce5f00fce2222cf9993930b97e5a2818
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47715116"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a><span data-ttu-id="e4632-102">تعيين الردود التلقائية لعلبة بريد المستخدم</span><span class="sxs-lookup"><span data-stu-id="e4632-102">Set auto replies for a user's mailbox</span></span>

<span data-ttu-id="e4632-103">**الطريقة 1**</span><span class="sxs-lookup"><span data-stu-id="e4632-103">**Method 1**</span></span>

1. <span data-ttu-id="e4632-104">سجّل الدخول إلى مدخل Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="e4632-104">Sign in to the Microsoft 365 portal.</span></span>

2. <span data-ttu-id="e4632-105">انتقل إلى **المستخدمون > المستخدمون النشطاء** (أو **المجموعات > علب البريد المشتركة** إذا قمت بتعيين ذلك في علبة بريد مشتركة).</span><span class="sxs-lookup"><span data-stu-id="e4632-105">Go to **Users > Active users** (or **Groups > Shared mailboxes** if you set this on a shared mailbox).</span></span>

3. <span data-ttu-id="e4632-106">حدد المستخدم الذي يمتلك علبة بريد Microsoft Exchange.</span><span class="sxs-lookup"><span data-stu-id="e4632-106">Select a user who has a Microsoft Exchange mailbox.</span></span>

4. <span data-ttu-id="e4632-107">في القائمة الثانوية على اليسار، انتقل إلى **إعدادات البريد > الردود التلقائية** (إذا كانت علبة البريد مشتركة، فما عليك سوى النقر فوق **الردود التلقائية** في القائمة الثانوية).</span><span class="sxs-lookup"><span data-stu-id="e4632-107">On the fly-out menu on the right, go to **Mail settings > Automatic replies** (if it's a shared mailbox, just click **Automatic replies** on the fly-out).</span></span>

<span data-ttu-id="e4632-108">**الطريقة 2**</span><span class="sxs-lookup"><span data-stu-id="e4632-108">**Method 2**</span></span>

1. <span data-ttu-id="e4632-109">سجّل الدخول إلى مدخل مسؤولي Microsoft 365 باستخدام بيانات اعتماد المسؤول.</span><span class="sxs-lookup"><span data-stu-id="e4632-109">Sign in to the Microsoft 365 admin portal by using administrator credentials.</span></span>

2. <span data-ttu-id="e4632-110">قم بتوسيع **مراكز المسؤولين** ثم انقر فوق **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="e4632-110">Expand **Admin Centers**, and then click **Exchange**.</span></span>

3. <span data-ttu-id="e4632-111">انقر فوق الصورة الموجودة أعلى الزاوية اليسرى وانقر فوق **مستخدم آخر** ثم حدد علبة بريد المستخدم المراد تغييرها.</span><span class="sxs-lookup"><span data-stu-id="e4632-111">Click the picture in the upper-right corner, click **Another User**, and then select the user mailbox that you want to change.</span></span>

4. <span data-ttu-id="e4632-112">على الجانب الأيمن، حدد **الخيارات** وانقر فوق **تنظيم البريد الإلكتروني** ثم انقر فوق **الردود التلقائية.**</span><span class="sxs-lookup"><span data-stu-id="e4632-112">On the left side, select **Options**, click **Organize E-mail**, and then click **Automatic replies.**</span></span>

<span data-ttu-id="e4632-113">**الطريقة 3**</span><span class="sxs-lookup"><span data-stu-id="e4632-113">**Method 3**</span></span>

<span data-ttu-id="e4632-114">قم بتشغيل أمر cmdlet التالي في Exchange Online PowerShell:</span><span class="sxs-lookup"><span data-stu-id="e4632-114">Run the following cmdlet in Exchange Online PowerShell:</span></span>

<span data-ttu-id="e4632-115">PowerShellCopy</span><span class="sxs-lookup"><span data-stu-id="e4632-115">PowerShellCopy</span></span>

```
    Set-MailboxAutoReplyConfiguration
```

<span data-ttu-id="e4632-116">للحصول على مزيد من المعلومات حول أمر cmdlet هذا، اطلع على [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).</span><span class="sxs-lookup"><span data-stu-id="e4632-116">For more information about this cmdlet, see [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).</span></span>
