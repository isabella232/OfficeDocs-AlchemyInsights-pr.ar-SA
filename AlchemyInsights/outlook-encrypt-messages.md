---
title: S/MIME في Outlook علي الويب
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 33e94eac6a2982b8036e13d17bf60015f244f2cb
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/15/2019
ms.locfileid: "40053212"
---
# <a name="encrypt-email-messages-in-outlook"></a><span data-ttu-id="835c8-102">تشفير رسائل البريد الكتروني في اوتلوك</span><span class="sxs-lookup"><span data-stu-id="835c8-102">Encrypt email messages in Outlook</span></span>

<span data-ttu-id="835c8-103">تم بناء Office 365 تشفير الرسائل علي Microsoft Azure حقوق أداره (Azure RMS) ، وهو جزء من حماية المعلومات Azure.</span><span class="sxs-lookup"><span data-stu-id="835c8-103">Office 365 Message Encryption is built on Microsoft Azure Rights Management (Azure RMS), which is part of Azure Information Protection.</span></span> <span data-ttu-id="835c8-104">إذا كان الاشتراك الخاص بك يتضمن أداره حقوق Azure أو حماية معلومات Azure ، **لا تحتاج إلى اتخاذ إيه إجراءات لتمكين أو تنشيط** "خدمه أداره الحقوق" يدويا.</span><span class="sxs-lookup"><span data-stu-id="835c8-104">If your subscription includes Azure Rights Management or Azure Information Protection, **you do not need to take any actions to manually enable or activate** the Rights Management Service.</span></span>

<span data-ttu-id="835c8-105">استنادا إلى ملاحظات العملاء ، لن نتمكن بعد الآن من تمكين قواعد تدفق بريد Exchange لتشفير البريد الكتروني الصادر تلقائيا الذي يحتوي علي نوع معين من المعلومات الحساسة في المستاجر بشكل افتراضي.</span><span class="sxs-lookup"><span data-stu-id="835c8-105">Based on customer feedback, we will no longer be enabling Exchange mail flow rules to automatically encrypt outbound email containing certain type of sensitive information in your tenant by default.</span></span> <span data-ttu-id="835c8-106">بدلا من ذلك ، نحن نقدم تعليمات مفصله حول كيف يمكنك ان تفعل ذلك بأنفسكم.</span><span class="sxs-lookup"><span data-stu-id="835c8-106">Instead, we are providing detailed instructions on how you can do so yourselves.</span></span> <span data-ttu-id="835c8-107">للحصول علي تفاصيل اضافيه حول كيفيه إنشاء قاعده نقل لتشفير المعلومات الحساسة ، راجع [هذه المقالة](https://aka.ms/OmeEtr).</span><span class="sxs-lookup"><span data-stu-id="835c8-107">For additional details on how to create a transport rule to encrypt sensitive information, see [this article](https://aka.ms/OmeEtr).</span></span>

- <span data-ttu-id="835c8-108">في حاله استخدام Outlook علي ويب ( **OWA**سابقا): عند إنشاء رسالة بريد الكتروني ، ببساطه انقر فوق **حماية** في OWA.</span><span class="sxs-lookup"><span data-stu-id="835c8-108">If using Outlook on the Web (formerly **OWA**): When composing an email message, simply click **Protect** in OWA.</span></span> <span data-ttu-id="835c8-109">سيتم تطبيق هذا الاذن "عدم الاعاده إلى الامام".</span><span class="sxs-lookup"><span data-stu-id="835c8-109">This will apply "Do not forward" permission.</span></span> <span data-ttu-id="835c8-110">انقر فوق **تغيير الاذن** واختر **تشفير** لتشفير الرسالة فقط.</span><span class="sxs-lookup"><span data-stu-id="835c8-110">Click **Change permission** and choose **Encrypt** to only encrypt the message.</span></span>

- <span data-ttu-id="835c8-111">في حاله استخدام **عميل outlook**: لإرسال رسالة مشفره من outlook 2013 أو 2016 ، أو outlook 2016 لنظام التشغيل Mac ، حدد **أذونات الخيارات** > \*\*\*\*، ثم حدد خيار الحماية الذي تحتاجه.</span><span class="sxs-lookup"><span data-stu-id="835c8-111">If using **Outlook client**: To send an encrypted message from Outlook 2013 or 2016, or Outlook 2016 for Mac, select **Options** > **Permissions**, then select the protection option you need.</span></span>

- <span data-ttu-id="835c8-112">**لتشفير كافة البريد الكتروني** المرسلة إلى بعض المستلمين أو المؤسسات الشريكة الخارجية تلقائيا ، تحتاج إلى إنشاء قاعده نقل تدفق البريد في مركز مسؤول Exchange.</span><span class="sxs-lookup"><span data-stu-id="835c8-112">To **automatically encrypt all email** sent to certain recipients or external partner organizations, you need to create a mail flow transport rule in the Exchange Admin Center.</span></span> <span data-ttu-id="835c8-113">يتم توفير تعليمات مفصله في [هذا المقال الدعم](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).</span><span class="sxs-lookup"><span data-stu-id="835c8-113">Detailed instructions are provided in [this support article](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).</span></span>

