---
title: قاعدة DLP لرقم الحساب المصرفي الأمريكي لا يعمل
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: b032a7c80e8b387114aeda95c4f6af7e57225517
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507321"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a><span data-ttu-id="064f4-102">إصدارات DLP مع أرقام الحسابات المصرفية في الولايات المتحدة</span><span class="sxs-lookup"><span data-stu-id="064f4-102">DLP issues with US bank account numbers</span></span>

<span data-ttu-id="064f4-103">**هام**: خلال هذه الأوقات غير المسبوقة، نقوم باتخاذ الخطوات اللازمة لضمان توفر خدمات SharePoint Online و OneDrive بشكل كبير – الرجاء زيارة [تعديلات الميزات المؤقتة لـ SharePoint Online](https://aka.ms/ODSPAdjustments) للحصول على مزيد من المعلومات.</span><span class="sxs-lookup"><span data-stu-id="064f4-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="064f4-104">**إصدارات DLP مع أرقام الحسابات المصرفية في الولايات المتحدة**</span><span class="sxs-lookup"><span data-stu-id="064f4-104">**DLP issues with US bank account numbers**</span></span>

<span data-ttu-id="064f4-105">هل تواجه مشاكل مع **منع فقدان البيانات (DLP)** لا تعمل للمحتوى الذي يحتوي على **رقم حساب مصرفي في الولايات المتحدة** عند استخدام نوع معلومات حساسة DLP في O365؟</span><span class="sxs-lookup"><span data-stu-id="064f4-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US Bank Account Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="064f4-106">إذا كان الأمر كذلك، تأكد من أن المحتوى الخاص بك يحتوي على المعلومات المطلوبة لما تبحث عنه سياسة DLP عند تقييمه.</span><span class="sxs-lookup"><span data-stu-id="064f4-106">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="064f4-107">على سبيل المثال، بالنسبة لسياسة **رقم الحساب المصرفي الأمريكي** التي تم تكوينها بمستوى ثقة 85%، يتم تقييم ما يلي ويجب الكشف عنها حتى تقوم القاعدة بتشغيلها:</span><span class="sxs-lookup"><span data-stu-id="064f4-107">For example, for a **US Bank Account Number** policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="064f4-108">**[الشكل:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 أرقام</span><span class="sxs-lookup"><span data-stu-id="064f4-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 digits</span></span>

- <span data-ttu-id="064f4-109">**[النمط:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 أرقام متتالية.</span><span class="sxs-lookup"><span data-stu-id="064f4-109">**[Pattern:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 consecutive digits.</span></span>

- <span data-ttu-id="064f4-110">**[المجموع الاختياري:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** لا، لا يوجد المجموع الاختياري</span><span class="sxs-lookup"><span data-stu-id="064f4-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="064f4-111">**[التعريف:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** سياسة DLP واثقة بنسبة 75٪ من أنها اكتشفت هذا النوع من المعلومات الحساسة إذا، على مقربة من 300 حرف:</span><span class="sxs-lookup"><span data-stu-id="064f4-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="064f4-112">Regex_usa_bank_account_number التعبير العادي يبحث عن المحتوى الذي يطابق النمط</span><span class="sxs-lookup"><span data-stu-id="064f4-112">The regular expression Regex_usa_bank_account_number finds content that matches the pattern</span></span>

  - <span data-ttu-id="064f4-113">تم العثور على كلمة رئيسية من Keyword_usa_Bank_Account.</span><span class="sxs-lookup"><span data-stu-id="064f4-113">A keyword from Keyword_usa_Bank_Account is found.</span></span>

    <span data-ttu-id="064f4-114">على سبيل المثال، سيتم تشغيل العينة التالية لسياسة **رقم الحساب المصرفي الأمريكي:** التحقق من الحساب 78344011</span><span class="sxs-lookup"><span data-stu-id="064f4-114">For example, the following sample would trigger for the **US Bank Account Number** policy: Checking Account 78344011</span></span>

<span data-ttu-id="064f4-115">لمزيد من المعلومات حول ما هو مطلوب للكشف عن **رقم الحساب المصرفي الأمريكي** للمحتوى الخاص بك، راجع القسم التالي في هذه المقالة: ما أنواع المعلومات [الحساسة البحث عن رقم الحساب المصرفي الأمريكي](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)</span><span class="sxs-lookup"><span data-stu-id="064f4-115">For more information on what is required for a **US Bank Account Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US Bank Account Number](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)</span></span>
  
<span data-ttu-id="064f4-116">باستخدام نوع معلومات حساسة مضمن ة مختلفة، راجع المقالة التالية للحصول على معلومات حول ما هو مطلوب للأنواع الأخرى: [ما تبحث عنه أنواع المعلومات الحساسة](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="064f4-116">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  