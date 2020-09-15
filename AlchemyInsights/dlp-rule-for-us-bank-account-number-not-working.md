---
title: قاعده DLP لرقم حساب مصرفي الولايات المتحدة لا يعمل
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
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: eb399e4b23de32a757562833ed32d97daa6a1247
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679283"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a><span data-ttu-id="958ea-102">مشاكل DLP مع أرقام الحسابات المصرفية في الولايات المتحدة</span><span class="sxs-lookup"><span data-stu-id="958ea-102">DLP issues with US bank account numbers</span></span>

<span data-ttu-id="958ea-103">**هام**: خلال هذه الأوقات غير المسبوقة، نقوم باتخاذ الخطوات اللازمة لضمان توفر خدمات SharePoint Online و OneDrive بشكل كبير – الرجاء زيارة [تعديلات الميزات المؤقتة لـ SharePoint Online](https://aka.ms/ODSPAdjustments) للحصول على مزيد من المعلومات.</span><span class="sxs-lookup"><span data-stu-id="958ea-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="958ea-104">**مشاكل DLP مع أرقام الحسابات المصرفية في الولايات المتحدة**</span><span class="sxs-lookup"><span data-stu-id="958ea-104">**DLP issues with US bank account numbers**</span></span>

<span data-ttu-id="958ea-105">هل تواجه مشاكل متعلقة **بمنع فقدان البيانات (DLP)** لا تعمل علي المحتوي الذي يحتوي علي **رقم حساب مصرفي للولايات** المتحدة عند استخدام نوع المعلومات الحساسة ل DLP في O365 ؟</span><span class="sxs-lookup"><span data-stu-id="958ea-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US Bank Account Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="958ea-106">إذا كان الأمر كذلك ، فتاكد من ان المحتوي يحتوي علي المعلومات المطلوبة لما يبحث عنه نهج DLP عند تقييمه.</span><span class="sxs-lookup"><span data-stu-id="958ea-106">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="958ea-107">علي سبيل المثال ، بالنسبة لنهج **رقم حساب مصرفي للولايات** المتحدة تم تكوينه باستخدام مستوي الثقة في 85% ، يتم تقييم التالي ويجب الكشف عنه لكي يتم تشغيل القاعدة:</span><span class="sxs-lookup"><span data-stu-id="958ea-107">For example, for a **US Bank Account Number** policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="958ea-108">**[التنسيق:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 أرقام</span><span class="sxs-lookup"><span data-stu-id="958ea-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 digits</span></span>

- <span data-ttu-id="958ea-109">**[النمط:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 أرقاما متتالية.</span><span class="sxs-lookup"><span data-stu-id="958ea-109">**[Pattern:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 consecutive digits.</span></span>

- <span data-ttu-id="958ea-110">**[المجموع الاختباري:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** لا ، لا توجد مجموعات اختباريه</span><span class="sxs-lookup"><span data-stu-id="958ea-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="958ea-111">**[تعريف:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** نهج DLP هو 75% تثق بأنه قد تم اكتشاف هذا النوع من المعلومات الهامه في حال وجوده في غضون أكثر من 300 حرفا:</span><span class="sxs-lookup"><span data-stu-id="958ea-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="958ea-112">يبحث التعبير العادي Regex_usa_bank_account_number عن المحتوي الذي يتطابق مع النمط</span><span class="sxs-lookup"><span data-stu-id="958ea-112">The regular expression Regex_usa_bank_account_number finds content that matches the pattern</span></span>

  - <span data-ttu-id="958ea-113">تم العثور علي كلمه أساسيه من Keyword_usa_Bank_Account.</span><span class="sxs-lookup"><span data-stu-id="958ea-113">A keyword from Keyword_usa_Bank_Account is found.</span></span>

    <span data-ttu-id="958ea-114">علي سبيل المثال ، سيتم تشغيل النموذج التالي لنهج **رقم الحساب المصرفي للولايات** المتحدة: التحقق من الحساب 78344011</span><span class="sxs-lookup"><span data-stu-id="958ea-114">For example, the following sample would trigger for the **US Bank Account Number** policy: Checking Account 78344011</span></span>

<span data-ttu-id="958ea-115">للحصول علي مزيد من المعلومات حول ما هو مطلوب للحصول علي **رقم حساب مصرفي للولايات** المتحدة ، راجع القسم التالي في هذه المقالة: [ما الذي تبحث عنه أنواع المعلومات الهامه لرقم الحساب المصرفي الأمريكي](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)</span><span class="sxs-lookup"><span data-stu-id="958ea-115">For more information on what is required for a **US Bank Account Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US Bank Account Number](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)</span></span>
  
<span data-ttu-id="958ea-116">باستخدام نوع آخر من المعلومات الحساسة المضمنة ، راجع المقالة التالية للحصول علي معلومات حول ما هو مطلوب للأنواع الأخرى: [ما الذي تبحث عنه أنواع المعلومات الهامه](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="958ea-116">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  