---
title: تماما مثل اسم الملف هو الأفضل
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: 113d01e0fc92cc9845e585919ab05f386d6892bb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664121"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="dceb7-102">"كيمياء العنوان المطلوب H1 ، H2's لا يعمل."</span><span class="sxs-lookup"><span data-stu-id="dceb7-102">"Required Alchemy Header H1, H2's dont work."</span></span>
<span data-ttu-id="dceb7-103">أفضل الممارسات والإرشادات لتاليف كيمياء:</span><span class="sxs-lookup"><span data-stu-id="dceb7-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="dceb7-104">**عدم تداخل كيمياء المعارف الدقيقة في المجلدات**-سيؤدي ذلك إلى قطع بنيه url.</span><span class="sxs-lookup"><span data-stu-id="dceb7-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="dceb7-105">نبحث إلى إصلاح هذا.</span><span class="sxs-lookup"><span data-stu-id="dceb7-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="dceb7-106">يجب ان تحتوي الملفات الموجودة في مجلد **التشيميينسايتس** علي أسماء أحرف صغيره تحتوي علي واصلات للمسافات.</span><span class="sxs-lookup"><span data-stu-id="dceb7-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="dceb7-107">***كيفيه التمكين-قائمه الانتظار القضائي***.</span><span class="sxs-lookup"><span data-stu-id="dceb7-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="dceb7-108">قم بتضمين معرف القاعدة أو معرف الحزمة من [مدخل شريك كيمياء](https://alchemyportal.azurewebsites.net) في الحقل ms. custom.</span><span class="sxs-lookup"><span data-stu-id="dceb7-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="dceb7-109">سبيل.</span><span class="sxs-lookup"><span data-stu-id="dceb7-109">ex.</span></span> <span data-ttu-id="dceb7-110">***ث. مخصص: 100021***</span><span class="sxs-lookup"><span data-stu-id="dceb7-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="dceb7-111">استخدم الجزء المتبقي من البيانات الاوليه في هذا الملف كقالب.</span><span class="sxs-lookup"><span data-stu-id="dceb7-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="dceb7-112">في [مدخل شريك كيمياء](https://alchemyportal.azurewebsites.net)، انتقل إلى الأسفل وصولا إلى القسم " **العنوان الدقيقة للعملاء":** واستخدمه كنقطه بداية لعنوان H1 الخاص بك للحصول علي المعرفة الدقيقة.</span><span class="sxs-lookup"><span data-stu-id="dceb7-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="dceb7-113">يجب ان تتضمن المعارف الدقيقة ل كيمياء H1 واحده فقط في الجزء العلوي أو سيتم تقسيمها في الإنتاج.</span><span class="sxs-lookup"><span data-stu-id="dceb7-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="dceb7-114">H2s لا تقدم أيا كان الأمران يستخدمان **الخط الغامق** أو الاصطلاحات الأخرى لتدل علي مقاطع منفصلة.</span><span class="sxs-lookup"><span data-stu-id="dceb7-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="dceb7-115">بعد ذلك ، قم بتعبئة النص الأساسي باستخدام مواد المسودة في القسم "المعارف الدقيقة للعملاء" من الصفحة "القاعدة الكيمياءه"</span><span class="sxs-lookup"><span data-stu-id="dceb7-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="dceb7-116">القوائم ذات التعداد النقطي جيده</span><span class="sxs-lookup"><span data-stu-id="dceb7-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="dceb7-117">القوائم ذات التعداد الرقمي أيضا</span><span class="sxs-lookup"><span data-stu-id="dceb7-117">Numbered lists too</span></span>
    1. <span data-ttu-id="dceb7-118">**التنسيق الغامق** *والمائل* عبارة عن "ا"</span><span class="sxs-lookup"><span data-stu-id="dceb7-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="dceb7-119">يجب ان تكون الارتباطات اما **"ارتباطات إلى الويب"/External** أو **الارتباطات العميقة بعناصر واجهه المستخدم**، وليس الارتباطات الداخلية.</span><span class="sxs-lookup"><span data-stu-id="dceb7-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="dceb7-120">لا يتم دعم الصور رسميا في الوقت الحالي ، ولكنها علي الخريطة.</span><span class="sxs-lookup"><span data-stu-id="dceb7-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="dceb7-121">وهذه هي بالفعل بت طويل جدا.</span><span class="sxs-lookup"><span data-stu-id="dceb7-121">And this is really already a bit too long.</span></span> <span data-ttu-id="dceb7-122">أفضل ممارسه هي حول 400 حرف---------------------------------</span><span class="sxs-lookup"><span data-stu-id="dceb7-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="dceb7-123">بمجرد ان يصبح المحتوي جاهزا ، اسحبه إلى الفرع المباشر.</span><span class="sxs-lookup"><span data-stu-id="dceb7-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="dceb7-124">ثم انتقل إلى [مدخل شريك كيمياء](https://alchemyportal.azurewebsites.net) وادخل اسم الملف في حقل url.</span><span class="sxs-lookup"><span data-stu-id="dceb7-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> 