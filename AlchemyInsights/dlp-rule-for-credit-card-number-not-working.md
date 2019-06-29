---
title: رقم بطاقة الائتمان لا تعمل قاعدة DLP
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: 5d3bdb3b074c485a2b19e934724ba6e74c84deae
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/28/2019
ms.locfileid: "35389564"
---
# <a name="dlp-issues-with-credit-card-numbers"></a><span data-ttu-id="15cc6-102">مشاكل تقنية DLP مع "أرقام بطاقات الائتمان"</span><span class="sxs-lookup"><span data-stu-id="15cc6-102">DLP issues with Credit Card Numbers</span></span>

<span data-ttu-id="15cc6-103">هل تواجه مشاكل في **منع فقدان البيانات (DLP)** لا يعمل للمحتوى الذي يحتوي على **رقم بطاقة الائتمان** عند استخدام نوع معلومات حساسة DLP في O365؟</span><span class="sxs-lookup"><span data-stu-id="15cc6-103">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="15cc6-104">إذا كان الأمر كذلك، تأكد من المحتوى الخاص بك يحتوي على المعلومات المطلوبة لتشغيل نهج DLP عندما يتم تقييمه.</span><span class="sxs-lookup"><span data-stu-id="15cc6-104">If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated.</span></span> <span data-ttu-id="15cc6-105">على سبيل المثال، **بطاقة الائتمان نهج** تكوين بمستوى ثقة 85 في المائة، التالية يتم تقييمها ويجب الكشف عن لتشغيل القاعدة:</span><span class="sxs-lookup"><span data-stu-id="15cc6-105">For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="15cc6-106">**[تنسيق:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** رقم 16 التي يمكن تنسيقها أو غير منسق (ددددددددددددددد) ويجب أن يجتاز اختبار ليون.</span><span class="sxs-lookup"><span data-stu-id="15cc6-106">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span>

- <span data-ttu-id="15cc6-107">**[نموذج:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** نمط معقد للغاية وفعالية الكشف عن بطاقات من جميع العلامات التجارية الكبرى في العالم، بما في ذلك التأشيرات ماستر كارد، بطاقة اكتشاف، JCB، أمريكان إكسبريس، بطاقات الهدايا وبطاقات العشاء.</span><span class="sxs-lookup"><span data-stu-id="15cc6-107">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span>

- <span data-ttu-id="15cc6-108">**[المجموع الاختباري:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** نعم، كان المجموع الاختباري ليون</span><span class="sxs-lookup"><span data-stu-id="15cc6-108">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Yes, the Luhn checksum</span></span>

- <span data-ttu-id="15cc6-109">**[تعريف:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** هو نهج DLP 85% واثقاً من الكشف عن هذا النوع من المعلومات الهامة إذا مسافة 300 حرف:</span><span class="sxs-lookup"><span data-stu-id="15cc6-109">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="15cc6-110">دالة Func_credit_card البحث عن المحتوى الذي يطابق النموذج.</span><span class="sxs-lookup"><span data-stu-id="15cc6-110">The function Func_credit_card finds content that matches the pattern.</span></span>

  - <span data-ttu-id="15cc6-111">أي مما يلي صحيحاً:</span><span class="sxs-lookup"><span data-stu-id="15cc6-111">One of the following is true:</span></span>

  - <span data-ttu-id="15cc6-112">تم العثور على كلمة أساسية من Keyword_cc_verification.</span><span class="sxs-lookup"><span data-stu-id="15cc6-112">A keyword from Keyword_cc_verification is found.</span></span>

  - <span data-ttu-id="15cc6-113">تم العثور على كلمة أساسية من Keyword_cc_name</span><span class="sxs-lookup"><span data-stu-id="15cc6-113">A keyword from Keyword_cc_name is found</span></span>

  - <span data-ttu-id="15cc6-114">دالة Func_expiration_date عن تاريخ في تنسيق التاريخ الصحيح.</span><span class="sxs-lookup"><span data-stu-id="15cc6-114">The function Func_expiration_date finds a date in the right date format.</span></span>

  - <span data-ttu-id="15cc6-115">مسارات المجموع الاختباري</span><span class="sxs-lookup"><span data-stu-id="15cc6-115">The checksum passes</span></span>

    <span data-ttu-id="15cc6-116">على سبيل المثال، النموذج التالي سيثير "نهج DLP رقم بطاقة الائتمان":</span><span class="sxs-lookup"><span data-stu-id="15cc6-116">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>

  - <span data-ttu-id="15cc6-117">تأشيرة المرور: 7352 3952 3647 4485</span><span class="sxs-lookup"><span data-stu-id="15cc6-117">Visa: 4485 3647 3952 7352</span></span>
  
  - <span data-ttu-id="15cc6-118">انتهاء الصلاحية: 2/2009</span><span class="sxs-lookup"><span data-stu-id="15cc6-118">Expires: 2/2009</span></span>

<span data-ttu-id="15cc6-119">لمزيد من المعلومات حول ما هو مطلوب **رقم بطاقة الائتمان** ليتم اكتشافها للمحتوى، راجع المقطع التالي في هذا المقال: [ما الحساسة معلومات الأنواع ابحث عن بطاقة الائتمان #](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="15cc6-119">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span></span>
  
<span data-ttu-id="15cc6-120">استخدام نوع معلومات حساسة مضمنة مختلفة، راجع المقالة التالية للحصول على المعلومات على ما هو مطلوب للأنواع الأخرى: [البحث عن "ما الحساسة معلومات الأنواع"](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="15cc6-120">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  