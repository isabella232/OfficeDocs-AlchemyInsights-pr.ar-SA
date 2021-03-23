---
title: استكشاف أخطاء رموز الخطأ مصادقة Azure AD وتخويلها (AADSTS) وإصلاحها
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9800"
- "9005744"
ms.openlocfilehash: 14555dfcb1406fd3a3977012393714a713ff80dc
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/19/2021
ms.locfileid: "51034845"
---
# <a name="troubleshoot-azure-ad-authentication-and-authorization-aadsts-error-codes"></a><span data-ttu-id="d2b87-102">استكشاف أخطاء رموز الخطأ مصادقة Azure AD وتخويلها (AADSTS) وإصلاحها</span><span class="sxs-lookup"><span data-stu-id="d2b87-102">Troubleshoot Azure AD Authentication and Authorization (AADSTS) error codes</span></span>

<span data-ttu-id="d2b87-103">لحل رموز أخطاء مصادقة AAD وتخويلها (AADSTS)، يجب تنفيذ الخطوات التالية الموصى بها:</span><span class="sxs-lookup"><span data-stu-id="d2b87-103">To resolve AAD authentication and authorization error codes (AADSTS), perform the following recommended steps:</span></span>

1. <span data-ttu-id="d2b87-104">**معالجة رموز الخطأ في التطبيق**</span><span class="sxs-lookup"><span data-stu-id="d2b87-104">**Handling error codes in your application**</span></span>

- <span data-ttu-id="d2b87-105">يوفر **المواصفات OAuth2.0**، إرشادات حول كيفية معالجة الأخطاء أثناء المصادقة باستخدام جزء الخطأ https://tools.ietf.org/html/rfc6749#section-5.2 من استجابة الخطأ.</span><span class="sxs-lookup"><span data-stu-id="d2b87-105">The **OAuth2.0 spec**, https://tools.ietf.org/html/rfc6749#section-5.2, provides guidance on how to handle errors during authentication using the error portion of the error response.</span></span>

    - <span data-ttu-id="d2b87-106">**:** سلسلة رمز خطأ يمكن استخدامها لتصنيف أنواع الأخطاء التي تحدث، ويجب استخدامها للتفاعل مع الأخطاء.</span><span class="sxs-lookup"><span data-stu-id="d2b87-106">**error**: An error code string that can be used to classify types of errors that occur, and should be used to react to errors.</span></span>
    - <span data-ttu-id="d2b87-107">حقل **الخطأ** له عدة قيم محتملة - راجع ارتباطات وثائق البروتوكول والمواصفات OAuth 2.0 للحصول على مزيد من المعلومات حول أخطاء معينة وكيفية التفاعل معها.</span><span class="sxs-lookup"><span data-stu-id="d2b87-107">The **error** field has several possible values - review the protocol documentation links and OAuth 2.0 specs for more information about specific errors and how to react to them.</span></span>

- <span data-ttu-id="d2b87-108">فيما يلي استجابة نموذجية للخطأ:</span><span class="sxs-lookup"><span data-stu-id="d2b87-108">Here is a sample error response:</span></span>
```
{
  "error": "invalid_scope",
  "error_description": "AADSTS70011: The provided value for the input parameter 'scope' is not 
valid. The scope https://example.contoso.com/activity.read is not valid.\r\nTrace ID: 255d1aef- 8c98-452f-ac51-23d051240864\r\nCorrelation ID: fb3d2015-bc17-4bb9-bb85-30c5cf1aaaa7\r\nTimestamp: 2016-01-09 02:02:12Z",
  "error_codes": [
    70011
  ],
  "timestamp": "2016-01-09 02:02:12Z",
  "trace_id": "255d1aef-8c98-452f-ac51-23d051240864",
  "correlation_id": "fb3d2015-bc17-4bb9-bb85-30c5cf1aaaa7", 
  "error_uri":"https://login.microsoftonline.com/error?code=70011"
}
```
2. <span data-ttu-id="d2b87-109">**البحث عن معلومات رمز الخطأ الحالي**</span><span class="sxs-lookup"><span data-stu-id="d2b87-109">**Lookup current error code information**</span></span>

- <span data-ttu-id="d2b87-110">رموز الأخطاء والرسائل عرضة للتغيير.</span><span class="sxs-lookup"><span data-stu-id="d2b87-110">Error codes and messages are subject to change.</span></span> <span data-ttu-id="d2b87-111">للحصول على أحدث المعلومات، راجع الصفحة للعثور على أوصاف أخطاء AADSTS وإصلاحاتها وبعض الحلول https://login.microsoftonline.com/error المقترحة.</span><span class="sxs-lookup"><span data-stu-id="d2b87-111">For the most current information, see the https://login.microsoftonline.com/error page to find AADSTS error descriptions, fixes, and some suggested workarounds.</span></span>
- <span data-ttu-id="d2b87-112">يمكنك أيضا البحث عن رموز أخطاء [AADSTS](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#aadsts-error-codes) المدرجة في المقالة مصادقة Azure AD ورموز خطأ [التخويل وإصلاحها.](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#handling-error-codes-in-your-application)</span><span class="sxs-lookup"><span data-stu-id="d2b87-112">You can also search for and troubleshoot [AADSTS error codes](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#aadsts-error-codes) listed in the article [Azure AD Authentication and authorization error codes](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#handling-error-codes-in-your-application).</span></span>

3. <span data-ttu-id="d2b87-113">**الحصول على تعليمات**</span><span class="sxs-lookup"><span data-stu-id="d2b87-113">**Get Help**</span></span>

- <span data-ttu-id="d2b87-114">[خيارات الدعم والدعم](https://docs.microsoft.com/azure/active-directory/develop/developer-support-help-options) للمطورين - إذا كنت بحاجة إلى إجابة عن سؤال أو مساعدة لحل مشكلة غير مشمولة في وثائقنا، فقد يكون الوقت قد حان للوصول إلى الخبراء للحصول على المساعدة.</span><span class="sxs-lookup"><span data-stu-id="d2b87-114">[Support and help options for developers](https://docs.microsoft.com/azure/active-directory/develop/developer-support-help-options) - If you need an answer to a question or help in solving a problem not covered in our documentation, it might be time to reach out to experts for help.</span></span> <span data-ttu-id="d2b87-115">توفر هذه المقالة العديد من الاقتراحات للحصول على إجابات لأسئلتك عند تطوير التطبيقات التي تتكامل مع النظام الأساسي لهوية Microsoft.</span><span class="sxs-lookup"><span data-stu-id="d2b87-115">This article provides several suggestions for getting answers to your questions as you develop apps that integrate with the Microsoft identity platform.</span></span>








