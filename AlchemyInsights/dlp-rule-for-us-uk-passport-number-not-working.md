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
ms.openlocfilehash: c63e814059c897531109aa78725e9811b311fb27
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931249"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a><span data-ttu-id="d5cf9-102">مشاكل مع DLP - أرقام جوازات السفر الأمريكية /المملكة المتحدة</span><span class="sxs-lookup"><span data-stu-id="d5cf9-102">Problems with DLP - US/UK passport numbers</span></span>

<span data-ttu-id="d5cf9-103">**هام:** يعمل العديد من عملاء SharePoint Online و OneDrive على تشغيل تطبيقات مهمة للأعمال مقابل الخدمة التي تعمل في الخلفية.</span><span class="sxs-lookup"><span data-stu-id="d5cf9-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="d5cf9-104">وتشمل هذه ترحيل المحتوى، منع فقدان البيانات (DLP)، وحلول النسخ الاحتياطي.</span><span class="sxs-lookup"><span data-stu-id="d5cf9-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="d5cf9-105">خلال هذه الأوقات غير المسبوقة، نتخذ خطوات لضمان أن تظل خدمات SharePoint Online و OneDrive متاحة للغاية وموثوقة للمستخدمين الذين يعتمدون على الخدمة أكثر من أي وقت مضى في سيناريوهات العمل عن بعد.</span><span class="sxs-lookup"><span data-stu-id="d5cf9-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="d5cf9-106">ولدعم هذا الهدف، قمنا بتنفيذ قيود خنق أكثر صرامة على تطبيقات الخلفية (الترحيل وDLP وحلول النسخ الاحتياطي) خلال ساعات النهار في أيام الأسبوع.</span><span class="sxs-lookup"><span data-stu-id="d5cf9-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="d5cf9-107">يجب أن تتوقع أن تحقق هذه التطبيقات إنتاجية محدودة جدًا خلال هذه الأوقات.</span><span class="sxs-lookup"><span data-stu-id="d5cf9-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="d5cf9-108">ومع ذلك ، خلال ساعات المساء وعطلة نهاية الأسبوع للمنطقة ، ستكون الخدمة جاهزة لمعالجة حجم أكبر بكثير من الطلبات من تطبيقات الخلفية.</span><span class="sxs-lookup"><span data-stu-id="d5cf9-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="d5cf9-109">**DLP القضايا مع أرقام جوازات السفر الأمريكية / المملكة المتحدة**</span><span class="sxs-lookup"><span data-stu-id="d5cf9-109">**DLP issues with US/UK passport numbers**</span></span>

<span data-ttu-id="d5cf9-110">هل تواجه مشاكل مع **منع فقدان البيانات (DLP)** لا تعمل للمحتوى الذي يحتوي على **رقم جواز سفر الولايات المتحدة / المملكة المتحدة** عند استخدام نوع معلومات حساسة DLP في O365؟</span><span class="sxs-lookup"><span data-stu-id="d5cf9-110">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US/UK passport number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="d5cf9-111">إذا كان الأمر كذلك، تأكد من أن المحتوى الخاص بك يحتوي على المعلومات المطلوبة لما تبحث عنه سياسة DLP عند تقييمه.</span><span class="sxs-lookup"><span data-stu-id="d5cf9-111">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="d5cf9-112">على سبيل المثال، بالنسبة لسياسة **رقم جواز سفر الولايات المتحدة والمملكة المتحدة** التي تم تكوينها بمستوى ثقة 75٪، يتم تقييم ما يلي ويجب الكشف عنها لتشغيل القاعدة</span><span class="sxs-lookup"><span data-stu-id="d5cf9-112">For example, for a **US/UK passport number** policy configured with a confidence level of 75%, the following are evaluated and must be detected for the rule to trigger</span></span>
  
- <span data-ttu-id="d5cf9-113">**[الشكل:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** تسعة أرقام</span><span class="sxs-lookup"><span data-stu-id="d5cf9-113">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Nine digits</span></span>

- <span data-ttu-id="d5cf9-114">**[نمط:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** تسعة أرقام متتالية</span><span class="sxs-lookup"><span data-stu-id="d5cf9-114">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Nine consecutive digits</span></span>

- <span data-ttu-id="d5cf9-115">**[المجموع الاختياري:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** لا، لا يوجد المجموع الاختياري</span><span class="sxs-lookup"><span data-stu-id="d5cf9-115">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="d5cf9-116">**[التعريف:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** سياسة DLP واثقة بنسبة 75٪ من أنها اكتشفت هذا النوع من المعلومات الحساسة إذا، على مقربة من 300 حرف:</span><span class="sxs-lookup"><span data-stu-id="d5cf9-116">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="d5cf9-117">Func_usa_uk_passport تعثر الدالة على المحتوى الذي يطابق النقش.</span><span class="sxs-lookup"><span data-stu-id="d5cf9-117">The function Func_usa_uk_passport finds content that matches the pattern.</span></span>

  - <span data-ttu-id="d5cf9-118">تم العثور على كلمة رئيسية من Keyword_passport.</span><span class="sxs-lookup"><span data-stu-id="d5cf9-118">A keyword from Keyword_passport is found.</span></span>

    <span data-ttu-id="d5cf9-119">على سبيل المثال، ستثير العينة التالية سياسة **رقم جواز السفر الأمريكي/المملكة المتحدة:** رقم جواز السفر الأمريكي 123456789</span><span class="sxs-lookup"><span data-stu-id="d5cf9-119">For example, the following sample would trigger for the **US/UK passport number** policy: U.S. Passport number 123456789</span></span>

<span data-ttu-id="d5cf9-120">لمزيد من المعلومات حول ما هو مطلوب للكشف عن رقم جواز سفر الولايات المتحدة والمملكة المتحدة للمحتوى الخاص بك، راجع القسم التالي في هذه المقالة: [ما أنواع المعلومات الحساسة البحث عن رقم جواز سفر الولايات المتحدة / المملكة المتحدة](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span><span class="sxs-lookup"><span data-stu-id="d5cf9-120">For more information on what is required for a US/UK Passport Number to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US/UK Passport Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span></span>
  
<span data-ttu-id="d5cf9-121">باستخدام نوع معلومات حساسة مضمن ة مختلفة، راجع المقالة التالية للحصول على معلومات حول ما هو مطلوب للأنواع الأخرى: [ما تبحث عنه أنواع المعلومات الحساسة](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="d5cf9-121">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  