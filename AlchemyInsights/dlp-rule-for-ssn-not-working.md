---
title: قاعدة DLP لـ SSN لا تعمل
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: 0b83a858975ffe1bb70f16a7452a13d57dff5340
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932502"
---
# <a name="dlp-issues-with-social-security-numbers"></a><span data-ttu-id="4cf5e-102">DLP القضايا مع أرقام الضمان الاجتماعي</span><span class="sxs-lookup"><span data-stu-id="4cf5e-102">DLP issues with Social Security Numbers</span></span>

<span data-ttu-id="4cf5e-103">**هام:** يعمل العديد من عملاء SharePoint Online و OneDrive على تشغيل تطبيقات مهمة للأعمال مقابل الخدمة التي تعمل في الخلفية.</span><span class="sxs-lookup"><span data-stu-id="4cf5e-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="4cf5e-104">وتشمل هذه ترحيل المحتوى، منع فقدان البيانات (DLP)، وحلول النسخ الاحتياطي.</span><span class="sxs-lookup"><span data-stu-id="4cf5e-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="4cf5e-105">خلال هذه الأوقات غير المسبوقة، نتخذ خطوات لضمان أن تظل خدمات SharePoint Online و OneDrive متاحة للغاية وموثوقة للمستخدمين الذين يعتمدون على الخدمة أكثر من أي وقت مضى في سيناريوهات العمل عن بعد.</span><span class="sxs-lookup"><span data-stu-id="4cf5e-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="4cf5e-106">ولدعم هذا الهدف، قمنا بتنفيذ قيود خنق أكثر صرامة على تطبيقات الخلفية (الترحيل وDLP وحلول النسخ الاحتياطي) خلال ساعات النهار في أيام الأسبوع.</span><span class="sxs-lookup"><span data-stu-id="4cf5e-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="4cf5e-107">يجب أن تتوقع أن تحقق هذه التطبيقات إنتاجية محدودة جدًا خلال هذه الأوقات.</span><span class="sxs-lookup"><span data-stu-id="4cf5e-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="4cf5e-108">ومع ذلك ، خلال ساعات المساء وعطلة نهاية الأسبوع للمنطقة ، ستكون الخدمة جاهزة لمعالجة حجم أكبر بكثير من الطلبات من تطبيقات الخلفية.</span><span class="sxs-lookup"><span data-stu-id="4cf5e-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="4cf5e-109">**مشكلات DLP مع SSNs**</span><span class="sxs-lookup"><span data-stu-id="4cf5e-109">**DLP issues with SSNs**</span></span>

<span data-ttu-id="4cf5e-110">هل تواجه مشاكل مع **منع فقدان البيانات (DLP)** لا تعمل للمحتوى الذي يحتوي على **رقم الضمان الاجتماعي (SSN)** عند استخدام نوع معلومات حساسة في Office 365؟</span><span class="sxs-lookup"><span data-stu-id="4cf5e-110">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Social Security Number (SSN)** when using a sensitive information type in Office 365?</span></span> <span data-ttu-id="4cf5e-111">إذا كان الأمر كذلك، تأكد من أن المحتوى الخاص بك يحتوي على المعلومات المطلوبة لما تبحث عنه سياسة DLP.</span><span class="sxs-lookup"><span data-stu-id="4cf5e-111">If so, make sure your content contains the needed information for what the DLP policy is looking.</span></span> 
  
<span data-ttu-id="4cf5e-112">على سبيل المثال، بالنسبة لسياسة SSN التي تم تكوينها بمستوى ثقة 85%، يتم تقييم ما يلي ويجب الكشف عنها حتى تقوم القاعدة بتشغيلها:</span><span class="sxs-lookup"><span data-stu-id="4cf5e-112">For example, for an SSN policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="4cf5e-113">**[التنسيق:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 أرقام، والتي قد تكون في نمط منسق أو غير منسق</span><span class="sxs-lookup"><span data-stu-id="4cf5e-113">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 digits, which may be in a formatted or unformatted pattern</span></span>

- <span data-ttu-id="4cf5e-114">**[نمط:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** أربع وظائف تبحث عن SSNs في أربعة أنماط مختلفة:</span><span class="sxs-lookup"><span data-stu-id="4cf5e-114">**[Pattern:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Four functions look for SSNs in four different patterns:</span></span>

  - <span data-ttu-id="4cf5e-115">Func_ssn يجد SSNs مع التنسيق القوي قبل عام 2011 التي يتم تنسيقها مع شرطات أو مسافات (ddd-ddddd or ddd ddddddddddddddddddddddddddddddddddddddddd</span><span class="sxs-lookup"><span data-stu-id="4cf5e-115">Func_ssn finds SSNs with pre-2011 strong formatting that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="4cf5e-116">Func_unformatted_ssn يجد SSNs مع التنسيق قوية قبل 2011 التي لم يتم تنسيقها كتسعة أرقام متتالية (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="4cf5e-116">Func_unformatted_ssn finds SSNs with pre-2011 strong formatting that are unformatted as nine consecutive digits (ddddddddd)</span></span>

  - <span data-ttu-id="4cf5e-117">Func_randomized_formatted_ssn يجد SSNs ما بعد 2011 التي تم تنسيقها مع شرطات أو مسافات (ddd-ddddd or ddd dddddddddddd)</span><span class="sxs-lookup"><span data-stu-id="4cf5e-117">Func_randomized_formatted_ssn finds post-2011 SSNs that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="4cf5e-118">Func_randomized_unformatted_ssn يجد SSNs ما بعد 2011 التي لم يتم تنسيقها كتسعة أرقام متتالية (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="4cf5e-118">Func_randomized_unformatted_ssn finds post-2011 SSNs that are unformatted as nine consecutive digits (ddddddddd)</span></span>

- <span data-ttu-id="4cf5e-119">**[المجموع الاختياري:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** لا، لا يوجد المجموع الاختياري</span><span class="sxs-lookup"><span data-stu-id="4cf5e-119">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** No, there is no Checksum</span></span>

- <span data-ttu-id="4cf5e-120">**[التعريف:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** سياسة DLP واثقة بنسبة 85٪ من أنها اكتشفت هذا النوع من المعلومات الحساسة إذا، على مقربة من 300 حرف:</span><span class="sxs-lookup"><span data-stu-id="4cf5e-120">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="4cf5e-121">Func_ssn [الدالة](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) العثور على المحتوى الذي يطابق النمط.</span><span class="sxs-lookup"><span data-stu-id="4cf5e-121">The [function Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) finds content that matches the pattern.</span></span>

  - <span data-ttu-id="4cf5e-122">تم العثور على كلمة رئيسية من [Keyword_ssn.](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn)</span><span class="sxs-lookup"><span data-stu-id="4cf5e-122">A keyword from [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) is found.</span></span> <span data-ttu-id="4cf5e-123">ومن أمثلة الكلمات الرئيسية: *الضمان الاجتماعي، الضمان الاجتماعي#، Soc Sec، SSN* .</span><span class="sxs-lookup"><span data-stu-id="4cf5e-123">Examples of keywords includes:  *Social Security, Social Security#, Soc Sec ,SSN*  .</span></span> <span data-ttu-id="4cf5e-124">على سبيل المثال، سيتم تشغيل العينة التالية لسياسة DLP SSN: **SSN: 489-36-8350**</span><span class="sxs-lookup"><span data-stu-id="4cf5e-124">For example, the following sample would trigger for the DLP SSN policy: **SSN: 489-36-8350**</span></span>
  
<span data-ttu-id="4cf5e-125">لمزيد من المعلومات حول ما هو مطلوب لSSNs ليتم الكشف عن المحتوى الخاص بك، راجع المقطع التالي في هذه المقالة: [ما أنواع المعلومات الحساسة البحث عن SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span><span class="sxs-lookup"><span data-stu-id="4cf5e-125">For more information on what is required for SSNs to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span></span>
  
<span data-ttu-id="4cf5e-126">باستخدام نوع معلومات حساسة مضمن ة مختلفة، راجع المقالة التالية للحصول على معلومات حول ما هو مطلوب للأنواع الأخرى: [ما تبحث عنه أنواع المعلومات الحساسة](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="4cf5e-126">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  