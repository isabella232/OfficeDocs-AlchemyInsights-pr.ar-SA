---
title: دلب قاعدة للولايات المتحدة/"المملكة المتحدة رقم جواز السفر" لا يعمل
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
ms.openlocfilehash: bc91af8be58d49204f84cd7d22f481348af3c013
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/22/2019
ms.locfileid: "36529906"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a><span data-ttu-id="c4647-102">مشاكل تقنية DLP-الولايات المتحدة/المملكة المتحدة رقم جواز السفر</span><span class="sxs-lookup"><span data-stu-id="c4647-102">Problems with DLP - US/UK Passport Numbers</span></span>

<span data-ttu-id="c4647-103">هل تواجه مشاكل **منع فقدان البيانات (DLP)** لا يعمل لاحتواء المحتوى **الولايات المتحدة/"المملكة المتحدة رقم جواز السفر"** عند استخدام نوع معلومات حساسة DLP في O365؟</span><span class="sxs-lookup"><span data-stu-id="c4647-103">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US/UK Passport Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="c4647-104">إذا كان الأمر كذلك، تأكد من أن المحتوى الخاص بك يحتوي على المعلومات المطلوبة لما نهج DLP تبحث عنه عندما يتم تقييم.</span><span class="sxs-lookup"><span data-stu-id="c4647-104">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="c4647-105">على سبيل المثال، **الولايات المتحدة/"المملكة المتحدة رقم جواز السفر"** النهج المكون بمستوى ثقة 75%، التالية يتم تقييمها ويجب الكشف عن لتشغيل القاعدة</span><span class="sxs-lookup"><span data-stu-id="c4647-105">For example, for a **US/UK Passport Number** policy configured with a confidence level of 75%, the following are evaluated and must be detected for the rule to trigger</span></span>
  
- <span data-ttu-id="c4647-106">**[تنسيق:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** تسعة أرقام</span><span class="sxs-lookup"><span data-stu-id="c4647-106">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Nine digits</span></span>

- <span data-ttu-id="c4647-107">**[نموذج:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** تسعة أرقام متتالية</span><span class="sxs-lookup"><span data-stu-id="c4647-107">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Nine consecutive digits</span></span>

- <span data-ttu-id="c4647-108">**[المجموع الاختباري:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** لا، هناك لم المجموع الاختباري</span><span class="sxs-lookup"><span data-stu-id="c4647-108">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="c4647-109">**[تعريف:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** نهج DLP هي 75% واثقاً من الكشف عن هذا النوع من المعلومات الهامة إذا مسافة 300 حرف:</span><span class="sxs-lookup"><span data-stu-id="c4647-109">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="c4647-110">دالة Func_usa_uk_passport البحث عن المحتوى الذي يطابق النموذج.</span><span class="sxs-lookup"><span data-stu-id="c4647-110">The function Func_usa_uk_passport finds content that matches the pattern.</span></span>

  - <span data-ttu-id="c4647-111">تم العثور على كلمة أساسية من Keyword_passport.</span><span class="sxs-lookup"><span data-stu-id="c4647-111">A keyword from Keyword_passport is found.</span></span>

    <span data-ttu-id="c4647-112">على سبيل المثال، فسيتم تشغيل النموذج التالي **الولايات المتحدة/"المملكة المتحدة رقم جواز السفر"** النهج: رقم "جواز السفر الأمريكي" 123456789</span><span class="sxs-lookup"><span data-stu-id="c4647-112">For example, the following sample would trigger for the **US/UK Passport Number** policy: U.S. Passport number 123456789</span></span>

<span data-ttu-id="c4647-113">لمزيد من المعلومات حول ما هو مطلوب للولايات المتحدة/"رقم جواز السفر المملكة المتحدة" بأن يتم كشفه للمحتوى، راجع المقطع التالي في هذه المقالة: [مظهر "ما الحساسة معلومات الأنواع" للولايات المتحدة/"المملكة المتحدة رقم جواز السفر"](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span><span class="sxs-lookup"><span data-stu-id="c4647-113">For more information on what is required for a US/UK Passport Number to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US/UK Passport Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span></span>
  
<span data-ttu-id="c4647-114">استخدام نوع معلومات حساسة مضمنة مختلفة، راجع المقالة التالية للحصول على المعلومات على ما هو مطلوب للأنواع الأخرى: [البحث عن "ما الحساسة معلومات الأنواع"](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="c4647-114">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  