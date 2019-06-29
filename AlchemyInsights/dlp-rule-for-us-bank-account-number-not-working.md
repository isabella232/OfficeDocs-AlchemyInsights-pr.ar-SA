---
title: قاعدة DLP "لنا رقم الحساب البنكي" لا يعمل
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: 83050b05cffacd3e81d34f05383c213eb0042fae
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/28/2019
ms.locfileid: "35389456"
---
<span data-ttu-id="97840-102">هل تواجه مشاكل في **منع فقدان البيانات (DLP)** لا يعمل للمحتوى الذي يحتوي على **رقم الحساب البنكي الولايات المتحدة** عند استخدام نوع معلومات حساسة DLP في O365؟</span><span class="sxs-lookup"><span data-stu-id="97840-102">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US Bank Account Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="97840-103">إذا كان الأمر كذلك، تأكد من أن المحتوى الخاص بك يحتوي على المعلومات المطلوبة لما نهج DLP تبحث عنه عندما يتم تقييم.</span><span class="sxs-lookup"><span data-stu-id="97840-103">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="97840-104">على سبيل المثال، لنهج **الولايات المتحدة رقم الحساب البنكي** الذي تم تكوينه بمستوى ثقة 85%، التالية يتم تقييمها ويجب الكشف عن لتشغيل القاعدة:</span><span class="sxs-lookup"><span data-stu-id="97840-104">For example, for a **US Bank Account Number** policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="97840-105">**[تنسيق:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** أرقام 8 17</span><span class="sxs-lookup"><span data-stu-id="97840-105">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 digits</span></span>

- <span data-ttu-id="97840-106">**[نمط:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** رقم 8-17 على التوالي.</span><span class="sxs-lookup"><span data-stu-id="97840-106">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 consecutive digits.</span></span>

- <span data-ttu-id="97840-107">**[المجموع الاختباري:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** لا، هناك لم المجموع الاختباري</span><span class="sxs-lookup"><span data-stu-id="97840-107">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="97840-108">**[تعريف:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** نهج DLP هي 75% واثقاً من الكشف عن هذا النوع من المعلومات الهامة إذا مسافة 300 حرف:</span><span class="sxs-lookup"><span data-stu-id="97840-108">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="97840-109">التعبير العادي Regex_usa_bank_account_number البحث عن المحتوى الذي يطابق نمط</span><span class="sxs-lookup"><span data-stu-id="97840-109">The regular expression Regex_usa_bank_account_number finds content that matches the pattern</span></span>

  - <span data-ttu-id="97840-110">تم العثور على كلمة أساسية من Keyword_usa_Bank_Account.</span><span class="sxs-lookup"><span data-stu-id="97840-110">A keyword from Keyword_usa_Bank_Account is found.</span></span>

    <span data-ttu-id="97840-111">على سبيل المثال، فسيتم تشغيل النموذج التالي للسياسة **الأمريكية رقم الحساب البنكي** : 78344011 التحقق من الحساب</span><span class="sxs-lookup"><span data-stu-id="97840-111">For example, the following sample would trigger for the **US Bank Account Number** policy: Checking Account 78344011</span></span>

<span data-ttu-id="97840-112">لمزيد من المعلومات حول ما هو مطلوب **رقم الحساب البنكي في الولايات المتحدة** بأن يتم كشفه للمحتوى، راجع المقطع التالي في هذا المقال: [ما الحساسة معلومات الأنواع ابحث عن "رقم الحساب البنكي في الولايات المتحدة"](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span><span class="sxs-lookup"><span data-stu-id="97840-112">For more information on what is required for a **US Bank Account Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US Bank Account Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span></span>
  
<span data-ttu-id="97840-113">استخدام نوع معلومات حساسة مضمنة مختلفة، راجع المقالة التالية للحصول على المعلومات على ما هو مطلوب للأنواع الأخرى: [البحث عن "ما الحساسة معلومات الأنواع"](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="97840-113">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  