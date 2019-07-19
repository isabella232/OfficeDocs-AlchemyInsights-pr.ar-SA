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
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: b77e514da36701808d46248e8f2a45137751a1c7
ms.sourcegitcommit: 5447031f9d0a320c49897b8adb5d29ac9437fbc5
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 07/18/2019
ms.locfileid: "35786400"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="10b91-102">لا تعمل المطلوبة خيمياء رأس H1، H2 الخاصة.</span><span class="sxs-lookup"><span data-stu-id="10b91-102">Required Alchemy Header H1, H2's dont work.</span></span>
<span data-ttu-id="10b91-103">أفضل الممارسات والمبادئ التوجيهية لكتابة "الكيمياء":</span><span class="sxs-lookup"><span data-stu-id="10b91-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="10b91-104">**عدم تداخل الأفكار "الكيمياء" في المجلدات**-سيؤدي هذا إلى قطع بنية عنوان url.</span><span class="sxs-lookup"><span data-stu-id="10b91-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="10b91-105">نحن نبحث في إصلاح ذلك.</span><span class="sxs-lookup"><span data-stu-id="10b91-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="10b91-106">يجب أن تحتوي ملفات في المجلد **التشيميينسايتس** أسماء الملفات الصغيرة مع وصلات لمسافات ex.</span><span class="sxs-lookup"><span data-stu-id="10b91-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="10b91-107">***كيف-تمكين-دعوى قضائية الاستمرار***.</span><span class="sxs-lookup"><span data-stu-id="10b91-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="10b91-108">تضمين معرف المستودع أو "معرف القاعدة" من [بوابة "الشركاء الكيمياء"](https://alchemyportal.azurewebsites.net) في الحقل ms.custom.</span><span class="sxs-lookup"><span data-stu-id="10b91-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="10b91-109">السابقين.</span><span class="sxs-lookup"><span data-stu-id="10b91-109">ex.</span></span> <span data-ttu-id="10b91-110">***ms.custom: 100021***</span><span class="sxs-lookup"><span data-stu-id="10b91-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="10b91-111">استخدم باقي البيانات الأولية في الجزء العلوي من هذا الملف كالقالب.</span><span class="sxs-lookup"><span data-stu-id="10b91-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="10b91-112">في [بوابة الشركاء "الكيمياء"](https://alchemyportal.azurewebsites.net)، انتقل إلى المقطع **"عنوان رؤية العميل":** واستخدام هذه النقطة كمنطلق للعنوان H1 للفكرة.</span><span class="sxs-lookup"><span data-stu-id="10b91-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="10b91-113">خيمياء رؤى يجب H1 واحدة فقط أعلى أو أنها سيؤدي في الإنتاج.</span><span class="sxs-lookup"><span data-stu-id="10b91-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="10b91-114">عدم تقديم H2s في هذه الحالة استخدام **غامق** أو اتفاقيات أخرى للدلالة على مقاطع منفصلة.</span><span class="sxs-lookup"><span data-stu-id="10b91-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="10b91-115">بعد ذلك، قم بملء نص استخدام مادة مشروع في قسم "آراء العملاء" من صفحة "الكيمياء" القواعد</span><span class="sxs-lookup"><span data-stu-id="10b91-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="10b91-116">قوائم ذات تعداد نقطي على ما يرام</span><span class="sxs-lookup"><span data-stu-id="10b91-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="10b91-117">قوائم ذات تعداد رقمي كبير جداً</span><span class="sxs-lookup"><span data-stu-id="10b91-117">Numbered lists too</span></span>
    1. <span data-ttu-id="10b91-118">**غامق** و *مائل* يتم أوك</span><span class="sxs-lookup"><span data-stu-id="10b91-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="10b91-119">ارتباطات يجب أن يكون أما **"ارتباطات ويب"/الخارجية** أو **ارتباطات عميق لعناصر واجهة المستخدم**والارتباطات الداخلية لا.</span><span class="sxs-lookup"><span data-stu-id="10b91-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="10b91-120">الصور غير معتمدة رسميا في هذا الوقت، ولكن كان على خارطة الطريق.</span><span class="sxs-lookup"><span data-stu-id="10b91-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="10b91-121">وهذا فعلا الفعل وقتاً طويلاً بعض الشيء.</span><span class="sxs-lookup"><span data-stu-id="10b91-121">And this is really already a bit too long.</span></span> <span data-ttu-id="10b91-122">أفضل ممارسة أحرف حوالي 400--</span><span class="sxs-lookup"><span data-stu-id="10b91-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="10b91-123">بمجرد المحتوى الخاص بك جاهز، تسحبه إلى الفرع مباشرة.</span><span class="sxs-lookup"><span data-stu-id="10b91-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="10b91-124">ثم انتقل إلى [بوابة الشركاء "الكيمياء"](https://alchemyportal.azurewebsites.net) وأدخل اسم الملف في الحقل.</span><span class="sxs-lookup"><span data-stu-id="10b91-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> 


