---
title: قاعدة DLP لرقم جواز السفر الأمريكي /UK لا يعمل
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: 534e258c31a9a71c618765511487487c53f455b5
ms.sourcegitcommit: d108a2da2f5dab05246e30b5108cca5173e09051
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/26/2020
ms.locfileid: "42977093"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a><span data-ttu-id="4d2b3-102">مشاكل مع DLP - أرقام جوازات السفر الأمريكية /المملكة المتحدة</span><span class="sxs-lookup"><span data-stu-id="4d2b3-102">Problems with DLP - US/UK passport numbers</span></span>

<span data-ttu-id="4d2b3-103">**هام:** خلال هذه الأوقات غير المسبوقة، نتخذ خطوات لضمان أن تظل خدمات SharePoint Online و OneDrive متاحة للغاية - يرجى زيارة [SharePoint Online تعديلات الميزة المؤقتة](https://aka.ms/ODSPAdjustments) للحصول على مزيد من المعلومات.</span><span class="sxs-lookup"><span data-stu-id="4d2b3-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="4d2b3-104">**DLP القضايا مع أرقام جوازات السفر الأمريكية / المملكة المتحدة**</span><span class="sxs-lookup"><span data-stu-id="4d2b3-104">**DLP issues with US/UK passport numbers**</span></span>

<span data-ttu-id="4d2b3-105">هل تواجه مشاكل مع **منع فقدان البيانات (DLP)** لا تعمل للمحتوى الذي يحتوي على **رقم جواز سفر الولايات المتحدة / المملكة المتحدة** عند استخدام نوع معلومات حساسة DLP في O365؟</span><span class="sxs-lookup"><span data-stu-id="4d2b3-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US/UK passport number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="4d2b3-106">إذا كان الأمر كذلك، تأكد من أن المحتوى الخاص بك يحتوي على المعلومات المطلوبة لما تبحث عنه سياسة DLP عند تقييمه.</span><span class="sxs-lookup"><span data-stu-id="4d2b3-106">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="4d2b3-107">على سبيل المثال، بالنسبة لسياسة **رقم جواز سفر الولايات المتحدة والمملكة المتحدة** التي تم تكوينها بمستوى ثقة 75٪، يتم تقييم ما يلي ويجب الكشف عنها لتشغيل القاعدة</span><span class="sxs-lookup"><span data-stu-id="4d2b3-107">For example, for a **US/UK passport number** policy configured with a confidence level of 75%, the following are evaluated and must be detected for the rule to trigger</span></span>
  
- <span data-ttu-id="4d2b3-108">**[الشكل:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** تسعة أرقام</span><span class="sxs-lookup"><span data-stu-id="4d2b3-108">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Nine digits</span></span>

- <span data-ttu-id="4d2b3-109">**[نمط:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** تسعة أرقام متتالية</span><span class="sxs-lookup"><span data-stu-id="4d2b3-109">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Nine consecutive digits</span></span>

- <span data-ttu-id="4d2b3-110">**[المجموع الاختياري:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** لا، لا يوجد المجموع الاختياري</span><span class="sxs-lookup"><span data-stu-id="4d2b3-110">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="4d2b3-111">**[التعريف:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** سياسة DLP واثقة بنسبة 75٪ من أنها اكتشفت هذا النوع من المعلومات الحساسة إذا، على مقربة من 300 حرف:</span><span class="sxs-lookup"><span data-stu-id="4d2b3-111">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="4d2b3-112">Func_usa_uk_passport تعثر الدالة على المحتوى الذي يطابق النقش.</span><span class="sxs-lookup"><span data-stu-id="4d2b3-112">The function Func_usa_uk_passport finds content that matches the pattern.</span></span>

  - <span data-ttu-id="4d2b3-113">تم العثور على كلمة رئيسية من Keyword_passport.</span><span class="sxs-lookup"><span data-stu-id="4d2b3-113">A keyword from Keyword_passport is found.</span></span>

    <span data-ttu-id="4d2b3-114">على سبيل المثال، ستثير العينة التالية سياسة **رقم جواز السفر الأمريكي/المملكة المتحدة:** رقم جواز السفر الأمريكي 123456789</span><span class="sxs-lookup"><span data-stu-id="4d2b3-114">For example, the following sample would trigger for the **US/UK passport number** policy: U.S. Passport number 123456789</span></span>

<span data-ttu-id="4d2b3-115">لمزيد من المعلومات حول ما هو مطلوب للكشف عن رقم جواز سفر الولايات المتحدة والمملكة المتحدة للمحتوى الخاص بك، راجع القسم التالي في هذه المقالة: [ما أنواع المعلومات الحساسة البحث عن رقم جواز سفر الولايات المتحدة / المملكة المتحدة](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span><span class="sxs-lookup"><span data-stu-id="4d2b3-115">For more information on what is required for a US/UK Passport Number to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US/UK Passport Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span></span>
  
<span data-ttu-id="4d2b3-116">باستخدام نوع معلومات حساسة مضمن ة مختلفة، راجع المقالة التالية للحصول على معلومات حول ما هو مطلوب للأنواع الأخرى: [ما تبحث عنه أنواع المعلومات الحساسة](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="4d2b3-116">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  