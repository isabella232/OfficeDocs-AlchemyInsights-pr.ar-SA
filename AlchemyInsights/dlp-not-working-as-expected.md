---
title: لا يعمل DLP كما هو متوقع
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
ms.openlocfilehash: 0ed893420b5813d5d18639c2c226c12f0306a13f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679680"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="f834e-102">لا يعمل DLP كما هو متوقع</span><span class="sxs-lookup"><span data-stu-id="f834e-102">DLP not working as expected</span></span>

<span data-ttu-id="f834e-103">**هام**: خلال هذه الأوقات غير المسبوقة، نقوم باتخاذ الخطوات اللازمة لضمان توفر خدمات SharePoint Online و OneDrive بشكل كبير – الرجاء زيارة [تعديلات الميزات المؤقتة لـ SharePoint Online](https://aka.ms/ODSPAdjustments) للحصول على مزيد من المعلومات.</span><span class="sxs-lookup"><span data-stu-id="f834e-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

 <span data-ttu-id="f834e-104">**اعداد DLP**</span><span class="sxs-lookup"><span data-stu-id="f834e-104">**Setting up DLP**</span></span>

<span data-ttu-id="f834e-105">هل تواجه مشاكل في **منع فقدان البيانات (DLP)** في Office 365 لا تعمل كما هو متوقع ؟</span><span class="sxs-lookup"><span data-stu-id="f834e-105">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="f834e-106">إذا كان الأمر كذلك ، فتاكد من اعداد **نهج dlp** بشكل صحيح ، ومن ان البيانات تحتوي علي ما تبحث عنه **نهج DLP** عند تقييمه.</span><span class="sxs-lookup"><span data-stu-id="f834e-106">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="f834e-107">تسمح لك نهج DLP بتعريف المعلومات الحساسة وحمايتها في مؤسستك.</span><span class="sxs-lookup"><span data-stu-id="f834e-107">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="f834e-108">لاعداد نهج DLP ، استخدم المعلومات الموجودة [هنا](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span><span class="sxs-lookup"><span data-stu-id="f834e-108">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="f834e-109">**ما هي نهج DLP التي تبحث عنها**</span><span class="sxs-lookup"><span data-stu-id="f834e-109">**What DLP policies look for**</span></span>
  
<span data-ttu-id="f834e-110">عند استخدام **أنواع المعلومات الحساسة المضمنة** في مراكز الأمان والتوافق ، تبحث نهج DLP عن أنماط وعناصر معينه عند اكتشاف هذه الأنواع الحساسة.</span><span class="sxs-lookup"><span data-stu-id="f834e-110">When using the **built-in sensitive information types** in the Security and Compliance centers, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="f834e-111">**أنواع المعلومات الحساسة المضمنة**</span><span class="sxs-lookup"><span data-stu-id="f834e-111">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="f834e-112">للحصول علي معلومات حول الأنواع الحساسة المضمنة وما يبحث عنه نهج DLP عند اكتشاف النوع الحساس ، راجع: [ما الذي تبحث عنه أنواع المعلومات الهامه](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span><span class="sxs-lookup"><span data-stu-id="f834e-112">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>

- <span data-ttu-id="f834e-113">**أنواع المعلومات الحساسة المخصصة**</span><span class="sxs-lookup"><span data-stu-id="f834e-113">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="f834e-114">إذا كنت تحاول إنشاء أنواع معلومات حساسة مخصصه ، فاستخدم المقالة التالية للحصول علي معلومات حول كيفيه إنشاء نوع حساس مخصص: [إنشاء نوع معلومات حساسة مخصصه](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="f834e-114">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="f834e-115">**اختبار نهج DLP**</span><span class="sxs-lookup"><span data-stu-id="f834e-115">**Test a DLP policy**</span></span>

<span data-ttu-id="f834e-116">لاختبار البيانات باستخدام نوع معلومات حساس أو مخصص مضمن ، استخدم الخيار **نوع الاختبار** ضمن **تصنيف**  >  **أنواع المعلومات الحساسة**.</span><span class="sxs-lookup"><span data-stu-id="f834e-116">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="f834e-117">لمزيد من المعلومات ، راجع [اختبار أنواع المعلومات الحساسة المخصصة](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).</span><span class="sxs-lookup"><span data-stu-id="f834e-117">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="f834e-118">**يراس**</span><span class="sxs-lookup"><span data-stu-id="f834e-118">**Reports**</span></span>
  
- <span data-ttu-id="f834e-119">احصل علي معارف دقيقه للبيانات باستخدام [تقارير DLP.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="f834e-119">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="f834e-120">راجع تفاصيل الحدث باستخدام [تقرير الحادث](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).</span><span class="sxs-lookup"><span data-stu-id="f834e-120">See specific details of the event with an [Incident Report](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).</span></span>
