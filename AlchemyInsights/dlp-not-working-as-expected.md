---
title: لا يعمل كما هو متوقع DLP
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: 102c8025571f840cf64091d75295acec50661df2
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/22/2019
ms.locfileid: "36530266"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="067dc-102">لا يعمل كما هو متوقع DLP</span><span class="sxs-lookup"><span data-stu-id="067dc-102">DLP not working as expected</span></span>

<span data-ttu-id="067dc-103">هل تواجه مشاكل في **منع فقدان البيانات (DLP)** في Office 365 لا يعمل كما هو متوقع؟</span><span class="sxs-lookup"><span data-stu-id="067dc-103">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="067dc-104">إذا كان الأمر كذلك، تأكد من أن إعداد **نهج DLP** بشكل صحيح، وأن تحتوي على أي **نهج DLP** تبحث عن عندما يتم تقييم.</span><span class="sxs-lookup"><span data-stu-id="067dc-104">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
 <span data-ttu-id="067dc-105">**إعداد DLP**</span><span class="sxs-lookup"><span data-stu-id="067dc-105">**Setting up DLP**</span></span>
  
<span data-ttu-id="067dc-106">دلب نهج يسمح لك لتحديد وحماية المعلومات الحساسة في المؤسسة الخاصة بك.</span><span class="sxs-lookup"><span data-stu-id="067dc-106">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="067dc-107">لإعداد سياسات DLP، استخدم المعلومات [هنا](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span><span class="sxs-lookup"><span data-stu-id="067dc-107">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="067dc-108">**البحث عن ما هي السياسات DLP**</span><span class="sxs-lookup"><span data-stu-id="067dc-108">**What DLP policies look for**</span></span>
  
<span data-ttu-id="067dc-109">عند استخدام **أنواع المعلومات الحساسة المضمنة** في مركز Office 365 الأمان والتوافق، نهج DLP البحث عن نماذج معينة والعناصر عند اكتشاف هذه الأنواع الحساسة.</span><span class="sxs-lookup"><span data-stu-id="067dc-109">When using the **built-in sensitive information types** in Office 365 Security and Compliance center, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="067dc-110">**أنواع المعلومات الحساسة المضمنة**</span><span class="sxs-lookup"><span data-stu-id="067dc-110">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="067dc-111">لمزيد من المعلومات حول الأنواع الحساسة المضمنة وما نهج DLP يفتش عند الكشف عن نوع الحساسة، راجع: [البحث عن ما هي أنواع المعلومات الحساسة](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span><span class="sxs-lookup"><span data-stu-id="067dc-111">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="067dc-112">**أنواع المعلومات الهامة المخصصة**</span><span class="sxs-lookup"><span data-stu-id="067dc-112">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="067dc-113">إذا كنت تحاول إنشاء أنواع المعلومات الهامة المخصصة، استخدم المقالة التالية للحصول على معلومات حول كيفية إنشاء نوع مخصص حساسة: [إنشاء نوع مخصص من معلومات حساسة](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="067dc-113">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="067dc-114">**اختبار نهج DLP**</span><span class="sxs-lookup"><span data-stu-id="067dc-114">**Test a DLP policy**</span></span>

<span data-ttu-id="067dc-115">لاختبار البيانات باستخدام نوع معلومات حساسة مضمن أو مخصص، استخدم الخيار **نوع الاختبار** تحت **تصنيفات** > **أنواع المعلومات الحساسة**.</span><span class="sxs-lookup"><span data-stu-id="067dc-115">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="067dc-116">لمزيد من المعلومات، راجع [أنواع الاختبار المخصص معلومات حساسة](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span><span class="sxs-lookup"><span data-stu-id="067dc-116">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="067dc-117">**التقارير**</span><span class="sxs-lookup"><span data-stu-id="067dc-117">**Reports**</span></span>
  
- <span data-ttu-id="067dc-118">الحصول على بيانات حساسة مع رؤى [تقارير تقنية DLP.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="067dc-118">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="067dc-119">راجع التفاصيل الخاصة بالحدث [تقرير الحادث](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span><span class="sxs-lookup"><span data-stu-id="067dc-119">See specific details of the event with an [Incident Report](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span></span>
