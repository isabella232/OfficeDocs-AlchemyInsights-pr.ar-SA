---
title: قاعده DLP لرقم Passport للولايات المتحدة/المملكة المتحدة لا يعمل
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
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: c6c7191f380f264113e2042f2869d9767922b2cc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679211"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a><span data-ttu-id="44f01-102">المشاكل المتعلقة بأرقام passport للولايات المتحدة/المملكة المتحدة</span><span class="sxs-lookup"><span data-stu-id="44f01-102">Problems with DLP - US/UK passport numbers</span></span>

<span data-ttu-id="44f01-103">**هام**: خلال هذه الأوقات غير المسبوقة، نقوم باتخاذ الخطوات اللازمة لضمان توفر خدمات SharePoint Online و OneDrive بشكل كبير – الرجاء زيارة [تعديلات الميزات المؤقتة لـ SharePoint Online](https://aka.ms/ODSPAdjustments) للحصول على مزيد من المعلومات.</span><span class="sxs-lookup"><span data-stu-id="44f01-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="44f01-104">**مشاكل DLP مع أرقام passport الامريكيه/المملكة المتحدة**</span><span class="sxs-lookup"><span data-stu-id="44f01-104">**DLP issues with US/UK passport numbers**</span></span>

<span data-ttu-id="44f01-105">هل تواجه مشاكل متعلقة **بمنع فقدان البيانات (DLP)** لا تعمل علي المحتوي الذي يحتوي علي **رقم passport للولايات المتحدة/المملكة** المتحدة عند استخدام نوع المعلومات الحساسة ل DLP في O365 ؟</span><span class="sxs-lookup"><span data-stu-id="44f01-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US/UK passport number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="44f01-106">إذا كان الأمر كذلك ، فتاكد من ان المحتوي يحتوي علي المعلومات المطلوبة لما يبحث عنه نهج DLP عند تقييمه.</span><span class="sxs-lookup"><span data-stu-id="44f01-106">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="44f01-107">علي سبيل المثال ، بالنسبة إلى نهج **رقم passport للولايات المتحدة/المملكة** المتحدة المكون بمستوي الثقة في 75% ، يتم تقييم التالي ويجب الكشف عنه لكي يتم تشغيل القاعدة</span><span class="sxs-lookup"><span data-stu-id="44f01-107">For example, for a **US/UK passport number** policy configured with a confidence level of 75%, the following are evaluated and must be detected for the rule to trigger</span></span>
  
- <span data-ttu-id="44f01-108">**[تنسيق:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** تسعه أرقام</span><span class="sxs-lookup"><span data-stu-id="44f01-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Nine digits</span></span>

- <span data-ttu-id="44f01-109">**[النمط:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** تسعه أرقام متتالية</span><span class="sxs-lookup"><span data-stu-id="44f01-109">**[Pattern:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Nine consecutive digits</span></span>

- <span data-ttu-id="44f01-110">**[المجموع الاختباري:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** لا ، لا توجد مجموعات اختباريه</span><span class="sxs-lookup"><span data-stu-id="44f01-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="44f01-111">**[تعريف:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** نهج DLP هو 75% تثق بأنه قد تم اكتشاف هذا النوع من المعلومات الهامه في حال وجوده في غضون أكثر من 300 حرفا:</span><span class="sxs-lookup"><span data-stu-id="44f01-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="44f01-112">تعثر الدالة Func_usa_uk_passport علي المحتوي الذي يتطابق مع النمط.</span><span class="sxs-lookup"><span data-stu-id="44f01-112">The function Func_usa_uk_passport finds content that matches the pattern.</span></span>

  - <span data-ttu-id="44f01-113">تم العثور علي كلمه أساسيه من Keyword_passport.</span><span class="sxs-lookup"><span data-stu-id="44f01-113">A keyword from Keyword_passport is found.</span></span>

    <span data-ttu-id="44f01-114">علي سبيل المثال ، سيتم تشغيل النموذج التالي لسياسة **رقم passport الامريكيه/المملكة** المتحدة: رقم passport الأمريكي 123456789</span><span class="sxs-lookup"><span data-stu-id="44f01-114">For example, the following sample would trigger for the **US/UK passport number** policy: U.S. Passport number 123456789</span></span>

<span data-ttu-id="44f01-115">للحصول علي مزيد من المعلومات حول العناصر المطلوبة للحصول علي رقم Passport للولايات المتحدة/المملكة المتحدة ، راجع القسم التالي في هذه المقالة: [ما الذي تبحث عنه أنواع المعلومات الهامه لرقم الولايات المتحدة/المملكة المتحدة](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)</span><span class="sxs-lookup"><span data-stu-id="44f01-115">For more information on what is required for a US/UK Passport Number to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US/UK Passport Number](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)</span></span>
  
<span data-ttu-id="44f01-116">باستخدام نوع آخر من المعلومات الحساسة المضمنة ، راجع المقالة التالية للحصول علي معلومات حول ما هو مطلوب للأنواع الأخرى: [ما الذي تبحث عنه أنواع المعلومات الهامه](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="44f01-116">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  