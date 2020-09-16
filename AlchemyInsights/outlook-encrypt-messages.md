---
title: S/MIME في Outlook علي الويب
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 052149d1f11387246bc1ff24ba48c45b944ba52c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47772249"
---
# <a name="encrypt-email-messages-in-outlook"></a><span data-ttu-id="2d009-102">تشفير رسائل البريد الكتروني في Outlook</span><span class="sxs-lookup"><span data-stu-id="2d009-102">Encrypt email messages in Outlook</span></span>

<span data-ttu-id="2d009-103">يتم إنشاء تشفير رسائل microsoft 365 علي Microsoft Azure Rights Management (Azure RMS) ، وهو جزء من حماية البيانات في Azure.</span><span class="sxs-lookup"><span data-stu-id="2d009-103">Microsoft 365 Message Encryption is built on Microsoft Azure Rights Management (Azure RMS), which is part of Azure Information Protection.</span></span> <span data-ttu-id="2d009-104">إذا كان اشتراكك يتضمن أداره الحقوق ل azure أو حماية معلومات Azure ، فلا **تحتاج إلى اتخاذ اي إجراءات لتمكين خدمه أداره الحقوق يدويا أو تنشيطها** .</span><span class="sxs-lookup"><span data-stu-id="2d009-104">If your subscription includes Azure Rights Management or Azure Information Protection, **you do not need to take any actions to manually enable or activate** the Rights Management Service.</span></span>

<span data-ttu-id="2d009-105">بالاستناد إلى ملاحظات العملاء ، لن يعود بحاجه إلى تمكين قواعد تدفقات البريد في Exchange لتشفير البريد الكتروني الصادر الذي يحتوي علي نوع معين من المعلومات الحساسة بشكل افتراضي.</span><span class="sxs-lookup"><span data-stu-id="2d009-105">Based on customer feedback, we will no longer be enabling Exchange mail flow rules to automatically encrypt outbound email containing certain type of sensitive information in your tenant by default.</span></span> <span data-ttu-id="2d009-106">بدلا من ذلك ، نقدم إرشادات مفصله حول كيفيه القيام بذلك طفرة.</span><span class="sxs-lookup"><span data-stu-id="2d009-106">Instead, we are providing detailed instructions on how you can do so yourselves.</span></span> <span data-ttu-id="2d009-107">للحصول علي مزيد من التفاصيل حول كيفيه إنشاء قاعده نقل لتشفير المعلومات الحساسة ، راجع [هذه المقالة](https://aka.ms/OmeEtr).</span><span class="sxs-lookup"><span data-stu-id="2d009-107">For additional details on how to create a transport rule to encrypt sensitive information, see [this article](https://aka.ms/OmeEtr).</span></span>

- <span data-ttu-id="2d009-108">إذا كنت تستخدم Outlook علي الويب (المعروف سابقا باسم **OWA**): عند إنشاء رسالة بريد الكتروني ، ما عليك سوي النقر فوق **حماية** في OWA.</span><span class="sxs-lookup"><span data-stu-id="2d009-108">If using Outlook on the Web (formerly **OWA**): When composing an email message, simply click **Protect** in OWA.</span></span> <span data-ttu-id="2d009-109">سيؤدي ذلك إلى تطبيق الاذن "عدم أعاده التوجيه".</span><span class="sxs-lookup"><span data-stu-id="2d009-109">This will apply "Do not forward" permission.</span></span> <span data-ttu-id="2d009-110">انقر فوق **تغيير الاذن** واختر **تشفير** لتشفير الرسالة فقط.</span><span class="sxs-lookup"><span data-stu-id="2d009-110">Click **Change permission** and choose **Encrypt** to only encrypt the message.</span></span>

- <span data-ttu-id="2d009-111">إذا كنت تستخدم **outlook client**: لإرسال رسالة مشفره من outlook 2013 أو 2016 ، أو Outlook 2016 for Mac ، حدد **الخيارات**  >  **الأذونات**، ثم حدد خيار الحماية الذي تريده.</span><span class="sxs-lookup"><span data-stu-id="2d009-111">If using **Outlook client**: To send an encrypted message from Outlook 2013 or 2016, or Outlook 2016 for Mac, select **Options** > **Permissions**, then select the protection option you need.</span></span>

- <span data-ttu-id="2d009-112">**لتشفير كل رسائل البريد الكتروني** التي يتم إرسالها إلى مستلمين معينين أو مؤسسات شركاء خارجيه ، يجب إنشاء قاعده نقل تدفق البريد في مركز أداره Exchange.</span><span class="sxs-lookup"><span data-stu-id="2d009-112">To **automatically encrypt all email** sent to certain recipients or external partner organizations, you need to create a mail flow transport rule in the Exchange Admin Center.</span></span> <span data-ttu-id="2d009-113">يتم توفير الإرشادات المفصلة في [مقاله الدعم هذه](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).</span><span class="sxs-lookup"><span data-stu-id="2d009-113">Detailed instructions are provided in [this support article](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).</span></span>

