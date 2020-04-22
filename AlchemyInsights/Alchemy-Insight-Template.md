---
title: نفس اسم الملف هو الأفضل
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: e2dcca1295e37007593b34c2d818ad1d1133e4a1
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43676520"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="3266f-102">مطلوب الكيمياء رأس H1، H2 لا تعمل.</span><span class="sxs-lookup"><span data-stu-id="3266f-102">Required Alchemy Header H1, H2's dont work.</span></span>
<span data-ttu-id="3266f-103">أفضل الممارسات والمبادئ التوجيهية لتأليف الكيمياء:</span><span class="sxs-lookup"><span data-stu-id="3266f-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="3266f-104">**لا عش الرؤى خيمياء في المجلدات**-- وهذا سوف كسر بنية رابط.</span><span class="sxs-lookup"><span data-stu-id="3266f-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="3266f-105">نحن نبحث في إصلاح هذا.</span><span class="sxs-lookup"><span data-stu-id="3266f-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="3266f-106">يجب أن تحتوي الملفات الموجودة في مجلد **AlchemyInsights** على أسماء ملفات صغيرة مع واصلات للمسافات السابقة.</span><span class="sxs-lookup"><span data-stu-id="3266f-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="3266f-107">***كيفية تمكين التقاضي - عقد.***</span><span class="sxs-lookup"><span data-stu-id="3266f-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="3266f-108">قم بتضمين معرف القاعدة أو معرف الدلو من [بوابة شريك الكيمياء](https://alchemyportal.azurewebsites.net) في الحقل ms.custom.</span><span class="sxs-lookup"><span data-stu-id="3266f-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="3266f-109">السابقين.</span><span class="sxs-lookup"><span data-stu-id="3266f-109">ex.</span></span> <span data-ttu-id="3266f-110">***ms.custom: 100021***</span><span class="sxs-lookup"><span data-stu-id="3266f-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="3266f-111">استخدم بقية بيانات التعريف في أعلى هذا الملف كقالب.</span><span class="sxs-lookup"><span data-stu-id="3266f-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="3266f-112">في [بوابة شريك الكيمياء](https://alchemyportal.azurewebsites.net)، انتقل لأسفل إلى قسم **عنوان رؤية العملاء:** واستخدم ذلك كنقطة انطلاق لعنوان H1 للرؤية.</span><span class="sxs-lookup"><span data-stu-id="3266f-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="3266f-113">الخيمياء رؤى يجب أن يكون فقط H1 واحد في الجزء العلوي أو أنها سوف كسر في الإنتاج.</span><span class="sxs-lookup"><span data-stu-id="3266f-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="3266f-114">H2s لا تجعل إما استخدام **جريئة** أو غيرها من الاتفاقيات للدلالة على أقسام منفصلة.</span><span class="sxs-lookup"><span data-stu-id="3266f-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="3266f-115">بعد ذلك، قم بتعبئة نص النص الأساسي باستخدام مسودة المواد في قسم رؤى العملاء في صفحة قاعدة الكيمياء</span><span class="sxs-lookup"><span data-stu-id="3266f-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="3266f-116">القوائم النقطية على ما يرام</span><span class="sxs-lookup"><span data-stu-id="3266f-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="3266f-117">قوائم مرقمة أيضًا</span><span class="sxs-lookup"><span data-stu-id="3266f-117">Numbered lists too</span></span>
    1. <span data-ttu-id="3266f-118">**جريئة** *ومائلة* هي أ ك</span><span class="sxs-lookup"><span data-stu-id="3266f-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="3266f-119">يجب أن تكون الروابط دائمًا **إما "روابط إلى الويب" / روابط خارجية** أو عميقة بعناصر واجهة **المستخدم**، وليس الروابط الداخلية.</span><span class="sxs-lookup"><span data-stu-id="3266f-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="3266f-120">لا يتم دعم الصور رسميًا في هذا الوقت ، ولكنها على خارطة الطريق.</span><span class="sxs-lookup"><span data-stu-id="3266f-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="3266f-121">وهذا هو حقا بالفعل قليلا طويلة جدا.</span><span class="sxs-lookup"><span data-stu-id="3266f-121">And this is really already a bit too long.</span></span> <span data-ttu-id="3266f-122">أفضل الممارسات حوالي 400 حرف ---------------------------------</span><span class="sxs-lookup"><span data-stu-id="3266f-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="3266f-123">بمجرد أن يكون المحتوى الخاص بك جاهزًا، اسحبه إلى الفرع المباشر.</span><span class="sxs-lookup"><span data-stu-id="3266f-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="3266f-124">ثم انتقل إلى [بوابة شريك الكيمياء](https://alchemyportal.azurewebsites.net) وأدخل اسم الملف في حقل رابط.</span><span class="sxs-lookup"><span data-stu-id="3266f-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> 