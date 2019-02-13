---
title: رقم بطاقة الائتمان لا تعمل قاعدة DLP
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: e1d60c493a27efb7f724d57051e21fad5bd0242f
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/12/2019
ms.locfileid: "29919067"
---
<span data-ttu-id="3deaa-p101">هل تواجه مشاكل في **منع فقدان البيانات (DLP)** لا يعمل للمحتوى الذي يحتوي على **رقم بطاقة الائتمان** عند استخدام نوع معلومات حساسة DLP في O365؟ إذا كان الأمر كذلك، تأكد من المحتوى الخاص بك يحتوي على المعلومات المطلوبة لتشغيل نهج DLP عندما يتم تقييمه. على سبيل المثال، **بطاقة الائتمان نهج** تكوين بمستوى ثقة 85 في المائة، التالية يتم تقييمها ويجب الكشف عن لتشغيل القاعدة:</span><span class="sxs-lookup"><span data-stu-id="3deaa-p101">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365? If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated. For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span> 
  
- <span data-ttu-id="3deaa-105">**[تنسيق:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** رقم 16 التي يمكن تنسيقها أو غير منسق (ددددددددددددددد) ويجب أن يجتاز اختبار ليون.</span><span class="sxs-lookup"><span data-stu-id="3deaa-105">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span> 
    
- <span data-ttu-id="3deaa-106">**[نموذج:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** نمط معقد للغاية وفعالية الكشف عن بطاقات من جميع العلامات التجارية الكبرى في العالم، بما في ذلك التأشيرات Mastercard، اكتشاف بطاقة، JCB، أمريكان إكسبريس، بطاقات الهدايا وبطاقات العشاء.</span><span class="sxs-lookup"><span data-stu-id="3deaa-106">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span> 
    
- <span data-ttu-id="3deaa-107">**[المجموع الاختباري:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** نعم، كان المجموع الاختباري ليون</span><span class="sxs-lookup"><span data-stu-id="3deaa-107">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Yes, the Luhn checksum</span></span> 
    
- <span data-ttu-id="3deaa-108">**[تعريف:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** هو نهج DLP 85% واثقاً من الكشف عن هذا النوع من المعلومات الهامة إذا مسافة 300 حرف:</span><span class="sxs-lookup"><span data-stu-id="3deaa-108">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span> 
    
  - <span data-ttu-id="3deaa-109">دالة Func_credit_card البحث عن المحتوى الذي يطابق النموذج.</span><span class="sxs-lookup"><span data-stu-id="3deaa-109">The function Func_credit_card finds content that matches the pattern.</span></span>
    
  - <span data-ttu-id="3deaa-110">أي مما يلي صحيحاً:</span><span class="sxs-lookup"><span data-stu-id="3deaa-110">One of the following is true:</span></span> 
    
  - <span data-ttu-id="3deaa-111">تم العثور على كلمة أساسية من Keyword_cc_verification.</span><span class="sxs-lookup"><span data-stu-id="3deaa-111">A keyword from Keyword_cc_verification is found.</span></span>
    
  - <span data-ttu-id="3deaa-112">تم العثور على كلمة أساسية من Keyword_cc_name</span><span class="sxs-lookup"><span data-stu-id="3deaa-112">A keyword from Keyword_cc_name is found</span></span>
    
  - <span data-ttu-id="3deaa-113">دالة Func_expiration_date عن تاريخ في تنسيق التاريخ الصحيح.</span><span class="sxs-lookup"><span data-stu-id="3deaa-113">The function Func_expiration_date finds a date in the right date format.</span></span>
    
  - <span data-ttu-id="3deaa-114">مسارات المجموع الاختباري</span><span class="sxs-lookup"><span data-stu-id="3deaa-114">The checksum passes</span></span>
    
    <span data-ttu-id="3deaa-115">على سبيل المثال، النموذج التالي سيثير "نهج DLP رقم بطاقة الائتمان":</span><span class="sxs-lookup"><span data-stu-id="3deaa-115">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>
    
  - <span data-ttu-id="3deaa-116">تأشيرة المرور: 7352 3952 3647 4485</span><span class="sxs-lookup"><span data-stu-id="3deaa-116">Visa: 4485 3647 3952 7352</span></span> 
    
  - <span data-ttu-id="3deaa-117">انتهاء الصلاحية: 2/2009</span><span class="sxs-lookup"><span data-stu-id="3deaa-117">Expires: 2/2009</span></span>
    
<span data-ttu-id="3deaa-118">لمزيد من المعلومات حول ما هو مطلوب **رقم بطاقة الائتمان** ليتم اكتشافها للمحتوى، راجع المقطع التالي في هذا المقال: [ما الحساسة معلومات الأنواع ابحث عن بطاقة الائتمان #](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="3deaa-118">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span></span>
  
<span data-ttu-id="3deaa-119">استخدام نوع معلومات حساسة مضمنة مختلفة، راجع المقالة التالية للحصول على المعلومات على ما هو مطلوب للأنواع الأخرى: [البحث عن "ما الحساسة معلومات الأنواع"](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="3deaa-119">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  

