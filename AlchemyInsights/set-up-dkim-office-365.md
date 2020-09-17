---
title: اعداد DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: b34bfdafcab6229a4dd2e9d9f23103fa13556482
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47808694"
---
# <a name="setup-dkim"></a><span data-ttu-id="73e6b-102">اعداد DKIM</span><span class="sxs-lookup"><span data-stu-id="73e6b-102">Setup DKIM</span></span>

<span data-ttu-id="73e6b-103">تتوفر الإرشادات الكاملة لتكوين العلامات الخاصة ب DKIM خاصه بالمجالات المخصصة في Microsoft 365 [هنا](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span><span class="sxs-lookup"><span data-stu-id="73e6b-103">The complete instructions for configuring DKIM for custom domains in Microsoft 365 are [here](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span></span>

1. <span data-ttu-id="73e6b-104">بالنسبة إلى **كل** مجال مخصص ، تحتاج إلى إنشاء **سجلي CNAME لوحدتي** الأشرف في خدمه استضافه DNS الخاصة بمجالك (عاده ما يكون مسجل المجال).</span><span class="sxs-lookup"><span data-stu-id="73e6b-104">For **each** custom domain, you need to create **two** DKIM CNAME records at your domain's DNS hosting service (typically, the domain registrar).</span></span> <span data-ttu-id="73e6b-105">علي سبيل المثال ، يتطلب contoso.com و fourthcoffee.com أربعه سجلات CNAME للحصول علي اليم: اثنين لcontoso.com واثنين لfourthcoffee.com.</span><span class="sxs-lookup"><span data-stu-id="73e6b-105">For example, contoso.com and fourthcoffee.com require four DKIM CNAME records: two for contoso.com and two for fourthcoffee.com.</span></span>

   <span data-ttu-id="73e6b-106">تستخدم سجلات "العلامات الأشرف" ل **dkim كل** مجال مخصص التنسيقات التالية:</span><span class="sxs-lookup"><span data-stu-id="73e6b-106">The DKIM CNAME records for **each** custom domain use the following formats:</span></span>

   - <span data-ttu-id="73e6b-107">**اسم المضيف**: `selector1._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="73e6b-107">**Host name**: `selector1._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="73e6b-108">**يشير إلى العنوان أو القيمة**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="73e6b-108">**Points to address or value**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="73e6b-109">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="73e6b-109">**TTL**: 3600</span></span>

   - <span data-ttu-id="73e6b-110">**اسم المضيف**: `selector2._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="73e6b-110">**Host name**: `selector2._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="73e6b-111">**يشير إلى العنوان أو القيمة**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="73e6b-111">**Points to address or value**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="73e6b-112">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="73e6b-112">**TTL**: 3600</span></span>

   <span data-ttu-id="73e6b-113">\<DomainGUID\> النص إلى اليمين `.mail.protection.outlook.com` في سجل MX المخصص للمجال المخصص (علي سبيل `contoso-com` المثال ، لمجال contoso.com).</span><span class="sxs-lookup"><span data-stu-id="73e6b-113">\<DomainGUID\> is the text to the left of `.mail.protection.outlook.com` in the customized MX record for the custom domain (for example, `contoso-com` for the domain contoso.com).</span></span> <span data-ttu-id="73e6b-114">\<InitialDomain\> هو المجال الذي استخدمته عند التسجيل في Microsoft 365 (علي سبيل المثال ، contoso.onmicrosoft.com).</span><span class="sxs-lookup"><span data-stu-id="73e6b-114">\<InitialDomain\> is the domain you used when you signed up for Microsoft 365 (for example, contoso.onmicrosoft.com).</span></span>

2. <span data-ttu-id="73e6b-115">بعد إنشاء سجلات CNAME للمجالات المخصصة ، أكمل الإرشادات التالية:</span><span class="sxs-lookup"><span data-stu-id="73e6b-115">After you've created the CNAME records for your custom domains, complete the following instructions:</span></span>

   <span data-ttu-id="73e6b-116">علي.</span><span class="sxs-lookup"><span data-stu-id="73e6b-116">a.</span></span> <span data-ttu-id="73e6b-117">[سجل دخولك إلى Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) باستخدام حساب العمل أو المؤسسة التعليمية.</span><span class="sxs-lookup"><span data-stu-id="73e6b-117">[sign in to Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) with your work or school account.</span></span>

   <span data-ttu-id="73e6b-118">ب.</span><span class="sxs-lookup"><span data-stu-id="73e6b-118">b.</span></span> <span data-ttu-id="73e6b-119">حدد أيقونه مشغل التطبيق في الزاوية العلوية اليمني واختر **المسؤول**.</span><span class="sxs-lookup"><span data-stu-id="73e6b-119">Select the app launcher icon in the upper-left and choose **Admin**.</span></span>

   <span data-ttu-id="73e6b-120">ن.</span><span class="sxs-lookup"><span data-stu-id="73e6b-120">c.</span></span> <span data-ttu-id="73e6b-121">في جزء التنقل السفلي الأيمن ، قم بتوسيع **المسؤول** واختر **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="73e6b-121">In the lower-left navigation, expand **Admin** and choose **Exchange**.</span></span>

   <span data-ttu-id="73e6b-122">ثلاثي.</span><span class="sxs-lookup"><span data-stu-id="73e6b-122">d.</span></span> <span data-ttu-id="73e6b-123">انتقل إلى **حماية**  >  **dkim**.</span><span class="sxs-lookup"><span data-stu-id="73e6b-123">Go to **Protection** > **DKIM**.</span></span>

   <span data-ttu-id="73e6b-124">ه.</span><span class="sxs-lookup"><span data-stu-id="73e6b-124">e.</span></span> <span data-ttu-id="73e6b-125">حدد المجال ، ثم اختر **تمكين** **التوقيع علي الرسائل لهذا المجال بواسطة التواقيع التي تضم اليم إلى dkim**</span><span class="sxs-lookup"><span data-stu-id="73e6b-125">Select the domain and then choose **Enable** for **Sign messages for this domain with DKIM signatures**.</span></span> <span data-ttu-id="73e6b-126">كرر هذه الخطوة لكل مجال مخصص.</span><span class="sxs-lookup"><span data-stu-id="73e6b-126">Repeat this step for each custom domain.</span></span>
