---
title: مطابقة اسم الملف أفضل [# القاعدة-وصف]
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 4/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: e248c2ee3cbb9a86f21c1f36be10c893df76ff52
ms.sourcegitcommit: 3070905131e6d8449981231a3551c0bb4ca38ae6
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/14/2019
ms.locfileid: "30634491"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="aa7ca-102">لا تعمل المطلوبة خيمياء رأس H1، H2 الخاصة.</span><span class="sxs-lookup"><span data-stu-id="aa7ca-102">Required Alchemy Header H1, H2's dont work.</span></span>
<span data-ttu-id="aa7ca-103">أفضل الممارسات والمبادئ التوجيهية لكتابة "الكيمياء":</span><span class="sxs-lookup"><span data-stu-id="aa7ca-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="aa7ca-104">**عدم تداخل الأفكار "الكيمياء" في المجلدات**-سيؤدي هذا إلى قطع بنية عنوان url.</span><span class="sxs-lookup"><span data-stu-id="aa7ca-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="aa7ca-105">نحن نبحث في إصلاح ذلك.</span><span class="sxs-lookup"><span data-stu-id="aa7ca-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="aa7ca-106">يجب أن تحتوي ملفات في المجلد **التشيميينسايتس** قاعدة معرف واسم القاعدة من [بوابة الشركاء "الكيمياء"](https://alchemyportal.azurewebsites.net) في اسم الملف.</span><span class="sxs-lookup"><span data-stu-id="aa7ca-106">Files in the **AlchemyInsights** folder should have Rule ID and Rule Name from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the filename.</span></span>
    1. <span data-ttu-id="aa7ca-107">السابقين.</span><span class="sxs-lookup"><span data-stu-id="aa7ca-107">ex.</span></span> <span data-ttu-id="aa7ca-108">***976-How-to-enable-litigation-hold***</span><span class="sxs-lookup"><span data-stu-id="aa7ca-108">***976-How-to-enable-litigation-hold***</span></span>
1. <span data-ttu-id="aa7ca-109">استخدام بيانات التعريف في الجزء العلوي من هذا الملف كالقالب.</span><span class="sxs-lookup"><span data-stu-id="aa7ca-109">Use the metadata at the top of this file as your template.</span></span> <span data-ttu-id="aa7ca-110">لا شيء غير مطلوب.</span><span class="sxs-lookup"><span data-stu-id="aa7ca-110">Nothing else is required.</span></span>
1. <span data-ttu-id="aa7ca-111">في [بوابة الشركاء "الكيمياء"](https://alchemyportal.azurewebsites.net)، انتقل إلى المقطع **"عنوان رؤية العميل":** واستخدام هذه النقطة كمنطلق للعنوان H1 للفكرة.</span><span class="sxs-lookup"><span data-stu-id="aa7ca-111">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="aa7ca-112">خيمياء رؤى يجب H1 واحدة فقط أعلى أو أنها سيؤدي في الإنتاج.</span><span class="sxs-lookup"><span data-stu-id="aa7ca-112">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="aa7ca-113">عدم تقديم H2s في هذه الحالة استخدام **غامق** أو اتفاقيات أخرى للدلالة على مقاطع منفصلة.</span><span class="sxs-lookup"><span data-stu-id="aa7ca-113">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="aa7ca-114">بعد ذلك، قم بملء نص استخدام مادة مشروع في قسم "آراء العملاء" من صفحة "الكيمياء" القواعد</span><span class="sxs-lookup"><span data-stu-id="aa7ca-114">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="aa7ca-115">قوائم ذات تعداد نقطي على ما يرام</span><span class="sxs-lookup"><span data-stu-id="aa7ca-115">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="aa7ca-116">قوائم ذات تعداد رقمي كبير جداً</span><span class="sxs-lookup"><span data-stu-id="aa7ca-116">Numbered lists too</span></span>
    1. <span data-ttu-id="aa7ca-117">**غامق** و *مائل* يتم أوك</span><span class="sxs-lookup"><span data-stu-id="aa7ca-117">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="aa7ca-118">ارتباطات يجب أن يكون أما **"ارتباطات ويب"/الخارجية** أو **ارتباطات عميق لعناصر واجهة المستخدم**والارتباطات الداخلية لا.</span><span class="sxs-lookup"><span data-stu-id="aa7ca-118">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>

<span data-ttu-id="aa7ca-119">وهذا فعلا الفعل وقتاً طويلاً بعض الشيء.</span><span class="sxs-lookup"><span data-stu-id="aa7ca-119">And this is really already a bit too long.</span></span> <span data-ttu-id="aa7ca-120">أفضل ممارسة أحرف حوالي 400--</span><span class="sxs-lookup"><span data-stu-id="aa7ca-120">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="aa7ca-121">بمجرد المحتوى الخاص بك جاهز، تسحبه إلى الفرع مباشرة.</span><span class="sxs-lookup"><span data-stu-id="aa7ca-121">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="aa7ca-122">ثم انتقل إلى [بوابة الشركاء "الكيمياء"](https://alchemyportal.azurewebsites.net) وأدخل اسم الملف في الحقل.</span><span class="sxs-lookup"><span data-stu-id="aa7ca-122">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> <span data-ttu-id="aa7ca-123">تأكد من رؤية مراجعة ونشر تقول "نعم" وثم انقر فوق "تحديث القاعدة".</span><span class="sxs-lookup"><span data-stu-id="aa7ca-123">Make sure Insight reviewed and published says "yes" and then click Update Rule.</span></span> <span data-ttu-id="aa7ca-124">**(هذا سيبدو أجمل في الإصدار الجديد من المدخل-الإفراج قريبا.)** 
 ![حقل محدد موقع معلومات](media/for-content-team.PNG)</span><span class="sxs-lookup"><span data-stu-id="aa7ca-124">**(This will look prettier in the new version of the portal - releasing soon.)**
![url field](media/for-content-team.PNG)</span></span>

