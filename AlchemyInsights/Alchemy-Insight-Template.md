---
title: نفس اسم الملف الأفضل
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 4/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 5555
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: 68f743ee9c448565470815f8410cc6ce4b384bed
ms.sourcegitcommit: 0b6e9470c6b73616ba8bacef7010f739b7fac332
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/21/2019
ms.locfileid: "30742350"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="0eeac-102">لا تعمل المطلوبة خيمياء رأس H1، H2 الخاصة.</span><span class="sxs-lookup"><span data-stu-id="0eeac-102">Required Alchemy Header H1, H2's dont work.</span></span>
<span data-ttu-id="0eeac-103">أفضل الممارسات والمبادئ التوجيهية لكتابة "الكيمياء":</span><span class="sxs-lookup"><span data-stu-id="0eeac-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="0eeac-104">**عدم تداخل الأفكار "الكيمياء" في المجلدات**-سيؤدي هذا إلى قطع بنية عنوان url.</span><span class="sxs-lookup"><span data-stu-id="0eeac-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="0eeac-105">نحن نبحث في إصلاح ذلك.</span><span class="sxs-lookup"><span data-stu-id="0eeac-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="0eeac-106">يجب أن تحتوي ملفات في المجلد **التشيميينسايتس** أسماء الملفات الصغيرة مع وصلات لمسافات ex.</span><span class="sxs-lookup"><span data-stu-id="0eeac-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="0eeac-107">***كيف-تمكين-دعوى قضائية الاستمرار***.</span><span class="sxs-lookup"><span data-stu-id="0eeac-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="0eeac-108">تضمين معرف المستودع أو "معرف القاعدة" من [بوابة "الشركاء الكيمياء"](https://alchemyportal.azurewebsites.net) في الحقل ms.custom.</span><span class="sxs-lookup"><span data-stu-id="0eeac-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="0eeac-109">السابقين.</span><span class="sxs-lookup"><span data-stu-id="0eeac-109">ex.</span></span> <span data-ttu-id="0eeac-110">***ms.custom: 100021***</span><span class="sxs-lookup"><span data-stu-id="0eeac-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="0eeac-111">استخدم باقي البيانات الأولية في الجزء العلوي من هذا الملف كالقالب.</span><span class="sxs-lookup"><span data-stu-id="0eeac-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="0eeac-112">في [بوابة الشركاء "الكيمياء"](https://alchemyportal.azurewebsites.net)، انتقل إلى المقطع **"عنوان رؤية العميل":** واستخدام هذه النقطة كمنطلق للعنوان H1 للفكرة.</span><span class="sxs-lookup"><span data-stu-id="0eeac-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="0eeac-113">خيمياء رؤى يجب H1 واحدة فقط أعلى أو أنها سيؤدي في الإنتاج.</span><span class="sxs-lookup"><span data-stu-id="0eeac-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="0eeac-114">عدم تقديم H2s في هذه الحالة استخدام **غامق** أو اتفاقيات أخرى للدلالة على مقاطع منفصلة.</span><span class="sxs-lookup"><span data-stu-id="0eeac-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="0eeac-115">بعد ذلك، قم بملء نص استخدام مادة مشروع في قسم "آراء العملاء" من صفحة "الكيمياء" القواعد</span><span class="sxs-lookup"><span data-stu-id="0eeac-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="0eeac-116">قوائم ذات تعداد نقطي على ما يرام</span><span class="sxs-lookup"><span data-stu-id="0eeac-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="0eeac-117">قوائم ذات تعداد رقمي كبير جداً</span><span class="sxs-lookup"><span data-stu-id="0eeac-117">Numbered lists too</span></span>
    1. <span data-ttu-id="0eeac-118">**غامق** و *مائل* يتم أوك</span><span class="sxs-lookup"><span data-stu-id="0eeac-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="0eeac-119">ارتباطات يجب أن يكون أما **"ارتباطات ويب"/الخارجية** أو **ارتباطات عميق لعناصر واجهة المستخدم**والارتباطات الداخلية لا.</span><span class="sxs-lookup"><span data-stu-id="0eeac-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="0eeac-120">الصور غير معتمدة رسميا في هذا الوقت، ولكن كان على خارطة الطريق.</span><span class="sxs-lookup"><span data-stu-id="0eeac-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="0eeac-121">وهذا فعلا الفعل وقتاً طويلاً بعض الشيء.</span><span class="sxs-lookup"><span data-stu-id="0eeac-121">And this is really already a bit too long.</span></span> <span data-ttu-id="0eeac-122">أفضل ممارسة أحرف حوالي 400--</span><span class="sxs-lookup"><span data-stu-id="0eeac-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="0eeac-123">بمجرد المحتوى الخاص بك جاهز، تسحبه إلى الفرع مباشرة.</span><span class="sxs-lookup"><span data-stu-id="0eeac-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="0eeac-124">ثم انتقل إلى [بوابة الشركاء "الكيمياء"](https://alchemyportal.azurewebsites.net) وأدخل اسم الملف في الحقل.</span><span class="sxs-lookup"><span data-stu-id="0eeac-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> <span data-ttu-id="0eeac-125">M</span><span class="sxs-lookup"><span data-stu-id="0eeac-125">M</span></span>