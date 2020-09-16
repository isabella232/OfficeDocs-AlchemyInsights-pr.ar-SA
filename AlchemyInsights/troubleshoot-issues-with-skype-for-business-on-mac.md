---
title: استكشاف الأخطاء وإصلاحها في Skype for Business علي جهاز Mac
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/30/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5984"
- "9003195"
ms.openlocfilehash: 794ec70971fc2eff31047f8346284118eb9d6add
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47665021"
---
# <a name="troubleshoot-issues-with-skype-for-business-on-mac"></a><span data-ttu-id="76f1f-102">استكشاف الأخطاء وإصلاحها في Skype for Business علي جهاز Mac</span><span class="sxs-lookup"><span data-stu-id="76f1f-102">Troubleshoot issues with Skype for Business on Mac</span></span>

<span data-ttu-id="76f1f-103">لمزيد من المعلومات، اطلع على:</span><span class="sxs-lookup"><span data-stu-id="76f1f-103">For more information, see:</span></span> 

- <span data-ttu-id="76f1f-104">قد لا تكون بعض الميزات ، مثل وظائف مجموعه الاستجابة أو الدردشة الثابتة متوفرة أو معتمده علي النظام الأساسي ل Mac.</span><span class="sxs-lookup"><span data-stu-id="76f1f-104">Some features, such as Response Group functionality or Persistent Chat, might not be available or supported on the Mac platform.</span></span> <span data-ttu-id="76f1f-105">تاكد من ان الوظيفة معتمده علي النظام الأساسي الخاص ب Mac.</span><span class="sxs-lookup"><span data-stu-id="76f1f-105">Verify that the functionality is supported on the Mac platform.</span></span> <span data-ttu-id="76f1f-106">بالنسبة إلى توفر الميزات لنظام التشغيل Mac ، راجع [مقارنه ميزات عميل الجوال لمقارنه](https://technet.microsoft.com/library/Dn951412.aspx) [ميزات عميل سطح المكتب](https://docs.microsoft.com/skypeforbusiness/plan-your-deployment/clients-and-devices/desktop-feature-comparison)ل skype for business و skype for business.</span><span class="sxs-lookup"><span data-stu-id="76f1f-106">For Mac feature availability, see [Mobile client feature comparison for Skype for Business](https://technet.microsoft.com/library/Dn951412.aspx) and [Desktop client feature comparison for Skype for Business](https://docs.microsoft.com/skypeforbusiness/plan-your-deployment/clients-and-devices/desktop-feature-comparison).</span></span>
- <span data-ttu-id="76f1f-107">إذا كنت تواجه مشكله في تسجيل الدخول علي تطبيق Skype for Business Mac ، فتاكد من ان طبولوجيا المصادقة الخاصة بك معتمده.</span><span class="sxs-lookup"><span data-stu-id="76f1f-107">If you are experiencing a sign-in issue on the Skype for Business Mac app, make sure that your authentication topology is supported.</span></span> <span data-ttu-id="76f1f-108">للحصول علي معلومات مفصله حول الأسلوب المعتمد ، راجع [طبولوجيا Skype For business المعتمدة بواسطة المصادقة الحديثة](https://docs.microsoft.com/skypeforbusiness/plan-your-deployment/modern-authentication/topologies-supported).</span><span class="sxs-lookup"><span data-stu-id="76f1f-108">For detailed information about the supported method, see [Skype for Business topologies supported with Modern Authentication](https://docs.microsoft.com/skypeforbusiness/plan-your-deployment/modern-authentication/topologies-supported).</span></span>  
- <span data-ttu-id="76f1f-109">إذا لم ترد هذه المعلومات علي أسئلتك ، فافتح تذكره دعم.</span><span class="sxs-lookup"><span data-stu-id="76f1f-109">If this information doesn't answer your questions, open a Support ticket.</span></span> <span data-ttu-id="76f1f-110">جمع أكبر قدر ممكن من المعلومات قبل فتح البطاقة.</span><span class="sxs-lookup"><span data-stu-id="76f1f-110">Collect as much information as possible prior to opening the ticket.</span></span> <span data-ttu-id="76f1f-111">علي سبيل المثال ، قم بتجميع كل السجلات ورسائل الأخطاء.</span><span class="sxs-lookup"><span data-stu-id="76f1f-111">For example, collect all logs and errors messages.</span></span> <span data-ttu-id="76f1f-112">لتجميع السجلات علي جهاز Mac ، انتقل إلى تفضيلات  **تطبيق سفب**  >  **Preferences**  >  **الجمع**.</span><span class="sxs-lookup"><span data-stu-id="76f1f-112">To collect logs on the Mac, go to  **SfB App** > **Preferences** > **Collect logs**.</span></span>  <span data-ttu-id="76f1f-113">يجب ان يتضمن السجل المزيد من التفاصيل قدر الإمكان من تسجيل الدخول إلى نقطه الفشل.</span><span class="sxs-lookup"><span data-stu-id="76f1f-113">The log should include as much detail as possible from sign-in to the point of failure.</span></span>