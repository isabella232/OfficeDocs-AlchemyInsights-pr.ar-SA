---
title: التحضير لاستخدام أمان طبقة النقل TLS 1.2 في Microsoft 365
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Critical
ms.custom:
- "1266"
- "1600052"
ms.assetid: d5c84f5c-a3ca-4abd-8633-7e9ff01328a9
ms.openlocfilehash: 1ec40ba36c69296298e24dca64a873d53682833a
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 11/17/2020
ms.locfileid: "49085891"
---
# <a name="prepare-for-use-of-tls-12-in-microsoft-365"></a><span data-ttu-id="74e67-102">التحضير لاستخدام أمان طبقة النقل TLS 1.2 في Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="74e67-102">Prepare for use of TLS 1.2 in Microsoft 365</span></span>

<span data-ttu-id="74e67-103">اعتباراً من 31 أكتوبر 2018، سيستمر Microsoft 365 في الانتقال إلى TLS 1.2.</span><span class="sxs-lookup"><span data-stu-id="74e67-103">As of October 31st, 2018, Microsoft 365 will continue transitioning to TLS 1.2.</span></span> <span data-ttu-id="74e67-104">بدءا من 15 أكتوبر 2020، سيبدأ O365 في إهمال TLS 1.0 و1.1 عبر الخدمة.</span><span class="sxs-lookup"><span data-stu-id="74e67-104">Starting October 15, 2020, O365 will begin the deprecation of TLS 1.0 and 1.1 across the service.</span></span> <span data-ttu-id="74e67-105">سيستمر طرح هذا التغيير على مدار الأسابيع والأشهر القليلة القادمة، ولكن يجب على العملاء افتراض عدم عمل مكالمات TLS 1.0/1.1 عند استخدام O365 بدءا من 15 أكتوبر 2020.</span><span class="sxs-lookup"><span data-stu-id="74e67-105">The rollout of this change will continue over the next few weeks and months, but customers should assume no TLS 1.0/1.1 calls will work when engaging with O365 starting Oct 15, 2020.</span></span> <span data-ttu-id="74e67-106">كما تم الاتصال مسبقا (MC126199 في ديسمبر 2017، إن MC128929 في فبراير 2018 و MC186827 في يوليو 2019 و MC218794 في يوليو 2020)، نقوم بنقل كل خدماتنا عبر الإنترنت إلى 1.2+ أمان طبقة النقل لتوفير التشفير الأفضل في الفئة وضمان أن تكون خدمتنا أكثر أمانا بشكل افتراضي.</span><span class="sxs-lookup"><span data-stu-id="74e67-106">As previously communicated (MC126199 in Dec 2017, MC128929 in Feb 2018, MC186827 in July 2019, and MC218794 in July 2020), we are moving all of our online services to Transport Layer Security (TLS) 1.2+ to provide best-in-class encryption, and to ensure our service is more secure, by default.</span></span> <span data-ttu-id="74e67-107">لا يزال يمكن للعملاء اختيار الحصول على TLS 1.0/1.1 على خوادمهم ومواردهم، ولكن يجب أن يفترضوا أن TLS 1.2 أو أعلى فقط ستعمل عند التفاعل مع موارد O365.</span><span class="sxs-lookup"><span data-stu-id="74e67-107">Customers can still choose to have TLS 1.0/1.1 on their servers and resources, but they should assume only TLS 1.2 or higher will work when interacting with O365 resources.</span></span>
  
<span data-ttu-id="74e67-108">لمعرفة المزيد حول هذه التغييرات، الرجاء الاطلاع [على هنا](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365?view=o365-worldwide) [وهنا](https://docs.microsoft.com/microsoft-365/compliance/tls-1.0-and-1.1-deprecation-for-office-365?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="74e67-108">To learn more about these changes, please see [here](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365?view=o365-worldwide) and [here](https://docs.microsoft.com/microsoft-365/compliance/tls-1.0-and-1.1-deprecation-for-office-365?view=o365-worldwide).</span></span>

  