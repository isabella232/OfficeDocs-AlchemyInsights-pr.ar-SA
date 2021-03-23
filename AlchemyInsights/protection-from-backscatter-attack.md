---
title: الحماية من هجوم Backscatter
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/18/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9779"
- "9005743"
ms.openlocfilehash: 8d9214fe2f5d55a21c72296421dd837d7f1d7e7d
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/19/2021
ms.locfileid: "51034785"
---
# <a name="protection-from-backscatter-attack"></a><span data-ttu-id="06dc1-102">الحماية من هجوم Backscatter</span><span class="sxs-lookup"><span data-stu-id="06dc1-102">Protection from Backscatter attack</span></span>

<span data-ttu-id="06dc1-103">إن الرسالة المرتد هي تقارير بعدم التسليم (تعرف أيضا بالتقارير بعدم التسليم أو رسائل البريد المرتد) التي تتلقاها للرسائل التي لم ترسلها.</span><span class="sxs-lookup"><span data-stu-id="06dc1-103">Backscatter is non-delivery reports (also known as NDRs or bounce messages) you receive for messages that you did not send.</span></span> <span data-ttu-id="06dc1-104">تزييف مرسلي البريد العشوائي (الانتحال) عنوان **من:** لرسائلهم، وغالبا ما يستخدمون عناوين البريد الإلكتروني الحقيقية لمصداقية رسائلهم.</span><span class="sxs-lookup"><span data-stu-id="06dc1-104">Spammers forge (spoof) the **From:** address of their messages, and they often use real email addresses to lend credibility to their messages.</span></span> <span data-ttu-id="06dc1-105">وبالتالي، عندما يرسل مرسلو البريد العشوائي رسائل حتما إلى مستلمين غير موجودين، يتم خداع خادم البريد الإلكتروني الوجهة بشكل أساسي لإرجاع الرسالة غير القابلة للرسالة غير القابلة للرسالة في عدم التسليم إلى المرسل المزيف في العنوان **من:** .</span><span class="sxs-lookup"><span data-stu-id="06dc1-105">So, when spammers inevitably send messages to non-existent recipients, the destination email server is essentially tricked into returning the undeliverable message in an NDR to the forged sender in the **From:** address.</span></span>

<span data-ttu-id="06dc1-106">يمكن العثور على معلومات إضافية في [Backscatter في EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/backscatter-messages-and-eop).</span><span class="sxs-lookup"><span data-stu-id="06dc1-106">Additional Information can be found in [Backscatter in EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/backscatter-messages-and-eop).</span></span>

<span data-ttu-id="06dc1-107">**تمكين الحماية من المكاتب Backscatter**</span><span class="sxs-lookup"><span data-stu-id="06dc1-107">**Enabling Backscatter protection**</span></span>

<span data-ttu-id="06dc1-108">لتمكين حماية Backscatter، اتبع المسار أدناه.</span><span class="sxs-lookup"><span data-stu-id="06dc1-108">To enable Backscatter protection, follow the path below.</span></span>

<span data-ttu-id="06dc1-109">**protection.office.com > إدارة المخاطر > نهج > مكافحةspam > حدد نهج تصفية البريد العشوائي ون نهج التحرير > خصائص البريد العشوائي > وضع علامة على البريد العشوائي > NDR backscatter > تعيينه إلى "On"**</span><span class="sxs-lookup"><span data-stu-id="06dc1-109">**protection.office.com > Threat Management > Policy > Antispam > Select the Spam Filter Policy and Edit policy > Spam properties > Mark as spam > NDR backscatter > Set it to “On”**</span></span>

<span data-ttu-id="06dc1-110">إذا كنت تعتقد أنه تم اختراق حساب، فشاهد ما يلي:</span><span class="sxs-lookup"><span data-stu-id="06dc1-110">If you believe an account has been compromised, see the following:</span></span>

- [<span data-ttu-id="06dc1-111">الاستجابة إلى حساب بريد إلكتروني م اختراق</span><span class="sxs-lookup"><span data-stu-id="06dc1-111">Responding to a Compromised Email Account</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account)
- [<span data-ttu-id="06dc1-112">إزالة المستخدمين المحظورين من مدخل المستخدمين المقيدين في Office 365</span><span class="sxs-lookup"><span data-stu-id="06dc1-112">Removing blocked users from the Restricted Users portal in Office 365</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/removing-user-from-restricted-users-portal-after-spam)



