---
title: DLP لا تعمل كما هو متوقع
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: efb4a19f345fe6b8a1e8bb72abeba4a923c05777
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704400"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="42b0b-102">DLP لا تعمل كما هو متوقع</span><span class="sxs-lookup"><span data-stu-id="42b0b-102">DLP not working as expected</span></span>

<span data-ttu-id="42b0b-103">**هام**: خلال هذه الأوقات غير المسبوقة، نقوم باتخاذ الخطوات اللازمة لضمان توفر خدمات SharePoint Online و OneDrive بشكل كبير – الرجاء زيارة [تعديلات الميزات المؤقتة لـ SharePoint Online](https://aka.ms/ODSPAdjustments) للحصول على مزيد من المعلومات.</span><span class="sxs-lookup"><span data-stu-id="42b0b-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

 <span data-ttu-id="42b0b-104">**إعداد DLP**</span><span class="sxs-lookup"><span data-stu-id="42b0b-104">**Setting up DLP**</span></span>

<span data-ttu-id="42b0b-105">هل تواجه مشاكل مع **منع فقدان البيانات (DLP)** في Office 365 لا يعمل كما هو متوقع؟</span><span class="sxs-lookup"><span data-stu-id="42b0b-105">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="42b0b-106">إذا كان الأمر كذلك، تأكد من إعداد **نهج DLP** بشكل صحيح، وأن بياناتك تحتوي على ما يبحث عنه **نهج DLP** عند تقييمه.</span><span class="sxs-lookup"><span data-stu-id="42b0b-106">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="42b0b-107">تسمح لك سياسات DLP بتحديد وحماية المعلومات الحساسة في مؤسستك.</span><span class="sxs-lookup"><span data-stu-id="42b0b-107">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="42b0b-108">لإعداد نُهج DLP، استخدم المعلومات [هنا](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span><span class="sxs-lookup"><span data-stu-id="42b0b-108">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="42b0b-109">**ما تبحث عنه سياسات DLP**</span><span class="sxs-lookup"><span data-stu-id="42b0b-109">**What DLP policies look for**</span></span>
  
<span data-ttu-id="42b0b-110">عند استخدام **أنواع المعلومات الحساسة المضمنة** في مراكز الأمان والامتثال، تبحث نُهج DLP عن أنماط وعناصر محددة عند اكتشاف هذه الأنواع الحساسة.</span><span class="sxs-lookup"><span data-stu-id="42b0b-110">When using the **built-in sensitive information types** in the Security and Compliance centers, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="42b0b-111">**أنواع المعلومات الحساسة المضمنة**</span><span class="sxs-lookup"><span data-stu-id="42b0b-111">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="42b0b-112">للحصول على معلومات حول الأنواع الحساسة المضمنة وما يبحث عنه نهج DLP عند الكشف عن النوع الحساس، راجع: [ما تبحث عنه أنواع المعلومات الحساسة](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span><span class="sxs-lookup"><span data-stu-id="42b0b-112">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="42b0b-113">**أنواع المعلومات الحساسة المخصصة**</span><span class="sxs-lookup"><span data-stu-id="42b0b-113">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="42b0b-114">إذا كنت تحاول إنشاء أنواع معلومات حساسة مخصصة، فاستخدم المقالة التالية للحصول على معلومات حول كيفية إنشاء نوع حساس مخصص: [إنشاء نوع معلومات حساسة مخصصة](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="42b0b-114">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="42b0b-115">**اختبار نهج DLP**</span><span class="sxs-lookup"><span data-stu-id="42b0b-115">**Test a DLP policy**</span></span>

<span data-ttu-id="42b0b-116">لاختبار البيانات باستخدام نوع معلومات حساسة مضمنة أو مخصصة، استخدم خيار **نوع الاختبار** ضمن أنواع**المعلومات الحساسة** **للتصنيفات** > .</span><span class="sxs-lookup"><span data-stu-id="42b0b-116">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="42b0b-117">لمزيد من المعلومات، راجع [اختبار أنواع المعلومات الحساسة المخصصة](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span><span class="sxs-lookup"><span data-stu-id="42b0b-117">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="42b0b-118">**التقارير**</span><span class="sxs-lookup"><span data-stu-id="42b0b-118">**Reports**</span></span>
  
- <span data-ttu-id="42b0b-119">احصل على رؤى بيانات حساسة باستخدام [تقارير DLP.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="42b0b-119">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="42b0b-120">راجع تفاصيل محددة للحدث مع [تقرير الحادث](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span><span class="sxs-lookup"><span data-stu-id="42b0b-120">See specific details of the event with an [Incident Report](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span></span>
