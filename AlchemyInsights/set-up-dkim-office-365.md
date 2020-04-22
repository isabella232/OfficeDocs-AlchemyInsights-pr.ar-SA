---
title: إعداد DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: d23a816d4eef065f800eaee60829d57dc1e7177f
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/21/2020
ms.locfileid: "43645659"
---
# <a name="setup-dkim"></a><span data-ttu-id="4223d-102">إعداد DKIM</span><span class="sxs-lookup"><span data-stu-id="4223d-102">Setup DKIM</span></span>

<span data-ttu-id="4223d-103">الإرشادات الكاملة لتكوين DKIM للمجالات المخصصة في Microsoft 365 [هنا](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="4223d-103">The complete instructions for configuring DKIM for custom domains in Microsoft 365 are [here](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span></span>

1. <span data-ttu-id="4223d-104">**لكل** مجال مخصص، تحتاج إلى إنشاء **سجلين** DKIM CNAME في خدمة استضافة DNS الخاصة بنطاقك (عادةً، مسجل النطاق).</span><span class="sxs-lookup"><span data-stu-id="4223d-104">For **each** custom domain, you need to create **two** DKIM CNAME records at your domain's DNS hosting service (typically, the domain registrar).</span></span> <span data-ttu-id="4223d-105">على سبيل المثال، تتطلب contoso.com fourthcoffee.com أربعة سجلات DKIM CNAME: اثنان contoso.com واثنين fourthcoffee.com.</span><span class="sxs-lookup"><span data-stu-id="4223d-105">For example, contoso.com and fourthcoffee.com require four DKIM CNAME records: two for contoso.com and two for fourthcoffee.com.</span></span>

   <span data-ttu-id="4223d-106">تستخدم سجلات DKIM CNAME **لكل** مجال مخصص التنسيقات التالية:</span><span class="sxs-lookup"><span data-stu-id="4223d-106">The DKIM CNAME records for **each** custom domain use the following formats:</span></span>

   - <span data-ttu-id="4223d-107">**اسم المضيف:**`selector1._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="4223d-107">**Host name**: `selector1._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="4223d-108">**نقاط للعنوان أو القيمة:**`selector1-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="4223d-108">**Points to address or value**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="4223d-109">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="4223d-109">**TTL**: 3600</span></span>

   - <span data-ttu-id="4223d-110">**اسم المضيف:**`selector2._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="4223d-110">**Host name**: `selector2._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="4223d-111">**نقاط للعنوان أو القيمة:**`selector2-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="4223d-111">**Points to address or value**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="4223d-112">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="4223d-112">**TTL**: 3600</span></span>

   <span data-ttu-id="4223d-113">\<DomainGUID\> هو النص إلى `.mail.protection.outlook.com` اليسار في سجل MX المخصص للمجال المخصص `contoso-com` (على سبيل المثال، للمجال contoso.com).</span><span class="sxs-lookup"><span data-stu-id="4223d-113">\<DomainGUID\> is the text to the left of `.mail.protection.outlook.com` in the customized MX record for the custom domain (for example, `contoso-com` for the domain contoso.com).</span></span> <span data-ttu-id="4223d-114">\<Domain\> هو المجال الذي استخدمته عند الاشتراك في Microsoft 365 (على سبيل المثال، contoso.onmicrosoft.com).</span><span class="sxs-lookup"><span data-stu-id="4223d-114">\<InitialDomain\> is the domain you used when you signed up for Microsoft 365 (for example, contoso.onmicrosoft.com).</span></span>

2. <span data-ttu-id="4223d-115">بعد إنشاء سجلات CNAME للمجالات المخصصة، أكمل الإرشادات التالية:</span><span class="sxs-lookup"><span data-stu-id="4223d-115">After you've created the CNAME records for your custom domains, complete the following instructions:</span></span>

   <span data-ttu-id="4223d-116">أ.</span><span class="sxs-lookup"><span data-stu-id="4223d-116">a.</span></span> <span data-ttu-id="4223d-117">[تسجيل الدخول إلى Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) باستخدام حساب العمل أو المدرسة.</span><span class="sxs-lookup"><span data-stu-id="4223d-117">[sign in to Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) with your work or school account.</span></span>

   <span data-ttu-id="4223d-118">ب.</span><span class="sxs-lookup"><span data-stu-id="4223d-118">b.</span></span> <span data-ttu-id="4223d-119">حدد رمز قاذفة التطبيق في أعلى اليسار واختر **المسؤول**.</span><span class="sxs-lookup"><span data-stu-id="4223d-119">Select the app launcher icon in the upper-left and choose **Admin**.</span></span>

   <span data-ttu-id="4223d-120">ج.</span><span class="sxs-lookup"><span data-stu-id="4223d-120">c.</span></span> <span data-ttu-id="4223d-121">في التنقل السفلي الأيسر، قم بتوسيع **المسؤول** واختيار **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="4223d-121">In the lower-left navigation, expand **Admin** and choose **Exchange**.</span></span>

   <span data-ttu-id="4223d-122">د.</span><span class="sxs-lookup"><span data-stu-id="4223d-122">d.</span></span> <span data-ttu-id="4223d-123">انتقل إلى **حماية** > **DKIM**.</span><span class="sxs-lookup"><span data-stu-id="4223d-123">Go to **Protection** > **DKIM**.</span></span>

   <span data-ttu-id="4223d-124">ه.</span><span class="sxs-lookup"><span data-stu-id="4223d-124">e.</span></span> <span data-ttu-id="4223d-125">حدد المجال ثم اختر **تمكين** **رسائل التوقيع لهذا المجال مع توقيعات DKIM**.</span><span class="sxs-lookup"><span data-stu-id="4223d-125">Select the domain and then choose **Enable** for **Sign messages for this domain with DKIM signatures**.</span></span> <span data-ttu-id="4223d-126">كرر هذه الخطوة لكل مجال مخصص.</span><span class="sxs-lookup"><span data-stu-id="4223d-126">Repeat this step for each custom domain.</span></span>
