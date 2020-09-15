---
title: قاعده DLP لعدم العمل
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
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: b221e66862ca01074f380fbb8433f8f9cac044cb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679356"
---
# <a name="dlp-issues-with-social-security-numbers"></a><span data-ttu-id="d9326-102">مشاكل DLP مع أرقام الأمان الاجتماعي</span><span class="sxs-lookup"><span data-stu-id="d9326-102">DLP issues with Social Security Numbers</span></span>

<span data-ttu-id="d9326-103">**هام**: خلال هذه الأوقات غير المسبوقة، نقوم باتخاذ الخطوات اللازمة لضمان توفر خدمات SharePoint Online و OneDrive بشكل كبير – الرجاء زيارة [تعديلات الميزات المؤقتة لـ SharePoint Online](https://aka.ms/ODSPAdjustments) للحصول على مزيد من المعلومات.</span><span class="sxs-lookup"><span data-stu-id="d9326-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="d9326-104">**مشاكل DLP مع سنس**</span><span class="sxs-lookup"><span data-stu-id="d9326-104">**DLP issues with SSNs**</span></span>

<span data-ttu-id="d9326-105">هل تواجه مشاكل متعلقة **بمنع فقدان البيانات (DLP)** لا تعمل علي المحتوي الذي يحتوي علي **رقم الأمان الاجتماعي (SSN)** عند استخدام نوع معلومات حساس في Microsoft 365 ؟</span><span class="sxs-lookup"><span data-stu-id="d9326-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Social Security Number (SSN)** when using a sensitive information type in Microsoft 365?</span></span> <span data-ttu-id="d9326-106">إذا كان الأمر كذلك ، فتاكد من ان المحتوي يحتوي علي المعلومات المطلوبة لما تبحث عنه نهج DLP.</span><span class="sxs-lookup"><span data-stu-id="d9326-106">If so, make sure your content contains the needed information for what the DLP policy is looking.</span></span> 
  
<span data-ttu-id="d9326-107">علي سبيل المثال ، بالنسبة إلى نهج SSN تم تكوينه باستخدام مستوي الثقة في 85% ، يتم تقييم التالي ويجب الكشف عنه لكي يتم تشغيل القاعدة:</span><span class="sxs-lookup"><span data-stu-id="d9326-107">For example, for an SSN policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="d9326-108">**[تنسيق:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 أرقام ، والتي قد تكون بنمط منسق أو غير منسق</span><span class="sxs-lookup"><span data-stu-id="d9326-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 digits, which may be in a formatted or unformatted pattern</span></span>

- <span data-ttu-id="d9326-109">**[النمط:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** تظهر أربعه دالات لسنس في أربعه نقوش مختلفه:</span><span class="sxs-lookup"><span data-stu-id="d9326-109">**[Pattern:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Four functions look for SSNs in four different patterns:</span></span>

  - <span data-ttu-id="d9326-110">Func_ssn 2011 البحث عن السنس التي تم تنسيقها باستخدام الشرط أو المسافات (ddd-dd أو ddd إلى dddd)</span><span class="sxs-lookup"><span data-stu-id="d9326-110">Func_ssn finds SSNs with pre-2011 strong formatting that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="d9326-111">Func_unformatted_ssn البحث عن السنس مع تنسيق 2011 القوي الذي تمت تهيئته علي انه تسعه أرقام متتالية (دددددددد)</span><span class="sxs-lookup"><span data-stu-id="d9326-111">Func_unformatted_ssn finds SSNs with pre-2011 strong formatting that are unformatted as nine consecutive digits (ddddddddd)</span></span>

  - <span data-ttu-id="d9326-112">تعثر الFunc_randomized_formatted_ssn علي 2011 سنس التي تم تنسيقها باستخدام الشرطات أو المسافات (ddd-dd أو ddd dd dddd)</span><span class="sxs-lookup"><span data-stu-id="d9326-112">Func_randomized_formatted_ssn finds post-2011 SSNs that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="d9326-113">تعثر الFunc_randomized_unformatted_ssn علي 2011 سنس التي تم تنسيقها علي انها تسعه أرقام متتالية (دددددددد)</span><span class="sxs-lookup"><span data-stu-id="d9326-113">Func_randomized_unformatted_ssn finds post-2011 SSNs that are unformatted as nine consecutive digits (ddddddddd)</span></span>

- <span data-ttu-id="d9326-114">**[المجموع الاختباري:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** لا ، لا توجد مجموعات اختباريه</span><span class="sxs-lookup"><span data-stu-id="d9326-114">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** No, there is no Checksum</span></span>

- <span data-ttu-id="d9326-115">**[تعريف:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** نهج DLP هو 85% تثق بأنه قد تم اكتشاف هذا النوع من المعلومات الهامه في حال وجوده في غضون أكثر من 300 حرفا:</span><span class="sxs-lookup"><span data-stu-id="d9326-115">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="d9326-116">تعثر [الدالة Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) علي المحتوي الذي يتطابق مع النمط.</span><span class="sxs-lookup"><span data-stu-id="d9326-116">The [function Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) finds content that matches the pattern.</span></span>

  - <span data-ttu-id="d9326-117">تم العثور علي كلمه أساسيه من [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) .</span><span class="sxs-lookup"><span data-stu-id="d9326-117">A keyword from [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) is found.</span></span> <span data-ttu-id="d9326-118">تتضمن أمثله الكلمات  *الاساسيه: الأمان الاجتماعي ، الأمان الاجتماعي # ، Soc Sec ، SSN*  .</span><span class="sxs-lookup"><span data-stu-id="d9326-118">Examples of keywords includes:  *Social Security, Social Security#, Soc Sec ,SSN*  .</span></span> <span data-ttu-id="d9326-119">علي سبيل المثال ، سيتم تشغيل النموذج التالي لنهج الاعداد الخاص ب DLP: **SSN: 489-36-8350**</span><span class="sxs-lookup"><span data-stu-id="d9326-119">For example, the following sample would trigger for the DLP SSN policy: **SSN: 489-36-8350**</span></span>
  
<span data-ttu-id="d9326-120">للحصول علي مزيد من المعلومات حول العناصر المطلوبة لسنس التي سيتم الكشف عنها لمحتويك ، راجع القسم التالي في هذه المقالة: [ما الذي تبحث عنه أنواع المعلومات الهامه لسنس](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)</span><span class="sxs-lookup"><span data-stu-id="d9326-120">For more information on what is required for SSNs to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for SSNs](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)</span></span>
  
<span data-ttu-id="d9326-121">باستخدام نوع آخر من المعلومات الحساسة المضمنة ، راجع المقالة التالية للحصول علي معلومات حول ما هو مطلوب للأنواع الأخرى: [ما الذي تبحث عنه أنواع المعلومات الهامه](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="d9326-121">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  