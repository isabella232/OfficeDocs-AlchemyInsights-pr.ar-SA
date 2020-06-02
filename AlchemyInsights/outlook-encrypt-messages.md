---
title: S / MIME في Outlook على الويب
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 6bbbf8722dacb8b7d5191d57ce1055a48dcb4dd0
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511495"
---
# <a name="encrypt-email-messages-in-outlook"></a><span data-ttu-id="442fa-102">تشفير رسائل البريد الإلكتروني في Outlook</span><span class="sxs-lookup"><span data-stu-id="442fa-102">Encrypt email messages in Outlook</span></span>

<span data-ttu-id="442fa-103">تم إنشاء تشفير رسالة Microsoft 365 على Microsoft Azure Rights Management (Azure RMS)، وهو جزء من حماية معلومات Azure.</span><span class="sxs-lookup"><span data-stu-id="442fa-103">Microsoft 365 Message Encryption is built on Microsoft Azure Rights Management (Azure RMS), which is part of Azure Information Protection.</span></span> <span data-ttu-id="442fa-104">إذا كان اشتراكك يتضمن إدارة حقوق Azure أو حماية معلومات Azure، فلن تحتاج إلى اتخاذ أي إجراءات لتمكين خدمة إدارة الحقوق **أو تنشيطها يدويًا.**</span><span class="sxs-lookup"><span data-stu-id="442fa-104">If your subscription includes Azure Rights Management or Azure Information Protection, **you do not need to take any actions to manually enable or activate** the Rights Management Service.</span></span>

<span data-ttu-id="442fa-105">استنادًا إلى ملاحظات العملاء، لن نتمكن بعد الآن من تمكين قواعد تدفق بريد Exchange من تشفير البريد الإلكتروني الصادر تلقائيًا الذي يحتوي على نوع معين من المعلومات الحساسة في المستأجر الخاص بك بشكل افتراضي.</span><span class="sxs-lookup"><span data-stu-id="442fa-105">Based on customer feedback, we will no longer be enabling Exchange mail flow rules to automatically encrypt outbound email containing certain type of sensitive information in your tenant by default.</span></span> <span data-ttu-id="442fa-106">وبدلا من ذلك، نقدم تعليمات مفصلة عن كيفية القيام بذلك بأنفسكم.</span><span class="sxs-lookup"><span data-stu-id="442fa-106">Instead, we are providing detailed instructions on how you can do so yourselves.</span></span> <span data-ttu-id="442fa-107">للحصول على تفاصيل إضافية حول كيفية إنشاء قاعدة نقل لتشفير المعلومات الحساسة، راجع [هذه المقالة](https://aka.ms/OmeEtr).</span><span class="sxs-lookup"><span data-stu-id="442fa-107">For additional details on how to create a transport rule to encrypt sensitive information, see [this article](https://aka.ms/OmeEtr).</span></span>

- <span data-ttu-id="442fa-108">إذا كنت تستخدم Outlook على الويب **(OWA**سابقاً): عند إنشاء رسالة بريد إلكتروني، ما عليك سوى النقر فوق **حماية** في OWA.</span><span class="sxs-lookup"><span data-stu-id="442fa-108">If using Outlook on the Web (formerly **OWA**): When composing an email message, simply click **Protect** in OWA.</span></span> <span data-ttu-id="442fa-109">سيؤدي ذلك إلى تطبيق إذن "عدم إعادة التوجيه".</span><span class="sxs-lookup"><span data-stu-id="442fa-109">This will apply "Do not forward" permission.</span></span> <span data-ttu-id="442fa-110">انقر فوق **تغيير الإذن** واختر **تشفير** لتشفير الرسالة فقط.</span><span class="sxs-lookup"><span data-stu-id="442fa-110">Click **Change permission** and choose **Encrypt** to only encrypt the message.</span></span>

- <span data-ttu-id="442fa-111">في حالة استخدام **عميل Outlook:** لإرسال رسالة مشفرة من Outlook 2013 أو 2016، أو Outlook 2016 لنظام التشغيل Mac، حدد **أذونات الخيارات،**  >  **Permissions**ثم حدد خيار الحماية الذي تحتاجه.</span><span class="sxs-lookup"><span data-stu-id="442fa-111">If using **Outlook client**: To send an encrypted message from Outlook 2013 or 2016, or Outlook 2016 for Mac, select **Options** > **Permissions**, then select the protection option you need.</span></span>

- <span data-ttu-id="442fa-112">لتشفير كافة رسائل البريد الإلكتروني المرسلة **تلقائيًا** إلى مستلمين معينين أو مؤسسات شريكة خارجية، تحتاج إلى إنشاء قاعدة نقل تدفق بريد في مركز Exchange Admin.</span><span class="sxs-lookup"><span data-stu-id="442fa-112">To **automatically encrypt all email** sent to certain recipients or external partner organizations, you need to create a mail flow transport rule in the Exchange Admin Center.</span></span> <span data-ttu-id="442fa-113">يتم توفير تعليمات مفصلة في [هذه المقالة الدعم](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).</span><span class="sxs-lookup"><span data-stu-id="442fa-113">Detailed instructions are provided in [this support article](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).</span></span>

