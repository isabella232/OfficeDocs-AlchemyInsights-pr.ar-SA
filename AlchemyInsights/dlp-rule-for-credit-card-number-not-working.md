---
title: قاعدة DLP لرقم بطاقة الائتمان لا يعمل
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: 80ff41b3e746f95278ccbf0df19eebb61f7f9ee0
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704188"
---
# <a name="dlp-issues-with-credit-card-numbers"></a><span data-ttu-id="5394d-102">مشكلات DLP مع أرقام بطاقات الائتمان</span><span class="sxs-lookup"><span data-stu-id="5394d-102">DLP issues with credit card numbers</span></span>

<span data-ttu-id="5394d-103">**هام**: خلال هذه الأوقات غير المسبوقة، نقوم باتخاذ الخطوات اللازمة لضمان توفر خدمات SharePoint Online و OneDrive بشكل كبير – الرجاء زيارة [تعديلات الميزات المؤقتة لـ SharePoint Online](https://aka.ms/ODSPAdjustments) للحصول على مزيد من المعلومات.</span><span class="sxs-lookup"><span data-stu-id="5394d-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="5394d-104">**مشكلات DLP مع أرقام بطاقات الائتمان**</span><span class="sxs-lookup"><span data-stu-id="5394d-104">**DLP issues with credit card numbers**</span></span>

<span data-ttu-id="5394d-105">هل تواجه مشاكل مع **منع فقدان البيانات (DLP)** لا تعمل للمحتوى الذي يحتوي على **رقم بطاقة الائتمان** عند استخدام نوع معلومات حساسة DLP في O365؟</span><span class="sxs-lookup"><span data-stu-id="5394d-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="5394d-106">إذا كان الأمر كذلك، تأكد من أن المحتوى الخاص بك يحتوي على المعلومات المطلوبة لتشغيل نهج DLP عند تقييمه.</span><span class="sxs-lookup"><span data-stu-id="5394d-106">If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated.</span></span> <span data-ttu-id="5394d-107">على سبيل المثال، بالنسبة **لسياسة بطاقة الائتمان** التي تم تكوينها بمستوى ثقة 85%، يتم تقييم ما يلي ويجب الكشف عنها حتى تقوم القاعدة بتشغيلها:</span><span class="sxs-lookup"><span data-stu-id="5394d-107">For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="5394d-108">**[التنسيق:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 رقمًا يمكن تنسيقها أو عدم تنسيقها (ddddddddddddd) ويجب أن تجتاز اختبار Luhn.</span><span class="sxs-lookup"><span data-stu-id="5394d-108">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span>

- <span data-ttu-id="5394d-109">**[نمط:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** نمط معقد وقوي للغاية يكشف البطاقات من جميع العلامات التجارية الكبرى في جميع أنحاء العالم ، بما في ذلك فيزا ، ماستركارد ، بطاقة ديسكفري ، JCB ، أمريكان إكسبريس ، بطاقات الهدايا ، وبطاقات العشاء.</span><span class="sxs-lookup"><span data-stu-id="5394d-109">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span>

- <span data-ttu-id="5394d-110">**[المجموع الاختياري:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** نعم، مجموع الاختيار لوهن</span><span class="sxs-lookup"><span data-stu-id="5394d-110">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Yes, the Luhn checksum</span></span>

- <span data-ttu-id="5394d-111">**[التعريف:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** سياسة DLP واثقة بنسبة 85٪ من أنها اكتشفت هذا النوع من المعلومات الحساسة إذا، على مقربة من 300 حرف:</span><span class="sxs-lookup"><span data-stu-id="5394d-111">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="5394d-112">Func_credit_card الدالة البحث عن المحتوى الذي يطابق النمط.</span><span class="sxs-lookup"><span data-stu-id="5394d-112">The function Func_credit_card finds content that matches the pattern.</span></span>

  - <span data-ttu-id="5394d-113">أحد ما يلي هو الصحيح:</span><span class="sxs-lookup"><span data-stu-id="5394d-113">One of the following is true:</span></span>

  - <span data-ttu-id="5394d-114">تم العثور على كلمة رئيسية من Keyword_cc_verification.</span><span class="sxs-lookup"><span data-stu-id="5394d-114">A keyword from Keyword_cc_verification is found.</span></span>

  - <span data-ttu-id="5394d-115">تم العثور على كلمة رئيسية من Keyword_cc_name</span><span class="sxs-lookup"><span data-stu-id="5394d-115">A keyword from Keyword_cc_name is found</span></span>

  - <span data-ttu-id="5394d-116">Func_expiration_date الدالة البحث عن تاريخ بتنسيق التاريخ الصحيح.</span><span class="sxs-lookup"><span data-stu-id="5394d-116">The function Func_expiration_date finds a date in the right date format.</span></span>

  - <span data-ttu-id="5394d-117">يمر المجموع الاختياري</span><span class="sxs-lookup"><span data-stu-id="5394d-117">The checksum passes</span></span>

    <span data-ttu-id="5394d-118">على سبيل المثال، سيتم تشغيل العينة التالية لسياسة رقم بطاقة الائتمان DLP:</span><span class="sxs-lookup"><span data-stu-id="5394d-118">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>

  - <span data-ttu-id="5394d-119">التأشيرة: 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="5394d-119">Visa: 4485 3647 3952 7352</span></span>
  
  - <span data-ttu-id="5394d-120">تنتهي صلاحيتها: 2/2009</span><span class="sxs-lookup"><span data-stu-id="5394d-120">Expires: 2/2009</span></span>

<span data-ttu-id="5394d-121">لمزيد من المعلومات حول ما هو مطلوب للكشف عن **رقم بطاقة الائتمان** للمحتوى الخاص بك، راجع القسم التالي في هذه المقالة: ما أنواع المعلومات [الحساسة البحث عن بطاقة الائتمان#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="5394d-121">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span></span>
  
<span data-ttu-id="5394d-122">باستخدام نوع معلومات حساسة مضمن ة مختلفة، راجع المقالة التالية للحصول على معلومات حول ما هو مطلوب للأنواع الأخرى: [ما تبحث عنه أنواع المعلومات الحساسة](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="5394d-122">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  