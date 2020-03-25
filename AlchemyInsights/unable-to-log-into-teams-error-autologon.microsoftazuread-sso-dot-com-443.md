---
title: لا يمكن تسجيل الدخول إلى Teams بسبب الخطأ autologon.microsoftazuread-sso.com:443
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "9001686"
- "3750"
ms.openlocfilehash: 77049153939989d1c63789adfec0b494d047a6e4
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931766"
---
# <a name="unable-to-log-into-teams-due-to-error-autologonmicrosoftazuread-sso-dot-com443"></a><span data-ttu-id="41354-102">لا يمكن تسجيل الدخول إلى Teams بسبب الخطأ autologon.microsoftazuread-sso dot com:443</span><span class="sxs-lookup"><span data-stu-id="41354-102">Unable to log into Teams due to error autologon.microsoftazuread-sso dot com:443</span></span>

<span data-ttu-id="41354-103">إذا تم تمكين SSO كمصادقة لـ O365، فقد تحتاج إلى إضافة عنوان URL "autologon.microsoftazuread-sso.com" إلى مواقع الإنترانت.</span><span class="sxs-lookup"><span data-stu-id="41354-103">If Seamless SSO is enabled as the O365 authentication, the URL "autologon.microsoftazuread-sso.com" may need to be added to Intranet Sites.</span></span>  <span data-ttu-id="41354-104">إذا تمت إضافته إلى "المواقع الموثوق بها" مسبقاً وكان SSO قيد الاستخدام، فيجب إزالته من "المواقع الموثوق بها".</span><span class="sxs-lookup"><span data-stu-id="41354-104">If it has previously been added to Trusted Sites  and Seamless SSO is in use, it should be removed from Trusted Sites.</span></span>

<span data-ttu-id="41354-105">الرجاء مراجعة["قائمة اختيار استكشاف أخطاء SSO وإصلاحها"](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist).</span><span class="sxs-lookup"><span data-stu-id="41354-105">Please review the [Seamless SSO Troubleshooting Checklist](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist).</span></span>

<span data-ttu-id="41354-106">اتبع هذه الخطوات لإضافة عنوان URL إلى قائمة مواقع الإنترانت:</span><span class="sxs-lookup"><span data-stu-id="41354-106">Follow these steps to add a URL to Intranet Sites list:</span></span>

1. <span data-ttu-id="41354-107">افتح Internet Explorer بالنقر فوق الزر **"بدء"**.</span><span class="sxs-lookup"><span data-stu-id="41354-107">Open Internet Explorer by clicking the **Start** button.</span></span> <span data-ttu-id="41354-108">في مربع البحث اكتب Internet Explorer، ثم انقر فوق **Internet Explorer**في قائمة النتائج.</span><span class="sxs-lookup"><span data-stu-id="41354-108">In the search box, type Internet Explorer, and then, in the list of results, click **Internet Explorer**.</span></span>
2. <span data-ttu-id="41354-109">انقر فوق قائمة **أدوات** ثم انقر فوق **خيارات الإنترنت**.</span><span class="sxs-lookup"><span data-stu-id="41354-109">Click **Tools**, and then click **Internet options**.</span></span>
3. <span data-ttu-id="41354-110">انقر فوق علامة التبويب **أمان**.</span><span class="sxs-lookup"><span data-stu-id="41354-110">Click the **Security** tab.</span></span>
4. <span data-ttu-id="41354-111">انقر الآن فوق **مواقع إنترانت المحلية** ثم انقر فوق الزر **المواقع** ثم فوق الزر **متقدم**.</span><span class="sxs-lookup"><span data-stu-id="41354-111">Now click on **Local Intranet sites** and then click on the **sites** button and then **Advanced** button.</span></span>
5. <span data-ttu-id="41354-112">ادخل عنوان URL لموقع الويب ثم انقر فوق **"إضافة"**.</span><span class="sxs-lookup"><span data-stu-id="41354-112">Enter the Website URL and click **Add**.</span></span>
6. <span data-ttu-id="41354-113">عند الانتهاء، انقر فوق **إغلاق**.</span><span class="sxs-lookup"><span data-stu-id="41354-113">When you are finished, click **Close**.</span></span>

<span data-ttu-id="41354-114">للحصول على مزيد من المعلومات، راجع [وثائق لنشر SSO لـ O365](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start) (يتضمن العملية المستندة إلى النهج لإضافة عنوان URL إلى مواقع إنترانت في الخطوة 3).</span><span class="sxs-lookup"><span data-stu-id="41354-114">For more information, see [Documentation for deploying Seamless SSO for O365](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start) (includes Policy-based process to add a URL to Intranet Sites in Step 3).</span></span>
