---
title: فتح الملف للقراءة فقط
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 39748581-d319-403c-8501-9b785e4a0ed8
ms.custom:
- "765"
- "2200014"
ms.openlocfilehash: e478572ea82e5ea11bac9fd7eacafb833253235d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813171"
---
# <a name="file-open-read-only"></a><span data-ttu-id="3d337-102">فتح الملف للقراءة فقط</span><span class="sxs-lookup"><span data-stu-id="3d337-102">File open read-only</span></span>

<span data-ttu-id="3d337-103">قد تجد أنه عند فتح الملفات، يتم فتحها للقراءة فقط.</span><span class="sxs-lookup"><span data-stu-id="3d337-103">You may find that when you are opening files, they open as read-only.</span></span> <span data-ttu-id="3d337-104">في بعض الحالات، يكون ذلك لمزيد من الأمان، على سبيل المثال عند فتح الملفات من الإنترنت، وفي أوقات أخرى، قد يكون ذلك بسبب إعداد يمكن تغييره.</span><span class="sxs-lookup"><span data-stu-id="3d337-104">In some cases, this is for added security, such as when you are opening files from the internet, and other times, it can be due to a setting that can be changed.</span></span> <span data-ttu-id="3d337-105">فيما يلي بعض السيناريوهات التي يتم فيها فتح ملف للقراءة فقط وبعض الخطوات التي يمكنك اتخاذها لتغيير ذلك.</span><span class="sxs-lookup"><span data-stu-id="3d337-105">Here are some scenarios where a file opens read-only and some steps you can take to change that.</span></span>
  
 <span data-ttu-id="3d337-106">**يتسبب برنامج الحماية من الفيروسات في فتحهم للقراءة فقط**</span><span class="sxs-lookup"><span data-stu-id="3d337-106">**My antivirus is causing them to open read-only**</span></span>
  
<span data-ttu-id="3d337-107">قد تحميك بعض برامج الحماية من الفيروسات من الملفات التي قد تكون غير آمنة عن طريق فتحها للقراءة فقط.</span><span class="sxs-lookup"><span data-stu-id="3d337-107">Some antivirus programs may protect you from potentially unsafe files by opening them read-only.</span></span> <span data-ttu-id="3d337-108">قد تحتاج إلى مراجعة موفر الحماية من الفيروسات لمعرفة كيفية ضبط هذه الإعدادات.</span><span class="sxs-lookup"><span data-stu-id="3d337-108">You may need to check with your antivirus provider to learn how to adjust these settings.</span></span> <span data-ttu-id="3d337-109">على سبيل المثال، تتضمن BitDefender محتوى حول إضافة استثناءات التطبيقات هنا: كيفية إضافة استثناءات التطبيقات أو العملية في مركز التحكم [Bitdefender](https://aka.ms/AA6098i).</span><span class="sxs-lookup"><span data-stu-id="3d337-109">BitDefender, for example, has content on adding application exclusions here: [How to add application or process exclusions in Bitdefender Control Center](https://aka.ms/AA6098i).</span></span>
  
 <span data-ttu-id="3d337-110">**هل تم تعيين خصائص الملف إلى للقراءة فقط؟**</span><span class="sxs-lookup"><span data-stu-id="3d337-110">**Are the file properties set to read-only?**</span></span>
  
<span data-ttu-id="3d337-111">يمكنك التحقق من خصائص الملف بالنقر ب الماوس الأيمن فوق الملف واختيار خصائص.</span><span class="sxs-lookup"><span data-stu-id="3d337-111">You can check the file properties by right-clicking on the file and choosing Properties.</span></span> <span data-ttu-id="3d337-112">إذا كانت السمة للقراءة فقط محددة، يمكنك إلغاء تحديدها والنقر فوق موافق.</span><span class="sxs-lookup"><span data-stu-id="3d337-112">If the Read-only attribute is checked, you can uncheck it and click OK.</span></span>
  
 <span data-ttu-id="3d337-113">**المحتوى في طريقة عرض محمية**</span><span class="sxs-lookup"><span data-stu-id="3d337-113">**The content is in protected view**</span></span>
  
<span data-ttu-id="3d337-114">يمكن أن تحتوي الملفات من الإنترنت ومن مواقع أخرى يحتمل أن تكون غير آمنة على فيروسات أو فيروسات متنقلة أو أنواع أخرى من البرامج الضارة التي يمكن أن تؤذي الكمبيوتر.</span><span class="sxs-lookup"><span data-stu-id="3d337-114">Files from the Internet and from other potentially unsafe locations can contain viruses, worms, or other kinds of malware that can harm your computer.</span></span> <span data-ttu-id="3d337-115">وهذا هو الحال عادة مع مرفقات البريد الإلكتروني أو الملفات التي قمت بتنزيلها.</span><span class="sxs-lookup"><span data-stu-id="3d337-115">This is also commonly the case with email attachments or files you've downloaded.</span></span> <span data-ttu-id="3d337-116">للمساعدة في حماية الكمبيوتر، يتم فتح الملفات من هذه المواقع التي قد تكون غير آمنة في "طريقة عرض محمية".</span><span class="sxs-lookup"><span data-stu-id="3d337-116">To help protect your computer, files from these potentially unsafe locations are opened in Protected View.</span></span> <span data-ttu-id="3d337-117">باستخدام "طريقة عرض محمية"، يمكنك قراءة ملف لمشاهدة محتوياته مع تقليل المخاطر.</span><span class="sxs-lookup"><span data-stu-id="3d337-117">By using Protected View, you can read a file and see its contents while reducing the risks.</span></span> <span data-ttu-id="3d337-118">لمزيد من المعلومات حول طريقة العرض المحمية وكيفية تغيير الإعدادات، راجع هذه المقالة: ما هي طريقة العرض [المحمية؟](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span><span class="sxs-lookup"><span data-stu-id="3d337-118">For more information on Protected view and how to change settings, see this article: [What is Protected View?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span></span>
  
 <span data-ttu-id="3d337-119">**هل OneDrive ممتلئ؟**</span><span class="sxs-lookup"><span data-stu-id="3d337-119">**Is OneDrive full?**</span></span>
  
<span data-ttu-id="3d337-120">إذا كان الملف مخزنا على OneDrive ومساحة التخزين في OneDrive ممتلئة، لن تتمكن من حفظ المستند حتى تكون ضمن المساحة المخصصة.</span><span class="sxs-lookup"><span data-stu-id="3d337-120">If the file is stored on OneDrive and your OneDrive storage space is full, you will be unable to save the document until you are under your allotted space.</span></span> <span data-ttu-id="3d337-121">يمكنك التحقق من المساحة المجانية على OneDrive بالنقر فوق أيقونة OneDrive في مركز الإعلامات واختيار إدارة التخزين، أو يمكنك الانتقال إلى ، تسجيل الدخول، ولاحظ مقدار المساحة المستخدمة في الجزء السفلي الأيسر من [https://onedrive.live.com](https://onedrive.live.com) الشاشة.</span><span class="sxs-lookup"><span data-stu-id="3d337-121">You can check your free space on OneDrive by clicking the OneDrive icon in the notification center and choosing Manage storage, or you can go to [https://onedrive.live.com](https://onedrive.live.com), sign in, and note the amount of used space in the lower left of the screen.</span></span>
  
 <span data-ttu-id="3d337-122">**هل تم تنشيط Office؟**</span><span class="sxs-lookup"><span data-stu-id="3d337-122">**Is Office activated?**</span></span>
  
<span data-ttu-id="3d337-123">إذا لم يتم تنشيط Office، أو إذا انتهت صلاحية اشتراكك، فقد تكون في وضع الأداء الوظيفي المنخفض للقراءة فقط.</span><span class="sxs-lookup"><span data-stu-id="3d337-123">If Office is not activated, or if your subscription has expired, you could be in read-only Reduced Functionality Mode.</span></span> <span data-ttu-id="3d337-124">للحصول على معلومات حول كيفية تنشيط Office، راجع: أخطاء التنشيط والمنتج غير مرخص [في Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span><span class="sxs-lookup"><span data-stu-id="3d337-124">For information on how to Activate Office, see: [Unlicensed Product and activation errors in Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>
  
 <span data-ttu-id="3d337-125">**إذا فشل كل شيء آخر...**</span><span class="sxs-lookup"><span data-stu-id="3d337-125">**If all else fails...**</span></span>
  
- <span data-ttu-id="3d337-126">حاول إعادة تشغيل الكمبيوتر</span><span class="sxs-lookup"><span data-stu-id="3d337-126">Try restarting the computer</span></span>
    
- <span data-ttu-id="3d337-127">تثبيت تحديثات Office</span><span class="sxs-lookup"><span data-stu-id="3d337-127">Install Office updates</span></span>
    
- <span data-ttu-id="3d337-128">إجراء إصلاح عبر الإنترنت ل Office</span><span class="sxs-lookup"><span data-stu-id="3d337-128">Perform an Online repair of Office</span></span>
    

