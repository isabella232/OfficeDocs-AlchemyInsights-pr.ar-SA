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
ms.openlocfilehash: bd2901580acdb1dc17f3e14a7a9356b07e70f910
ms.sourcegitcommit: bf6a0e80d09aebae19b9e993c2552b88e49177c9
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/16/2020
ms.locfileid: "44750957"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="67776-102">"مطلوب الكيمياء رأس H1، H2 لا تعمل."</span><span class="sxs-lookup"><span data-stu-id="67776-102">"Required Alchemy Header H1, H2's dont work."</span></span>
<span data-ttu-id="67776-103">أفضل الممارسات والمبادئ التوجيهية لتألّف الخيميائي:</span><span class="sxs-lookup"><span data-stu-id="67776-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="67776-104">**لا تعشش "أفكار الخيمياء" في المجلدات**- وهذا سوف يكسر بنية رابط.</span><span class="sxs-lookup"><span data-stu-id="67776-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="67776-105">نحن نبحث في إصلاح هذا.</span><span class="sxs-lookup"><span data-stu-id="67776-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="67776-106">يجب أن يكون للملفات الموجودة في مجلد **AlchemyInsights** أسماء ملفات صغيرة مع واصلات لمساحات ex.</span><span class="sxs-lookup"><span data-stu-id="67776-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="67776-107">***كيف لتمكين التقاضي عقد***.</span><span class="sxs-lookup"><span data-stu-id="67776-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="67776-108">قم بتضمين معرف القاعدة أو معرف المستودع من [مدخل "شريك الخيمياء"](https://alchemyportal.azurewebsites.net) في حقل ms.custom.</span><span class="sxs-lookup"><span data-stu-id="67776-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="67776-109">السابقين.</span><span class="sxs-lookup"><span data-stu-id="67776-109">ex.</span></span> <span data-ttu-id="67776-110">***ms.custom: 100021***</span><span class="sxs-lookup"><span data-stu-id="67776-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="67776-111">استخدم بقية بيانات التعريف في أعلى هذا الملف كقالب.</span><span class="sxs-lookup"><span data-stu-id="67776-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="67776-112">في [بوابة شريك الخيمياء](https://alchemyportal.azurewebsites.net)، انتقل لأسفل إلى قسم **عنوان إحصاءات العملاء:** واستخدم ذلك كنقطة انطلاق لعنوان H1 الخاص بك للحصول على البصيرة.</span><span class="sxs-lookup"><span data-stu-id="67776-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="67776-113">يجب أن تكون "الرؤى الخيميائي" واحدة فقط H1 في الأعلى أو أنها سوف كسر في الإنتاج.</span><span class="sxs-lookup"><span data-stu-id="67776-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="67776-114">H2s لا تجعل إما استخدام **جريئة** أو غيرها من الاتفاقيات للدلالة على أقسام منفصلة.</span><span class="sxs-lookup"><span data-stu-id="67776-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="67776-115">بعد ذلك، قم بملء النص الأساسي باستخدام مسودة المواد في قسم رؤى العملاء في صفحة قاعدة الخيميائي</span><span class="sxs-lookup"><span data-stu-id="67776-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="67776-116">القوائم النقطية على ما يرام</span><span class="sxs-lookup"><span data-stu-id="67776-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="67776-117">القوائم المرقمة أيضاً</span><span class="sxs-lookup"><span data-stu-id="67776-117">Numbered lists too</span></span>
    1. <span data-ttu-id="67776-118">**جريئة** *ومليئة* هي على ما يرام</span><span class="sxs-lookup"><span data-stu-id="67776-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="67776-119">يجب أن تكون الروابط دائما إما **"وصلات إلى شبكة الإنترنت" / الخارجية** أو **روابط عميقة لعناصر واجهة المستخدم**، وليس الروابط الداخلية.</span><span class="sxs-lookup"><span data-stu-id="67776-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="67776-120">الصور غير مدعومة رسميا في هذا الوقت، لكنها على خارطة الطريق.</span><span class="sxs-lookup"><span data-stu-id="67776-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="67776-121">وهذا هو بالفعل قليلا طويلة جدا.</span><span class="sxs-lookup"><span data-stu-id="67776-121">And this is really already a bit too long.</span></span> <span data-ttu-id="67776-122">أفضل الممارسات حوالي 400 حرف ---------------------------------</span><span class="sxs-lookup"><span data-stu-id="67776-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="67776-123">بمجرد أن يصبح المحتوى جاهزًا، اسحبه إلى الفرع المباشر.</span><span class="sxs-lookup"><span data-stu-id="67776-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="67776-124">ثم انتقل إلى [بوابة شريك الخيمياء](https://alchemyportal.azurewebsites.net) وأدخل اسم الملف في حقل URL.</span><span class="sxs-lookup"><span data-stu-id="67776-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> 