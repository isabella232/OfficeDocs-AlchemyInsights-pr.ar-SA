---
title: S/MIME في Outlook على ويب
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: f2c047ca31c586c0aa36701e6e7ca9976cfd1734
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/29/2019
ms.locfileid: "36666827"
---
# <a name="encrypt-email-messages-in-outlook"></a><span data-ttu-id="61a36-102">تشفير رسائل البريد الإلكتروني في Outlook</span><span class="sxs-lookup"><span data-stu-id="61a36-102">Encrypt email messages in Outlook</span></span>

<span data-ttu-id="61a36-103">تشفير الرسائل office 365 تستند إلى Microsoft Azure إدارة الحقوق (RMS Azure)، التي جزء من حماية معلومات Azure.</span><span class="sxs-lookup"><span data-stu-id="61a36-103">Office 365 Message Encryption is built on Microsoft Azure Rights Management (Azure RMS), which is part of Azure Information Protection.</span></span> <span data-ttu-id="61a36-104">إذا كان يتضمن الاشتراك Azure إدارة حقوق أو حماية المعلومات أزور، **لا تحتاج إلى اتخاذ أي إجراءات لتمكين يدوياً أو تنشيط** "خدمة إدارة الحقوق".</span><span class="sxs-lookup"><span data-stu-id="61a36-104">If your subscription includes Azure Rights Management or Azure Information Protection, **you do not need to take any actions to manually enable or activate** the Rights Management Service.</span></span>

<span data-ttu-id="61a36-105">بناء على ملاحظات العملاء، أننا سوف لا يمكن تمكين Exchange قواعد تدفق البريد تلقائياً تشفير البريد الإلكتروني الصادر التي تحتوي على نوع معين من المعلومات الحساسة في المستأجر الخاص بك بشكل افتراضي.</span><span class="sxs-lookup"><span data-stu-id="61a36-105">Based on customer feedback, we will no longer be enabling Exchange mail flow rules to automatically encrypt outbound email containing certain type of sensitive information in your tenant by default.</span></span> <span data-ttu-id="61a36-106">بدلاً من ذلك، نقدم إرشادات مفصلة حول كيفية القيام بذلك أنفسكم.</span><span class="sxs-lookup"><span data-stu-id="61a36-106">Instead, we are providing detailed instructions on how you can do so yourselves.</span></span> <span data-ttu-id="61a36-107">للحصول على تفاصيل إضافية حول كيفية إنشاء قاعدة نقل لتشفير المعلومات الحساسة، راجع [هذا المقال](https://aka.ms/OmeEtr).</span><span class="sxs-lookup"><span data-stu-id="61a36-107">For additional details on how to create a transport rule to encrypt sensitive information, see [this article](https://aka.ms/OmeEtr).</span></span>

- <span data-ttu-id="61a36-108">في حالة استخدام Outlook على الويب (سابقا **OWA**): عند إنشاء رسالة بريد إلكتروني، ببساطة انقر فوق **حماية** في OWA.</span><span class="sxs-lookup"><span data-stu-id="61a36-108">If using Outlook on the Web (formerly **OWA**): When composing an email message, simply click **Protect** in OWA.</span></span> <span data-ttu-id="61a36-109">سيتم تطبيق هذا الإذن "القيام بإعادة التوجيه".</span><span class="sxs-lookup"><span data-stu-id="61a36-109">This will apply "Do not forward" permission.</span></span> <span data-ttu-id="61a36-110">انقر فوق **تغيير الإذن** واختر **تشفير** تشفير الرسالة فقط.</span><span class="sxs-lookup"><span data-stu-id="61a36-110">Click **Change permission** and choose **Encrypt** to only encrypt the message.</span></span>

- <span data-ttu-id="61a36-111">في حالة استخدام **عميل Outlook**: لإرسال رسالة مشفرة من Outlook 2013 أو 2016 أو Outlook 2016 لنظام التشغيل Mac، قم بتحديد **خيارات** > **الأذونات**، ثم قم بتحديد خيار الحماية التي تحتاجها.</span><span class="sxs-lookup"><span data-stu-id="61a36-111">If using **Outlook client**: To send an encrypted message from Outlook 2013 or 2016, or Outlook 2016 for Mac, select **Options** > **Permissions**, then select the protection option you need.</span></span>

- <span data-ttu-id="61a36-112">**تشفير كافة رسائل البريد الإلكتروني** المرسلة إلى بعض المستلمين أو المنظمات الشريكة الخارجية، تحتاج إلى إنشاء قاعدة نقل تدفق بريد في مركز مسؤول Exchange.</span><span class="sxs-lookup"><span data-stu-id="61a36-112">To **automatically encrypt all email** sent to certain recipients or external partner organizations, you need to create a mail flow transport rule in the Exchange Admin Center.</span></span> <span data-ttu-id="61a36-113">يتم توفير إرشادات مفصلة في [هذه المقالة الدعم](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).</span><span class="sxs-lookup"><span data-stu-id="61a36-113">Detailed instructions are provided in [this support article](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).</span></span>

