---
title: S/MIME في Outlook على الويب
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 6915470655b85922f6f97e8ca6fac353224b1ae0
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/04/2019
ms.locfileid: "36752847"
---
# <a name="encrypt-email-messages-in-outlook"></a><span data-ttu-id="5c2f4-102">تشفير رسائل البريد الإلكتروني في أوتلوك</span><span class="sxs-lookup"><span data-stu-id="5c2f4-102">Encrypt email messages in Outlook</span></span>

<span data-ttu-id="5c2f4-103">تم إنشاء تشفير الرسائل Office 365 على إدارة حقوق Microsoft Azure (Azure RMS)، وهو جزء من حماية معلومات Azure.</span><span class="sxs-lookup"><span data-stu-id="5c2f4-103">Office 365 Message Encryption is built on Microsoft Azure Rights Management (Azure RMS), which is part of Azure Information Protection.</span></span> <span data-ttu-id="5c2f4-104">إذا كان اشتراكك يتضمن إدارة حقوق Azure أو حماية معلومات Azure، **فلن تحتاج إلى اتخاذ أية إجراءات لتمكين أو تنشيط** خدمة إدارة الحقوق يدويًا.</span><span class="sxs-lookup"><span data-stu-id="5c2f4-104">If your subscription includes Azure Rights Management or Azure Information Protection, **you do not need to take any actions to manually enable or activate** the Rights Management Service.</span></span>

<span data-ttu-id="5c2f4-105">استنادًا إلى ملاحظات العملاء، لن نتمكن بعد الآن من تمكين قواعد تدفق بريد Exchange من تشفير البريد الإلكتروني الصادر تلقائيًا الذي يحتوي على نوع معين من المعلومات الحساسة في المستأجر بشكل افتراضي.</span><span class="sxs-lookup"><span data-stu-id="5c2f4-105">Based on customer feedback, we will no longer be enabling Exchange mail flow rules to automatically encrypt outbound email containing certain type of sensitive information in your tenant by default.</span></span> <span data-ttu-id="5c2f4-106">بدلا من ذلك، نحن نقدم تعليمات مفصلة حول كيف يمكنك أن تفعل ذلك أنفسكم.</span><span class="sxs-lookup"><span data-stu-id="5c2f4-106">Instead, we are providing detailed instructions on how you can do so yourselves.</span></span> <span data-ttu-id="5c2f4-107">للحصول على تفاصيل إضافية حول كيفية إنشاء قاعدة نقل لتشفير المعلومات الحساسة، راجع [هذه المقالة](https://aka.ms/OmeEtr).</span><span class="sxs-lookup"><span data-stu-id="5c2f4-107">For additional details on how to create a transport rule to encrypt sensitive information, see [this article](https://aka.ms/OmeEtr).</span></span>

- <span data-ttu-id="5c2f4-108">في حالة استخدام Outlook على \*\*\*\* ويب (OWA سابقاً): عند إنشاء رسالة بريد إلكتروني، ببساطة انقر فوق **حماية** في OWA.</span><span class="sxs-lookup"><span data-stu-id="5c2f4-108">If using Outlook on the Web (formerly **OWA**): When composing an email message, simply click **Protect** in OWA.</span></span> <span data-ttu-id="5c2f4-109">سيؤدي هذا إلى تطبيق إذن "عدم إعادة توجيه".</span><span class="sxs-lookup"><span data-stu-id="5c2f4-109">This will apply "Do not forward" permission.</span></span> <span data-ttu-id="5c2f4-110">انقر فوق **تغيير الإذن** واختر **تشفير** لتشفير الرسالة فقط.</span><span class="sxs-lookup"><span data-stu-id="5c2f4-110">Click **Change permission** and choose **Encrypt** to only encrypt the message.</span></span>

- <span data-ttu-id="5c2f4-111">في حالة استخدام **عميل Outlook**: لإرسال رسالة مشفرة من Outlook 2013 أو 2016، أو Outlook 2016 لنظام التشغيل Mac، حدد**أذونات** **الخيارات** > ، ثم حدد خيار الحماية التي تحتاجها.</span><span class="sxs-lookup"><span data-stu-id="5c2f4-111">If using **Outlook client**: To send an encrypted message from Outlook 2013 or 2016, or Outlook 2016 for Mac, select **Options** > **Permissions**, then select the protection option you need.</span></span>

- <span data-ttu-id="5c2f4-112">لتشفير كافة **رسائل البريد الإلكتروني** المرسلة إلى مستلمين معينين أو المؤسسات الشريكة الخارجية تلقائياً، تحتاج إلى إنشاء قاعدة نقل تدفق بريد في مركز مسؤول Exchange.</span><span class="sxs-lookup"><span data-stu-id="5c2f4-112">To **automatically encrypt all email** sent to certain recipients or external partner organizations, you need to create a mail flow transport rule in the Exchange Admin Center.</span></span> <span data-ttu-id="5c2f4-113">يتم توفير تعليمات مفصلة في [هذه المقالة الدعم](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).</span><span class="sxs-lookup"><span data-stu-id="5c2f4-113">Detailed instructions are provided in [this support article](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).</span></span>

