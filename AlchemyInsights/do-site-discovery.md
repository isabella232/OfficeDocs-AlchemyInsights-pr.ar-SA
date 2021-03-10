---
title: القيام باكتشاف الموقع
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9143"
- "9005291"
ms.openlocfilehash: bdf94220de45d92f63e56501ea4e35389224d25c
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/08/2021
ms.locfileid: "50692407"
---
# <a name="do-site-discovery"></a><span data-ttu-id="59e5b-102">القيام باكتشاف الموقع</span><span class="sxs-lookup"><span data-stu-id="59e5b-102">Do site discovery</span></span>

<span data-ttu-id="59e5b-103">إذا كانت مؤسستك لا تزال تستخدم تطبيقات ويب القديمة وخططت لاستخدام وضع Internet Explorer (الذي يستخدمه معظم العملاء)، يجب عليك القيام ببعض الاكتشاف الإضافي للموقع.</span><span class="sxs-lookup"><span data-stu-id="59e5b-103">If your organization still uses legacy web applications and plans to use Internet Explorer mode (which most customers do), then you should do some additional site discovery.</span></span>

<span data-ttu-id="59e5b-104">**لقد نشرت بالفعل إصدارا قديما من Microsoft Edge**</span><span class="sxs-lookup"><span data-stu-id="59e5b-104">**You've already deployed an older version of Microsoft Edge**</span></span>

<span data-ttu-id="59e5b-105">إذا كنت قد قمت بالفعل بتكوين قائمة مواقع المؤسسة للعمل مع الإصدار القديم من Microsoft Edge، فإن اكتشاف موقعك على وشك أن ينتهى.</span><span class="sxs-lookup"><span data-stu-id="59e5b-105">If you've already configured your Enterprise Site List to work for the legacy version of Microsoft Edge, then your site discovery is almost done.</span></span> <span data-ttu-id="59e5b-106">الأمر الوحيد الذي قد تحتاج إلى القيام به هو إضافة مواقع حيادية.</span><span class="sxs-lookup"><span data-stu-id="59e5b-106">The one thing you might need to do is add neutral sites.</span></span>

<span data-ttu-id="59e5b-107">عادة ما تكون المواقع المحايدة مواقع توفر تسجيل الدخول الفردي (SSO).</span><span class="sxs-lookup"><span data-stu-id="59e5b-107">Neutral sites are typically sites that provide single sign-on (SSO).</span></span> <span data-ttu-id="59e5b-108">إذا كنت تذهب إلى موقع محايد من Microsoft Edge، إذا كنت تريد البقاء في Microsoft Edge للمصادقة.</span><span class="sxs-lookup"><span data-stu-id="59e5b-108">If you go to a neutral site from Microsoft Edge, then you want to stay in Microsoft Edge to authenticate.</span></span> <span data-ttu-id="59e5b-109">إذا كنت تذهب إلى موقع محايد في وضع Internet Explorer، إذا كنت تريد البقاء في وضع Internet Explorer للمصادقة.</span><span class="sxs-lookup"><span data-stu-id="59e5b-109">If you go to a neutral site in Internet Explorer mode, then you want to stay in Internet Explorer mode to authenticate.</span></span>

<span data-ttu-id="59e5b-110">حدد أي SSO أو مواقع حيادية أخرى تستخدمها وأضفها إلى قائمة مواقع المؤسسة.</span><span class="sxs-lookup"><span data-stu-id="59e5b-110">Identify any SSO or other neutral sites that you use and add these to your Enterprise Site List.</span></span>

<span data-ttu-id="59e5b-111">**Internet Explorer هو المستعرض الافتراضي**</span><span class="sxs-lookup"><span data-stu-id="59e5b-111">**Internet Explorer is your default browser**</span></span>

<span data-ttu-id="59e5b-112">إذا كنت تستخدم Internet Explorer الآن فقط، فقد لا تعلم المواقع التي تمت ترقيتها إلى معايير الويب الحديثة والتي ما زالت تتطلب Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="59e5b-112">If you're only using Internet Explorer now, you might not know which sites have upgraded to modern web standards and which still require Internet Explorer.</span></span> <span data-ttu-id="59e5b-113">وسترغب في البحث عن هذه المواقع وإضافتها إلى قائمة مواقع المؤسسة بحيث يمكنك استخدام وضع Internet Explorer لتلك المواقع فقط.</span><span class="sxs-lookup"><span data-stu-id="59e5b-113">You'll want to find and add these sites to the Enterprise Site List so that you can use Internet Explorer mode only for those sites.</span></span>

> [!NOTE]
> <span data-ttu-id="59e5b-114">[يكتشف "اكتشاف موقع المؤسسة"](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) المواقع التي قد تحتاج إلى وضع Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="59e5b-114">[Enterprise Site Discovery](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) discovers sites that might need Internet Explorer mode.</span></span> <span data-ttu-id="59e5b-115">يمكنه تجميع البيانات على أجهزة الكمبيوتر التي تعمل بنظام Windows Internet Explorer 8 عبر Internet Explorer 11 على Windows 10 أو Windows 8.1 أو Windows 7.</span><span class="sxs-lookup"><span data-stu-id="59e5b-115">It can collect data on computers running Windows Internet Explorer 8 through Internet Explorer 11 on Windows 10, Windows 8.1, or Windows 7.</span></span>

<span data-ttu-id="59e5b-116">**تحليل البيانات**</span><span class="sxs-lookup"><span data-stu-id="59e5b-116">**Analyze the data**</span></span>

<span data-ttu-id="59e5b-117">بعد تجميع بيانات الموقع، نوصي بإجراء العملية التالية التي تصحب أربع خطوات لتحليل البيانات:</span><span class="sxs-lookup"><span data-stu-id="59e5b-117">After you've collected site data, we recommend the following four-step process to analyze the data:</span></span>
1. <span data-ttu-id="59e5b-118">قم بفرز البيانات حسب المجال، ثم حسب URL.</span><span class="sxs-lookup"><span data-stu-id="59e5b-118">Sort the data by domain, and then by URL.</span></span>
2. <span data-ttu-id="59e5b-119">تعريف حدود التطبيق لتكوينه في وضع Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="59e5b-119">Define the boundaries of an app to configure for Internet Explorer mode.</span></span> <span data-ttu-id="59e5b-120">تريد تضمين كل المواقع و عناصر التحكم على الويب التي تعرف التطبيق، ولكنك لا تريد تضمين عناصر تحكم ومواقع إضافية.</span><span class="sxs-lookup"><span data-stu-id="59e5b-120">You want to include all the sites and web controls that define the app, but you don't want to include extra sites and controls.</span></span> <span data-ttu-id="59e5b-121">قد تكون بعض المواقع بسيطة كما قد يتطلب البعض الآخر تعريف *https://contoso.com/app1* مواقع وصفحات متعددة.</span><span class="sxs-lookup"><span data-stu-id="59e5b-121">Some sites might be as simple as *https://contoso.com/app1* while others might require you to define multiple sites and pages.</span></span>
3. <span data-ttu-id="59e5b-122">اختبر التطبيق للتحقق من أنه لا يعمل في أصلي.</span><span class="sxs-lookup"><span data-stu-id="59e5b-122">Test the app to verify that it doesn't work natively.</span></span> <span data-ttu-id="59e5b-123">ستعرض العديد من المواقع محتوى حديث عند الكشف عن مستعرض حديث، كما أنها لا تقدم محتوى أقدم إلا عند الكشف عن Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="59e5b-123">Many sites will offer modern content when they detect a modern browser and only offer legacy content when they detect Internet Explorer.</span></span>
4. <span data-ttu-id="59e5b-124">أضف التطبيق إلى قائمة مواقع المؤسسة إذا فشل في الاختبار.</span><span class="sxs-lookup"><span data-stu-id="59e5b-124">Add the app to your Enterprise Site List if it fails testing.</span></span>

> [!NOTE]
> <span data-ttu-id="59e5b-125">كأفضل ممارسة، يمكنك تجميع كل المواقع التي تتضمن تطبيقا.</span><span class="sxs-lookup"><span data-stu-id="59e5b-125">As a best practice, group all of the sites that comprise an app.</span></span> <span data-ttu-id="59e5b-126">بهذه الطريقة، عندما تقوم بترقية تطبيق، يصبح من السهل إزالة الموقع بالكامل من وضع Internet Explorer وبدء استخدام مستعرض حديث لهذا التطبيق.</span><span class="sxs-lookup"><span data-stu-id="59e5b-126">This way, when you upgrade an app, it's easier to remove the entire site from Internet Explorer mode and start using a modern browser for that app.</span></span>

<span data-ttu-id="59e5b-127">بمجرد انتهائك من اكتشاف الموقع وتحليل البيانات، تكون جاهزا لبدء النظر في استراتيجية القناة.</span><span class="sxs-lookup"><span data-stu-id="59e5b-127">Once you're done with site discovery and you've analyzed the data, you're ready to start looking at your channel strategy.</span></span>

