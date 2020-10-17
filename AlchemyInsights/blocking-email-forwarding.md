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
ms.openlocfilehash: 2f3528375d251542fd82761d00c776706de2e23c
ms.sourcegitcommit: f7b82f75a5400e992ecbd48a666783354e2e2871
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/15/2020
ms.locfileid: "48473088"
---
# <a name="blocking-or-unblocking-email-forwarding"></a><span data-ttu-id="3880f-102">حظر أعاده توجيه البريد الكتروني أو إلغاء حظره</span><span class="sxs-lookup"><span data-stu-id="3880f-102">Blocking or unblocking email forwarding</span></span>

<span data-ttu-id="3880f-103">لتمكين أعاده توجيه البريد الكتروني لعلبه بريد معينه أو تعطيلها ، راجع [تكوين أعاده توجيه البريد الكتروني](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span><span class="sxs-lookup"><span data-stu-id="3880f-103">To enable or disable email forwarding for a specific mailbox, see [Configure email forwarding](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span></span>

<span data-ttu-id="3880f-104">علي مستوي المستاجر ، يتم التحكم في أعاده التوجيه الخارجي باستخدام نهج البريد العشوائي الصادر.</span><span class="sxs-lookup"><span data-stu-id="3880f-104">On the tenant level, control of external forwarding is done using the outbound spam policy.</span></span> <span data-ttu-id="3880f-105">يمكنك التحقق من نهج تصفيه البريد العشوائي الصادر من مركز الأمان والتوافق [هنا] ( https://protection.office.com/antispam) أو باستخدام [الأمر Get هوستيدوتبوندسبامفيلتيربوليسي](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy).</span><span class="sxs-lookup"><span data-stu-id="3880f-105">You can check the outbound spam filter policy from Security and Compliance Center [here] (https://protection.office.com/antispam) or by using the [Get-HostedOutboundSpamFilterPolicy command](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy).</span></span>

<span data-ttu-id="3880f-106">إذا ظهرت رسالة الخطا التالية: **"550 5.7.520 تم رفض الوصول ، فلا تسمح مؤسستك باعاده التوجيه الخارجي"**، الرجاء التاكد من تكوين النهج لتمكين الإرسال التلقائي الخارجي.</span><span class="sxs-lookup"><span data-stu-id="3880f-106">If you are getting the following error: **“550 5.7.520 Access denied, Your organization does not allow external forwarding”**, please make sure the policy is configured to enable External Auto-forward.</span></span>

<span data-ttu-id="3880f-107">**ملاحظه:** من المستحسن الإبقاء علي أوتوفوروارد الخارجي معطلا علي نهج تصفيه البريد الكتروني الصادر الافتراضي وتمكينه فقط للمستخدمين الذين يحتاجون إلى أعاده توجيه خارجيه من خلال إنشاء نهج مخصص لهؤلاء المستخدمين.</span><span class="sxs-lookup"><span data-stu-id="3880f-107">**Note:** It is recommended to keep the External Autoforward disabled on your default outbound spam filter policy and enable it only for the users who need external forwarding by creating a custom policy for those users.</span></span> <span data-ttu-id="3880f-108">يمكنك قراءه المزيد في [تكوين أعاده توجيه البريد الكتروني الخارجي في Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).</span><span class="sxs-lookup"><span data-stu-id="3880f-108">You can read more in [Configuring external email forwarding in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).</span></span>