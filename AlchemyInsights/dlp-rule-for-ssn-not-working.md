---
title: دلب قاعدة للتأمين الاجتماعي لا يعمل
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
ms.openlocfilehash: fffd355279b064b31c0a8bf60518b15ee1ed1848
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/28/2019
ms.locfileid: "35389420"
---
# <a name="dlp-issues-with-social-security-numbers"></a><span data-ttu-id="0c480-102">مشاكل تقنية DLP مع أرقام الضمان الاجتماعي</span><span class="sxs-lookup"><span data-stu-id="0c480-102">DLP issues with Social Security Numbers</span></span>

<span data-ttu-id="0c480-103">هل تواجه مشاكل في **منع فقدان البيانات (DLP)** لا يعمل للمحتوى الذي يحتوي على **"رقم التأمين الاجتماعي" (SSN)** عند استخدام نوع معلومات حساسة في Office 365؟</span><span class="sxs-lookup"><span data-stu-id="0c480-103">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Social Security Number (SSN)** when using a sensitive information type in Office 365?</span></span> <span data-ttu-id="0c480-104">إذا كان الأمر كذلك، تأكد من أن المحتوى الخاص بك يحتوي على المعلومات المطلوبة لما يبحث النهج DLP.</span><span class="sxs-lookup"><span data-stu-id="0c480-104">If so, make sure your content contains the needed information for what the DLP policy is looking.</span></span> 
  
<span data-ttu-id="0c480-105">على سبيل المثال، لنهج التأمين الاجتماعي تكوين بمستوى ثقة 85%، التالية يتم تقييمها ويجب الكشف عن لتشغيل القاعدة:</span><span class="sxs-lookup"><span data-stu-id="0c480-105">For example, for an SSN policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="0c480-106">**[التنسيق:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 أرقام، الذي قد يكون في نمط منسق أو غير منسق</span><span class="sxs-lookup"><span data-stu-id="0c480-106">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 digits, which may be in a formatted or unformatted pattern</span></span>

- <span data-ttu-id="0c480-107">**[نموذج:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** أربع مهام البحث عن شبكات الأمان الاجتماعي في أربعة أنماط مختلفة:</span><span class="sxs-lookup"><span data-stu-id="0c480-107">**[Pattern:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Four functions look for SSNs in four different patterns:</span></span>

  - <span data-ttu-id="0c480-108">Func_ssn البحث عن شبكات الأمان الاجتماعي ب 2011 قبل تنسيق قوي المنسقة بواسطة شرطات أو مسافات (dddd dd ddd أو ddd يوم dddd)</span><span class="sxs-lookup"><span data-stu-id="0c480-108">Func_ssn finds SSNs with pre-2011 strong formatting that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="0c480-109">Func_unformatted_ssn البحث عن شبكات الأمان الاجتماعي ب 2011 قبل تنسيق قوي التي تكون غير منسقة تسعة أرقام متتالية (دددددددد)</span><span class="sxs-lookup"><span data-stu-id="0c480-109">Func_unformatted_ssn finds SSNs with pre-2011 strong formatting that are unformatted as nine consecutive digits (ddddddddd)</span></span>

  - <span data-ttu-id="0c480-110">ويرى Func_randomized_formatted_ssn 2011 نشر شبكات الأمان الاجتماعي التي تم تنسيقها باستخدام الشرط أو مسافات (dddd dd ddd أو ddd يوم dddd)</span><span class="sxs-lookup"><span data-stu-id="0c480-110">Func_randomized_formatted_ssn finds post-2011 SSNs that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="0c480-111">ويرى Func_randomized_unformatted_ssn 2011 نشر شبكات الأمان الاجتماعي التي تكون غير منسقة تسعة أرقام متتالية (دددددددد)</span><span class="sxs-lookup"><span data-stu-id="0c480-111">Func_randomized_unformatted_ssn finds post-2011 SSNs that are unformatted as nine consecutive digits (ddddddddd)</span></span>

- <span data-ttu-id="0c480-112">**[المجموع الاختباري:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** لا، هناك لم المجموع الاختباري</span><span class="sxs-lookup"><span data-stu-id="0c480-112">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** No, there is no Checksum</span></span>

- <span data-ttu-id="0c480-113">**[تعريف:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** هو نهج DLP 85% واثقاً من الكشف عن هذا النوع من المعلومات الهامة إذا مسافة 300 حرف:</span><span class="sxs-lookup"><span data-stu-id="0c480-113">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="0c480-114">[دالة Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) البحث عن المحتوى الذي يطابق النموذج.</span><span class="sxs-lookup"><span data-stu-id="0c480-114">The [function Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) finds content that matches the pattern.</span></span>

  - <span data-ttu-id="0c480-115">تم العثور على كلمة أساسية من [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) .</span><span class="sxs-lookup"><span data-stu-id="0c480-115">A keyword from [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) is found.</span></span> <span data-ttu-id="0c480-116">تتضمن أمثلة للكلمات الأساسية: *الضمان الاجتماعي، # الضمان الاجتماعي، شركة نفط الجنوب الثانية، والتأمين الاجتماعي* .</span><span class="sxs-lookup"><span data-stu-id="0c480-116">Examples of keywords includes:  *Social Security, Social Security#, Soc Sec ,SSN*  .</span></span> <span data-ttu-id="0c480-117">على سبيل المثال، فسيتم تشغيل النموذج التالي لنهج التأمين الاجتماعي DLP: **رقم الضمان الاجتماعي: 489-36-8350**</span><span class="sxs-lookup"><span data-stu-id="0c480-117">For example, the following sample would trigger for the DLP SSN policy: **SSN: 489-36-8350**</span></span>
  
<span data-ttu-id="0c480-118">لمزيد من المعلومات حول ما هو مطلوب لشبكات الأمان الاجتماعي بأن يتم كشفه للمحتوى، راجع المقطع التالي في هذا المقال: [ما الحساسة معلومات الأنواع البحث عن شبكات الأمان الاجتماعي](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span><span class="sxs-lookup"><span data-stu-id="0c480-118">For more information on what is required for SSNs to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span></span>
  
<span data-ttu-id="0c480-119">استخدام نوع معلومات حساسة مضمنة مختلفة، راجع المقالة التالية للحصول على المعلومات على ما هو مطلوب للأنواع الأخرى: [البحث عن "ما الحساسة معلومات الأنواع"](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="0c480-119">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  