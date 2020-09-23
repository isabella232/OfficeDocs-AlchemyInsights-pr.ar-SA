---
title: 726 حظر أعاده توجيه البريد الكتروني
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "726"
- "1200004"
ms.assetid: 8865c68e-7e8a-4135-a254-d7f69f1ded30
ms.openlocfilehash: c0d9ed14f83d3c7d47e1728d5ed9ca3a19412ad2
ms.sourcegitcommit: f74c9698a31634154ce58dda8b3145bb10685ace
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/23/2020
ms.locfileid: "48219842"
---
# <a name="blocking-or-unblocking-email-forwarding"></a><span data-ttu-id="eaedf-102">حظر أعاده توجيه البريد الكتروني أو إلغاء حظره</span><span class="sxs-lookup"><span data-stu-id="eaedf-102">Blocking or unblocking email forwarding</span></span>

<span data-ttu-id="eaedf-103">لتمكين أعاده توجيه البريد الكتروني لعلبه بريد معينه أو تعطيلها ، راجع [تكوين أعاده توجيه البريد الكتروني](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span><span class="sxs-lookup"><span data-stu-id="eaedf-103">To enable or disable email forwarding for a specific mailbox, see [Configure email forwarding](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span></span>

<span data-ttu-id="eaedf-104">علي مستوي المستاجر ، يتم التحكم في أعاده التوجيه الخارجي باستخدام نهج الحماية من البريد العشوائي الصادر.</span><span class="sxs-lookup"><span data-stu-id="eaedf-104">On the tenant level, control of External forwarding is done using the outbound anti-spam policy.</span></span> <span data-ttu-id="eaedf-105">إذا تم تعيينه إلى إيقاف التشغيل أو التلقائي ، فقد يؤدي ذلك إلى منع أعاده توجيه البريد الكتروني باستخدام "550 5.7.520 Access</span><span class="sxs-lookup"><span data-stu-id="eaedf-105">If it is set to Off or Automatic, it might block email forwarding with the “550 5.7.520 Access denied, Your organization does not allow external forwarding” error.</span></span> <span data-ttu-id="eaedf-106">التالي ، إذا تم تعيين أعاده التوجيه إلى محظور ، فهذا يعني ان الخطا سيشاهده المستخدمون.</span><span class="sxs-lookup"><span data-stu-id="eaedf-106">Subsequently, if forwarding was set to be blocked, that is the error your users will see.</span></span>

<span data-ttu-id="eaedf-107">إذا تم حظر أعاده التوجيه ، فالرجاء التاكد من تكوين النهج لتمكين الأوتوفوروارد الخارجي.</span><span class="sxs-lookup"><span data-stu-id="eaedf-107">If forwarding is being blocked, please make sure the policy is configured to enable External Autoforward.</span></span> <span data-ttu-id="eaedf-108">يمكنك التحقق من نهج تصفيه البريد العشوائي الصادر من مركز الأمان والتوافق أو عن طريق تشغيل الأمر هوستيدوتبوندسبامفيلتيربوليسي | fl name, أوتوفورواردينجمودي.</span><span class="sxs-lookup"><span data-stu-id="eaedf-108">You can check the Outbound Spam Filter Policy from Security and Compliance Center or by running command Get-HostedOutboundSpamFilterPolicy | fl name,AutoForwardingMode.</span></span> <span data-ttu-id="eaedf-109">إذا كنت تريد اعداد حظر أوتوفوروارد ، سيعلمك الأمر نفسه بحاله النهج الآن.</span><span class="sxs-lookup"><span data-stu-id="eaedf-109">If you want to set up Autoforward blocking, the same command will tell you the state of policy now.</span></span>

<span data-ttu-id="eaedf-110">ملاحظه: يوصي بالاحتفاظ بالأوتوفوروارد الخارجية معطلا علي نهج تصفيه البريد الكتروني الصادر الافتراضي وتمكينها فقط للمستخدمين الذين يحتاجون إلى أعاده توجيه خارجيه عن طريق إنشاء نهج مخصص لهؤلاء المستخدمين.</span><span class="sxs-lookup"><span data-stu-id="eaedf-110">Note: It is recommended to keep the External Autoforward disabled on your Default Outbound Spam Filter Policy and enable it only for the users who need external forwarding by creating a custom policy for those users.</span></span> <span data-ttu-id="eaedf-111">يمكنك قراءه المزيد في [تكوين أعاده توجيه البريد الكتروني الخارجي في Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).</span><span class="sxs-lookup"><span data-stu-id="eaedf-111">You can read more in [Configuring external email forwarding in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).</span></span>