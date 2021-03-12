---
title: لا تعمل DLP كما هو متوقع
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: 0f07e64c95675a4f6a0aeb6df110fe4e6a21d72f
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707797"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="c66c6-102">لا تعمل DLP كما هو متوقع</span><span class="sxs-lookup"><span data-stu-id="c66c6-102">DLP not working as expected</span></span>

<span data-ttu-id="c66c6-103">**هام**: خلال هذه الأوقات غير المسبوقة، نقوم باتخاذ الخطوات اللازمة لضمان توفر خدمات SharePoint Online و OneDrive بشكل كبير – الرجاء زيارة [تعديلات الميزات المؤقتة لـ SharePoint Online](https://aka.ms/ODSPAdjustments) للحصول على مزيد من المعلومات.</span><span class="sxs-lookup"><span data-stu-id="c66c6-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

 <span data-ttu-id="c66c6-104">**إعداد DLP**</span><span class="sxs-lookup"><span data-stu-id="c66c6-104">**Setting up DLP**</span></span>

<span data-ttu-id="c66c6-105">هل تواجه مشاكل في منع فقدان **البيانات (DLP)** في Office 365 لا يعمل كما هو متوقع؟</span><span class="sxs-lookup"><span data-stu-id="c66c6-105">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="c66c6-106">إذا كان الأمر كذلك، فتأكد من إعداد نهج **DLP** بشكل صحيح، ومن احتواء بياناتك على ما يبحث عنه نهج **DLP** عند تقييمه.</span><span class="sxs-lookup"><span data-stu-id="c66c6-106">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="c66c6-107">تسمح لك سياسات DLP بتحديد المعلومات الحساسة في مؤسستك وحمايتها.</span><span class="sxs-lookup"><span data-stu-id="c66c6-107">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="c66c6-108">لإعداد سياسات DLP، استخدم المعلومات [هنا.](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template)</span><span class="sxs-lookup"><span data-stu-id="c66c6-108">To setup DLP policies, use the information [here](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template).</span></span>
  
 <span data-ttu-id="c66c6-109">**ما تبحث عنه سياسات DLP**</span><span class="sxs-lookup"><span data-stu-id="c66c6-109">**What DLP policies look for**</span></span>
  
<span data-ttu-id="c66c6-110">عند استخدام أنواع **المعلومات** الحساسة المضمنة في مراكز الأمان والتوافق، تبحث سياسات DLP عن أنماط وعناصر معينة عند الكشف عن هذه الأنواع الحساسة.</span><span class="sxs-lookup"><span data-stu-id="c66c6-110">When using the **built-in sensitive information types** in the Security and Compliance centers, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="c66c6-111">**أنواع المعلومات الحساسة المضمنة**</span><span class="sxs-lookup"><span data-stu-id="c66c6-111">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="c66c6-112">للحصول على معلومات حول الأنواع الحساسة المضمنة وما الذي تبحث عنه سياسة DLP عند الكشف عن النوع الحساس، راجع: ما تبحث عنه أنواع المعلومات [الحساسة.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="c66c6-112">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>

- <span data-ttu-id="c66c6-113">**أنواع المعلومات الحساسة المخصصة**</span><span class="sxs-lookup"><span data-stu-id="c66c6-113">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="c66c6-114">إذا كنت تحاول إنشاء أنواع معلومات مخصصة حساسة، فاستخدم المقالة التالية للحصول على معلومات حول كيفية إنشاء نوع معلومات مخصص حساس: إنشاء نوع معلومات مخصص [حساس.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type)</span><span class="sxs-lookup"><span data-stu-id="c66c6-114">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="c66c6-115">**اختبار نهج DLP**</span><span class="sxs-lookup"><span data-stu-id="c66c6-115">**Test a DLP policy**</span></span>

<span data-ttu-id="c66c6-116">لاختبار البيانات باستخدام نوع معلومات مضمن أو مخصص  حساس، استخدم الخيار "نوع الاختبار" ضمن أنواع المعلومات الحساسة  >  **للتصنيفات.**</span><span class="sxs-lookup"><span data-stu-id="c66c6-116">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="c66c6-117">لمزيد من المعلومات، راجع [اختبار أنواع المعلومات الحساسة المخصصة.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center)</span><span class="sxs-lookup"><span data-stu-id="c66c6-117">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="c66c6-118">**التقارير**</span><span class="sxs-lookup"><span data-stu-id="c66c6-118">**Reports**</span></span>
  
- <span data-ttu-id="c66c6-119">احصل على تحليلات البيانات الحساسة باستخدام [تقارير DLP.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="c66c6-119">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="c66c6-120">راجع تفاصيل معينة للحدث باستخدام تقرير [حادث.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports)</span><span class="sxs-lookup"><span data-stu-id="c66c6-120">See specific details of the event with an [Incident Report](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).</span></span>
