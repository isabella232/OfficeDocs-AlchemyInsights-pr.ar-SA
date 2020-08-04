---
title: استخدام برنامج TeamViewer لإدارة أجهزة Intune عن بعد
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1284"
- "6700008"
ms.openlocfilehash: 63e7f068f3c53240ad13d1679df460c97a1a94f4
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 07/28/2020
ms.locfileid: "46554712"
---
# <a name="use-teamviewer-to-remotely-administer-intune-devices"></a><span data-ttu-id="2e730-102">استخدام برنامج TeamViewer لإدارة أجهزة Intune عن بعد</span><span class="sxs-lookup"><span data-stu-id="2e730-102">Use TeamViewer to remotely administer Intune devices</span></span>

<span data-ttu-id="2e730-103">يمكن إدارة الأجهزة التي تديرها Intune عن بعد باستخدام [برنامج TeamViewer](https://www.teamviewer.com/).</span><span class="sxs-lookup"><span data-stu-id="2e730-103">Devices managed by Intune can be administered remotely by using [TeamViewer](https://www.teamviewer.com/).</span></span>

<span data-ttu-id="2e730-104">لإدارة Intune باستخدام TeamViewer، استخدم الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="2e730-104">To administer Intune by using TeamViewer, use these steps:</span></span> 

<span data-ttu-id="2e730-105">ابدأ بالحصول على بيانات الاعتماد من TeamViewer لإعداد موصل TeamViewer على Intune.</span><span class="sxs-lookup"><span data-stu-id="2e730-105">Begin by obtaining credentials from TeamViewer to set up the TeamViewer Connector on Intune.</span></span> <span data-ttu-id="2e730-106">يسمح هذا المسؤول بإدخال بيانات الاعتماد في واجهة مستخدم موصل TeamViewer ضمن الأجهزة، عملية لمرة واحدة لتأسيس الارتباط بين Intune وخدمة TeamViewer.</span><span class="sxs-lookup"><span data-stu-id="2e730-106">This allows the admin to enter credentials in the TeamViewer Connector UI under Devices, a one-time operation to establish the link between Intune and the TeamViewer service.</span></span>

<span data-ttu-id="2e730-107">**الجزء 1: بدء جلسة عمل باستخدام جهاز بعيد**</span><span class="sxs-lookup"><span data-stu-id="2e730-107">**Part 1: Start a session with a remote device**</span></span>

1. <span data-ttu-id="2e730-108">ضمن **كافة الأجهزة**، حدد الجهاز الذي تريد بدء جلسة عمل عن بعد به.</span><span class="sxs-lookup"><span data-stu-id="2e730-108">Under **All devices**, select the device you want to start a remote session with.</span></span>
2. <span data-ttu-id="2e730-109">من **... المزيد**، حدد **جلسة مساعدة عن بعد جديدة**.</span><span class="sxs-lookup"><span data-stu-id="2e730-109">From  **…More**, select **New remote assistance session**.</span></span>
3. <span data-ttu-id="2e730-110">حدد **نعم** للاعتراف بأنك تريد إنشاء جلسة عمل بعيدة.</span><span class="sxs-lookup"><span data-stu-id="2e730-110">Select **Yes** to acknowledge you want to establish a remote session.</span></span>
    <span data-ttu-id="2e730-111">بعد أن تم التعرف على طلب "بدء جلسة عمل جديدة عن بعد" من قبل خدمة TeamViewer، سترى خيار **بدء المساعدة عن بعد** ضمن تفاصيل جزء نظرة عامة (أو أساسيات) للجهاز.</span><span class="sxs-lookup"><span data-stu-id="2e730-111">After the "Initiating a new remote session" request is acknowledged by the TeamViewer service, you'll see an option to **Start remote assistance** under the details of the Overview (or, Essentials) pane for the device.</span></span> <span data-ttu-id="2e730-112">حدد **عرض المزيد** لتوسيع الجزء وإظهار حالة المساعدة عن بعد.</span><span class="sxs-lookup"><span data-stu-id="2e730-112">Select **See More** to expand the pane and show the Remote Assistance status.</span></span>
4. <span data-ttu-id="2e730-113">حدد **بدء جلسة العمل البعيدة** لبدء جلسة العمل على جانب المسؤول.</span><span class="sxs-lookup"><span data-stu-id="2e730-113">Select **Start remote session** to initiate the session on the admin side.</span></span>
5. <span data-ttu-id="2e730-114">اختر تنزيل الملف الثنائي TeamViewer (Windows)، وحدد **تشغيل**.</span><span class="sxs-lookup"><span data-stu-id="2e730-114">Choose to download the TeamViewer binary (Windows), and select **Run**.</span></span><br/>
    <span data-ttu-id="2e730-115">**ملاحظة** يمكنك تجاهل أي صفحة متصفح ويب مفتوحة لموقع TeamViewer على شبكة الإنترنت.</span><span class="sxs-lookup"><span data-stu-id="2e730-115">**Note** You can ignore any web browser page opened to the TeamViewer web site.</span></span>

6. <span data-ttu-id="2e730-116">قم بالإقرار بطلب تطبيق TeamViewer لإجراء تغييرات على الجهاز (Windows فقط).</span><span class="sxs-lookup"><span data-stu-id="2e730-116">Acknowledge the request for the TeamViewer app to make changes on the device (Windows only).</span></span>
7. <span data-ttu-id="2e730-117">يبدأ تطبيق TeamViewer ويتضمن رمز الجلسة لمصادقة الاتصال بالجهاز البعيد.</span><span class="sxs-lookup"><span data-stu-id="2e730-117">The TeamViewer app starts and includes the session code to authenticate the connection with the remote device.</span></span>

<span data-ttu-id="2e730-118">**الجزء 2: على الجهاز المستهدف لجلسة عمل عن بعد**</span><span class="sxs-lookup"><span data-stu-id="2e730-118">**Part 2: On the device being targeted for a remote session**</span></span>

1. <span data-ttu-id="2e730-119">افتح مدخل شركة Intune.</span><span class="sxs-lookup"><span data-stu-id="2e730-119">Open the Intune company portal.</span></span>
2. <span data-ttu-id="2e730-120">ابحث عن إشارة إعلام: "مسؤول تكنولوجيا المعلومات يطلب التحكم في هذا الجهاز لجلسة مساعدة عن بعد"، وحدد الإعلام.</span><span class="sxs-lookup"><span data-stu-id="2e730-120">Look for a notification flag: "Your IT administrator is requesting control of this device for a remote assistance session," and select the notification.</span></span>
3. <span data-ttu-id="2e730-121">اختر تنزيل تطبيق TeamViewer، أو الاعتراف بتنزيل تطبيق TeamViewer من متجر التطبيقات، وحدد **تشغيل**.</span><span class="sxs-lookup"><span data-stu-id="2e730-121">Choose to download the TeamViewer application, or acknowledge download of the TeamViewer app from the app store, and select **Run**.</span></span>
    <span data-ttu-id="2e730-122">**ملاحظة** يمكنك تجاهل أي صفحة متصفح ويب مفتوحة لموقع TeamViewer على شبكة الإنترنت.</span><span class="sxs-lookup"><span data-stu-id="2e730-122">**Note** You can ignore any web browser page opened to the TeamViewer web site.</span></span>

4. <span data-ttu-id="2e730-123">قم بالإقرار بطلب تطبيق TeamViewer لإجراء تغييرات على الجهاز (Windows فقط).</span><span class="sxs-lookup"><span data-stu-id="2e730-123">Acknowledge the request for the TeamViewer app to make changes on the device (Windows only).</span></span>
5. <span data-ttu-id="2e730-124">يبدأ تطبيق TeamViewer ويتضمن رمز الجلسة لمصادقة الاتصال بالجهاز البعيد.</span><span class="sxs-lookup"><span data-stu-id="2e730-124">The TeamViewer app starts and includes the session code to authenticate the connection with the remote device.</span></span>
6. <span data-ttu-id="2e730-125">يسألك أحد النوافذ المنبثقة عما إذا كنت تريد السماح لبدء الجلسة.</span><span class="sxs-lookup"><span data-stu-id="2e730-125">A popup asks if you want to allow the session to start.</span></span>

<span data-ttu-id="2e730-126">**ملاحظة** رموز جلسة العمل التي تم إنشاؤها بواسطة خدمة TeamViewer هي استخدام مرة واحدة فقط.</span><span class="sxs-lookup"><span data-stu-id="2e730-126">**Note** The session codes generated by the TeamViewer service are one-time use only.</span></span> <span data-ttu-id="2e730-127">إذا فقدت الاتصال، يجب عليك:</span><span class="sxs-lookup"><span data-stu-id="2e730-127">If you lose the connection, you must:</span></span>

1. <span data-ttu-id="2e730-128">أغلق مثيل تطبيق TeamViewer على الجهاز البعيد وعلى محطة العمل المشرفة.</span><span class="sxs-lookup"><span data-stu-id="2e730-128">Close the instance of the TeamViewer app on the remote device and on the admin workstation.</span></span>
2. <span data-ttu-id="2e730-129">أغلق مدخل الشركة على الجهاز البعيد.</span><span class="sxs-lookup"><span data-stu-id="2e730-129">Close the company portal on the remote device.</span></span>
3. <span data-ttu-id="2e730-130">بدء تشغيل "جلسة مساعدة جديدة عن بعد" جديدة من مدخل المسؤول.</span><span class="sxs-lookup"><span data-stu-id="2e730-130">Initiate a new "New remote Assistance session" from the admin portal.</span></span>
4. <span data-ttu-id="2e730-131">إعادة فتح مدخل الشركة على الجهاز البعيد لتلقي الإعلام الجديد.</span><span class="sxs-lookup"><span data-stu-id="2e730-131">Re-open the company portal on the remote device to receive the new notification.</span></span>
5. <span data-ttu-id="2e730-132">قم بتنزيل تطبيق TeamViewer وفتحه على كل من الجهاز البعيد ومحطة العمل المشرفة، كما كان الحال من قبل.</span><span class="sxs-lookup"><span data-stu-id="2e730-132">Download and open the TeamViewer app on both the remote device and the admin workstation, as before.</span></span>