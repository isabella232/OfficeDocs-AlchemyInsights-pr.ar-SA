---
title: قاعده DLP لرقم بطاقة الائتمان لا يعمل
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
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: d5dd6354e7a1bcbb7f2fb917952ddbee5077e88d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679428"
---
# <a name="dlp-issues-with-credit-card-numbers"></a><span data-ttu-id="dd1b6-102">مشاكل DLP مع أرقام بطاقات الائتمان</span><span class="sxs-lookup"><span data-stu-id="dd1b6-102">DLP issues with credit card numbers</span></span>

<span data-ttu-id="dd1b6-103">**هام**: خلال هذه الأوقات غير المسبوقة، نقوم باتخاذ الخطوات اللازمة لضمان توفر خدمات SharePoint Online و OneDrive بشكل كبير – الرجاء زيارة [تعديلات الميزات المؤقتة لـ SharePoint Online](https://aka.ms/ODSPAdjustments) للحصول على مزيد من المعلومات.</span><span class="sxs-lookup"><span data-stu-id="dd1b6-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="dd1b6-104">**مشاكل DLP مع أرقام بطاقات الائتمان**</span><span class="sxs-lookup"><span data-stu-id="dd1b6-104">**DLP issues with credit card numbers**</span></span>

<span data-ttu-id="dd1b6-105">هل تواجه مشاكل متعلقة **بمنع فقدان البيانات (DLP)** لا تعمل علي المحتوي الذي يحتوي علي **رقم بطاقة ائتمان** عند استخدام نوع معلومات الحساسية ل DLP في O365 ؟</span><span class="sxs-lookup"><span data-stu-id="dd1b6-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="dd1b6-106">إذا كان الأمر كذلك ، فتاكد من ان المحتوي يحتوي علي المعلومات المطلوبة لتشغيل نهج DLP عند تقييمه.</span><span class="sxs-lookup"><span data-stu-id="dd1b6-106">If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated.</span></span> <span data-ttu-id="dd1b6-107">علي سبيل المثال ، بالنسبة **لسياسة بطاقة الائتمان** التي تم تكوينها باستخدام مستوي الثقة في 85% ، يتم تقييم التالية ويجب الكشف عنها ليتم تشغيل القاعدة:</span><span class="sxs-lookup"><span data-stu-id="dd1b6-107">For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="dd1b6-108">**[تنسيق:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 خانه رقميه يمكن تنسيقها أو تهيئتها (ددددددددددددددد) ويجب ان تمرر اختبار لوهن.</span><span class="sxs-lookup"><span data-stu-id="dd1b6-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span>

- <span data-ttu-id="dd1b6-109">**[النمط:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** نمط معقد جدا وقوي يقوم بالكشف عن البطاقات من كل المنتجات الرئيسية في انحاء العالم ، بما في ذلك التاشيره والMasterCard والكشف عن البطاقات والJCB فالامريكيه وبطاقات الهدايا وبطاقات دينير.</span><span class="sxs-lookup"><span data-stu-id="dd1b6-109">**[Pattern:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span>

- <span data-ttu-id="dd1b6-110">**[المجموع الاختباري:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** نعم ، المجموع الاختباري للوهن</span><span class="sxs-lookup"><span data-stu-id="dd1b6-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Yes, the Luhn checksum</span></span>

- <span data-ttu-id="dd1b6-111">**[تعريف:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** نهج DLP هو 85% تثق بأنه قد تم اكتشاف هذا النوع من المعلومات الهامه في حال وجوده في غضون أكثر من 300 حرفا:</span><span class="sxs-lookup"><span data-stu-id="dd1b6-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="dd1b6-112">تعثر الدالة Func_credit_card علي المحتوي الذي يتطابق مع النمط.</span><span class="sxs-lookup"><span data-stu-id="dd1b6-112">The function Func_credit_card finds content that matches the pattern.</span></span>

  - <span data-ttu-id="dd1b6-113">يعد أحد الخيارات التالية صحيحا:</span><span class="sxs-lookup"><span data-stu-id="dd1b6-113">One of the following is true:</span></span>

  - <span data-ttu-id="dd1b6-114">تم العثور علي كلمه أساسيه من Keyword_cc_verification.</span><span class="sxs-lookup"><span data-stu-id="dd1b6-114">A keyword from Keyword_cc_verification is found.</span></span>

  - <span data-ttu-id="dd1b6-115">تم العثور علي كلمه أساسيه من Keyword_cc_name</span><span class="sxs-lookup"><span data-stu-id="dd1b6-115">A keyword from Keyword_cc_name is found</span></span>

  - <span data-ttu-id="dd1b6-116">تعثر الدالة Func_expiration_date علي تاريخ بتنسيق التاريخ الصحيح.</span><span class="sxs-lookup"><span data-stu-id="dd1b6-116">The function Func_expiration_date finds a date in the right date format.</span></span>

  - <span data-ttu-id="dd1b6-117">يمرر المجموع الاختباري</span><span class="sxs-lookup"><span data-stu-id="dd1b6-117">The checksum passes</span></span>

    <span data-ttu-id="dd1b6-118">علي سبيل المثال ، سيتم تشغيل النموذج التالي لنهج رقم بطاقة ائتمان DLP:</span><span class="sxs-lookup"><span data-stu-id="dd1b6-118">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>

  - <span data-ttu-id="dd1b6-119">التاشيره: 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="dd1b6-119">Visa: 4485 3647 3952 7352</span></span>
  
  - <span data-ttu-id="dd1b6-120">تنتهي الصلاحية: 2/2009</span><span class="sxs-lookup"><span data-stu-id="dd1b6-120">Expires: 2/2009</span></span>

<span data-ttu-id="dd1b6-121">للحصول علي مزيد من المعلومات حول ما هو مطلوب لاكتشاف **رقم بطاقة الائتمان** للمحتوي ، راجع القسم التالي في هذه المقالة: [ما الذي تبحث عنه أنواع المعلومات الحساسة عن بطاقة الائتمان #](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="dd1b6-121">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)</span></span>
  
<span data-ttu-id="dd1b6-122">باستخدام نوع آخر من المعلومات الحساسة المضمنة ، راجع المقالة التالية للحصول علي معلومات حول ما هو مطلوب للأنواع الأخرى: [ما الذي تبحث عنه أنواع المعلومات الهامه](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="dd1b6-122">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  