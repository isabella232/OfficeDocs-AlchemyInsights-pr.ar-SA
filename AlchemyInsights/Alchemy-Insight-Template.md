---
title: نفس اسم الملف هو أفضل
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 4/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: 31a578800468e9f3a69fff4f6e2e1945943c779c
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/25/2019
ms.locfileid: "35800032"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="5d5be-102">مطلوب الكيمياء راس H1 ، H2's لا تعمل.</span><span class="sxs-lookup"><span data-stu-id="5d5be-102">Required Alchemy Header H1, H2's dont work.</span></span>
<span data-ttu-id="5d5be-103">أفضل الممارسات والمبادئ التوجيهية لتاليف الكيمياء:</span><span class="sxs-lookup"><span data-stu-id="5d5be-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="5d5be-104">**لا تتداخل رؤى الكيمياء في المجلدات**-وهذا سوف كسر بنيه url.</span><span class="sxs-lookup"><span data-stu-id="5d5be-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="5d5be-105">نحن نبحث في إصلاح هذا.</span><span class="sxs-lookup"><span data-stu-id="5d5be-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="5d5be-106">يجب ان تحتوي الملفات الموجودة في المجلد **التشيميينسايتس** علي أسماء أحرف صغيره مع واصلات للمساحات السابقة.</span><span class="sxs-lookup"><span data-stu-id="5d5be-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="5d5be-107">***كيفيه تمكين-التقاضي-عقد***.</span><span class="sxs-lookup"><span data-stu-id="5d5be-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="5d5be-108">تضمين معرف القاعدة أو معرف المستودع من [مدخل شريك الكيمياء](https://alchemyportal.azurewebsites.net) في الحقل المخصص ل ms.</span><span class="sxs-lookup"><span data-stu-id="5d5be-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="5d5be-109">السابقين.</span><span class="sxs-lookup"><span data-stu-id="5d5be-109">ex.</span></span> <span data-ttu-id="5d5be-110">***السيدة المخصصة: 100021***</span><span class="sxs-lookup"><span data-stu-id="5d5be-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="5d5be-111">استخدم بقية بيانات التعريف في اعلي هذا الملف كقالب.</span><span class="sxs-lookup"><span data-stu-id="5d5be-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="5d5be-112">في [بوابه شريك الكيمياء](https://alchemyportal.azurewebsites.net)، انتقل لأسفل إلى **عنوان رؤية العميل** القسم: واستخدم ذلك كنقطه انطلاق لعنوان H1 الخاص بك للحصول علي البصيرة.</span><span class="sxs-lookup"><span data-stu-id="5d5be-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="5d5be-113">يجب ان يكون لديك رؤى الكيمياء فقط H1 واحد في الأعلى أو انها سوف كسر في الإنتاج.</span><span class="sxs-lookup"><span data-stu-id="5d5be-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="5d5be-114">H2s لا تجعل اما استخدام **غامق** أو اصطلاحات أخرى للدلالة علي أقسام منفصلة.</span><span class="sxs-lookup"><span data-stu-id="5d5be-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="5d5be-115">بعد ذلك ، أملا النص الأساسي باستخدام مسودة المادة في قسم رؤى العملاء في صفحه قاعده الكيمياء</span><span class="sxs-lookup"><span data-stu-id="5d5be-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="5d5be-116">القوائم النقطية جيده</span><span class="sxs-lookup"><span data-stu-id="5d5be-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="5d5be-117">القوائم المرقمة أيضا</span><span class="sxs-lookup"><span data-stu-id="5d5be-117">Numbered lists too</span></span>
    1. <span data-ttu-id="5d5be-118">**غامق** *ومائل* هي-موافق</span><span class="sxs-lookup"><span data-stu-id="5d5be-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="5d5be-119">يجب ان تكون الارتباطات دائما اما **"ارتباطات إلى ويب"/الخارجية** أو **الارتباطات العميقة إلى عناصر واجهه المستخدم**، وليس الارتباطات الداخلية.</span><span class="sxs-lookup"><span data-stu-id="5d5be-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="5d5be-120">لا يتم دعم الصور رسميا في هذا الوقت ، ولكنها علي خريطة الطريق.</span><span class="sxs-lookup"><span data-stu-id="5d5be-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="5d5be-121">وهذا هو حقا بالفعل طويلا قليلا.</span><span class="sxs-lookup"><span data-stu-id="5d5be-121">And this is really already a bit too long.</span></span> <span data-ttu-id="5d5be-122">أفضل الممارسات حوالي 400 حرفا---------------------------------</span><span class="sxs-lookup"><span data-stu-id="5d5be-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="5d5be-123">بمجرد ان يكون المحتوي جاهزا ، اسحبه إلى الفرع المباشر.</span><span class="sxs-lookup"><span data-stu-id="5d5be-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="5d5be-124">ثم ، انتقل إلى [بوابه شريك الكيمياء](https://alchemyportal.azurewebsites.net) وادخل اسم الملف في حقل url.</span><span class="sxs-lookup"><span data-stu-id="5d5be-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> 