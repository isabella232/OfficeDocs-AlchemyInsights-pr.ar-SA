---
title: DLP لا تعمل كما هو متوقع
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: 574a8a43d8264e98c6af2bfeb1bb472475e6e334
ms.sourcegitcommit: d108a2da2f5dab05246e30b5108cca5173e09051
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/26/2020
ms.locfileid: "42977425"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="fc8c9-102">DLP لا تعمل كما هو متوقع</span><span class="sxs-lookup"><span data-stu-id="fc8c9-102">DLP not working as expected</span></span>

<span data-ttu-id="fc8c9-103">**هام:** خلال هذه الأوقات غير المسبوقة، نتخذ خطوات لضمان أن تظل خدمات SharePoint Online و OneDrive متاحة للغاية - يرجى زيارة [SharePoint Online تعديلات الميزة المؤقتة](https://aka.ms/ODSPAdjustments) للحصول على مزيد من المعلومات.</span><span class="sxs-lookup"><span data-stu-id="fc8c9-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

 <span data-ttu-id="fc8c9-104">**إعداد DLP**</span><span class="sxs-lookup"><span data-stu-id="fc8c9-104">**Setting up DLP**</span></span>

<span data-ttu-id="fc8c9-105">هل تواجه مشاكل مع **منع فقدان البيانات (DLP)** في Office 365 لا يعمل كما هو متوقع؟</span><span class="sxs-lookup"><span data-stu-id="fc8c9-105">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="fc8c9-106">إذا كان الأمر كذلك، تأكد من إعداد **نهج DLP** بشكل صحيح، وأن بياناتك تحتوي على ما يبحث عنه **نهج DLP** عند تقييمه.</span><span class="sxs-lookup"><span data-stu-id="fc8c9-106">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="fc8c9-107">تسمح لك سياسات DLP بتحديد وحماية المعلومات الحساسة في مؤسستك.</span><span class="sxs-lookup"><span data-stu-id="fc8c9-107">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="fc8c9-108">لإعداد نُهج DLP، استخدم المعلومات [هنا](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span><span class="sxs-lookup"><span data-stu-id="fc8c9-108">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="fc8c9-109">**ما تبحث عنه سياسات DLP**</span><span class="sxs-lookup"><span data-stu-id="fc8c9-109">**What DLP policies look for**</span></span>
  
<span data-ttu-id="fc8c9-110">عند استخدام **أنواع المعلومات الحساسة المضمنة** في مركز الأمان والامتثال Office 365، تبحث نُهج DLP عن أنماط وعناصر محددة عند اكتشاف هذه الأنواع الحساسة.</span><span class="sxs-lookup"><span data-stu-id="fc8c9-110">When using the **built-in sensitive information types** in Office 365 Security and Compliance center, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="fc8c9-111">**أنواع المعلومات الحساسة المضمنة**</span><span class="sxs-lookup"><span data-stu-id="fc8c9-111">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="fc8c9-112">للحصول على معلومات حول الأنواع الحساسة المضمنة وما يبحث عنه نهج DLP عند الكشف عن النوع الحساس، راجع: [ما تبحث عنه أنواع المعلومات الحساسة](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span><span class="sxs-lookup"><span data-stu-id="fc8c9-112">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="fc8c9-113">**أنواع المعلومات الحساسة المخصصة**</span><span class="sxs-lookup"><span data-stu-id="fc8c9-113">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="fc8c9-114">إذا كنت تحاول إنشاء أنواع معلومات حساسة مخصصة، فاستخدم المقالة التالية للحصول على معلومات حول كيفية إنشاء نوع حساس مخصص: [إنشاء نوع معلومات حساسة مخصصة](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="fc8c9-114">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="fc8c9-115">**اختبار نهج DLP**</span><span class="sxs-lookup"><span data-stu-id="fc8c9-115">**Test a DLP policy**</span></span>

<span data-ttu-id="fc8c9-116">لاختبار البيانات باستخدام نوع معلومات حساسة مضمنة أو مخصصة، استخدم خيار **نوع الاختبار** ضمن أنواع**المعلومات الحساسة** **للتصنيفات** > .</span><span class="sxs-lookup"><span data-stu-id="fc8c9-116">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="fc8c9-117">لمزيد من المعلومات، راجع [اختبار أنواع المعلومات الحساسة المخصصة](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span><span class="sxs-lookup"><span data-stu-id="fc8c9-117">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="fc8c9-118">**التقارير**</span><span class="sxs-lookup"><span data-stu-id="fc8c9-118">**Reports**</span></span>
  
- <span data-ttu-id="fc8c9-119">احصل على رؤى بيانات حساسة باستخدام [تقارير DLP.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="fc8c9-119">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="fc8c9-120">راجع تفاصيل محددة للحدث مع [تقرير الحادث](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span><span class="sxs-lookup"><span data-stu-id="fc8c9-120">See specific details of the event with an [Incident Report](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span></span>
