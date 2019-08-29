---
title: إعداد DKIM في Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: dd908db6a4bc1739b3c1cff059387034d67e093d
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/29/2019
ms.locfileid: "36666251"
---
# <a name="setup-dkim-in-office-365"></a><span data-ttu-id="325d2-102">إعداد DKIM في Office 365</span><span class="sxs-lookup"><span data-stu-id="325d2-102">Setup DKIM in Office 365</span></span>

<span data-ttu-id="325d2-103">إرشادات كاملة حول تكوين DKIM للمجالات المخصصة في Office 365 [هنا](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="325d2-103">The complete instructions for configuring DKIM for custom domains in Office 365 are [here](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span></span>

1. <span data-ttu-id="325d2-104">**كل** مجال مخصص، تحتاج إلى إنشاء **جهازي** سجلات DKIM CNAME على المجال DNS خدمة استضافة (عادة، المسجل المجال).</span><span class="sxs-lookup"><span data-stu-id="325d2-104">For **each** custom domain, you need to create **two** DKIM CNAME records at your domain's DNS hosting service (typically, the domain registrar).</span></span> <span data-ttu-id="325d2-105">على سبيل المثال، تتطلب contoso.com و fourthcoffee.com أربعة سجلات DKIM CNAME: اثنان ل contoso.com واثنان من fourthcoffee.com.</span><span class="sxs-lookup"><span data-stu-id="325d2-105">For example, contoso.com and fourthcoffee.com require four DKIM CNAME records: two for contoso.com and two for fourthcoffee.com.</span></span>

   <span data-ttu-id="325d2-106">استخدام سجلات DKIM CNAME **كل** مجال مخصص التنسيقات التالية:</span><span class="sxs-lookup"><span data-stu-id="325d2-106">The DKIM CNAME records for **each** custom domain use the following formats:</span></span>

   - <span data-ttu-id="325d2-107">**اسم المضيف**:`selector1._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="325d2-107">**Host name**: `selector1._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="325d2-108">**يشير إلى عنوان أو القيمة**:`selector1-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="325d2-108">**Points to address or value**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="325d2-109">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="325d2-109">**TTL**: 3600</span></span>

   - <span data-ttu-id="325d2-110">**اسم المضيف**:`selector2._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="325d2-110">**Host name**: `selector2._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="325d2-111">**يشير إلى عنوان أو القيمة**:`selector2-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="325d2-111">**Points to address or value**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="325d2-112">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="325d2-112">**TTL**: 3600</span></span>

   <span data-ttu-id="325d2-113">\<DomainGUID\> النص إلى اليسار `.mail.protection.outlook.com` في السجل MX المخصصة للمجال المخصص (على سبيل المثال، `contoso-com` ل contoso.com المجال).</span><span class="sxs-lookup"><span data-stu-id="325d2-113">\<DomainGUID\> is the text to the left of `.mail.protection.outlook.com` in the customized MX record for the custom domain (for example, `contoso-com` for the domain contoso.com).</span></span> <span data-ttu-id="325d2-114">\<إينيتيالدومين\> هي المجال الذي تستخدمه عند اشتراكك في Office 365 (على سبيل المثال، contoso.onmicrosoft.com).</span><span class="sxs-lookup"><span data-stu-id="325d2-114">\<InitialDomain\> is the domain you used when you signed up for Office 365 (for example, contoso.onmicrosoft.com).</span></span>

2. <span data-ttu-id="325d2-115">بعد أن قمت بإنشاء سجلات CNAME للمجالات المخصصة الخاصة بك، أكمل الإرشادات التالية:</span><span class="sxs-lookup"><span data-stu-id="325d2-115">After you've created the CNAME records for your custom domains, complete the following instructions:</span></span>

   <span data-ttu-id="325d2-116">أ.</span><span class="sxs-lookup"><span data-stu-id="325d2-116">a.</span></span> <span data-ttu-id="325d2-117">[تسجيل الدخول إلى Office 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) باستخدام حسابك العمل أو المدرسة.</span><span class="sxs-lookup"><span data-stu-id="325d2-117">[Sign in to Office 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) with your work or school account.</span></span>

   <span data-ttu-id="325d2-118">(ب).</span><span class="sxs-lookup"><span data-stu-id="325d2-118">b.</span></span> <span data-ttu-id="325d2-119">حدد رمز التطبيق المشغل في الزاوية العليا اليسرى واختر **المسؤول**.</span><span class="sxs-lookup"><span data-stu-id="325d2-119">Select the app launcher icon in the upper-left and choose **Admin**.</span></span>

   <span data-ttu-id="325d2-120">(ج).</span><span class="sxs-lookup"><span data-stu-id="325d2-120">c.</span></span> <span data-ttu-id="325d2-121">في شريط التنقل الأيسر السفلي، قم بتوسيع **الإدارة** واختر **تبادل**.</span><span class="sxs-lookup"><span data-stu-id="325d2-121">In the lower-left navigation, expand **Admin** and choose **Exchange**.</span></span>

   <span data-ttu-id="325d2-122">(د).</span><span class="sxs-lookup"><span data-stu-id="325d2-122">d.</span></span> <span data-ttu-id="325d2-123">انتقل إلى **حماية** > **DKIM**.</span><span class="sxs-lookup"><span data-stu-id="325d2-123">Go to **Protection** > **DKIM**.</span></span>

   <span data-ttu-id="325d2-124">(ه).</span><span class="sxs-lookup"><span data-stu-id="325d2-124">e.</span></span> <span data-ttu-id="325d2-125">حدد المجال، ثم اختر **تمكين** **توقيع الرسائل لهذا المجال بتوقيعات DKIM**.</span><span class="sxs-lookup"><span data-stu-id="325d2-125">Select the domain and then choose **Enable** for **Sign messages for this domain with DKIM signatures**.</span></span> <span data-ttu-id="325d2-126">كرر هذه الخطوة لكل مجال مخصص.</span><span class="sxs-lookup"><span data-stu-id="325d2-126">Repeat this step for each custom domain.</span></span>
