---
title: فتح الملف للقراءة فقط
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/26/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 39748581-d319-403c-8501-9b785e4a0ed8
ms.custom:
- "765"
- "2200014"
ms.openlocfilehash: eddd427b159a782abf53adda934de8b15a02ed00
ms.sourcegitcommit: 8864b5789d9905916039081b53530c7e6d8bc529
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/10/2019
ms.locfileid: "36822221"
---
# <a name="file-open-read-only"></a><span data-ttu-id="15982-102">فتح الملف للقراءة فقط</span><span class="sxs-lookup"><span data-stu-id="15982-102">File open read-only</span></span>

<span data-ttu-id="15982-103">قد تجد أنه عند فتح الملفات، يتم فتحها للقراءة فقط.</span><span class="sxs-lookup"><span data-stu-id="15982-103">You may find that when you are opening files, they open as read-only.</span></span> <span data-ttu-id="15982-104">في بعض الحالات، يكون هذا لمزيد من الأمان، مثل عند فتح الملفات من الإنترنت، وفي أوقات أخرى، يمكن أن يكون بسبب إعداد يمكن تغييره.</span><span class="sxs-lookup"><span data-stu-id="15982-104">In some cases, this is for added security, such as when you are opening files from the internet, and other times, it can be due to a setting that can be changed.</span></span> <span data-ttu-id="15982-105">فيما يلي بعض وحدات السيناريو حيث يفتح ملف للقراءة فقط وبعض الخطوات التي يمكنك اتخاذها لتغيير ذلك.</span><span class="sxs-lookup"><span data-stu-id="15982-105">Here are some scenarios where a file opens read-only and some steps you can take to change that.</span></span>
  
 <span data-ttu-id="15982-106">**مكافحة الفيروسات بلدي يسبب لهم لفتح للقراءة فقط**</span><span class="sxs-lookup"><span data-stu-id="15982-106">**My antivirus is causing them to open read-only**</span></span>
  
<span data-ttu-id="15982-107">قد تحميك بعض برامج مكافحة الفيروسات من الملفات التي قد تكون غير آمنة عن طريق فتحها للقراءة فقط.</span><span class="sxs-lookup"><span data-stu-id="15982-107">Some antivirus programs may protect you from potentially unsafe files by opening them read-only.</span></span> <span data-ttu-id="15982-108">قد تحتاج إلى مراجعة موفر مكافحة الفيروسات لمعرفة كيفية ضبط هذه الإعدادات.</span><span class="sxs-lookup"><span data-stu-id="15982-108">You may need to check with your antivirus provider to learn how to adjust these settings.</span></span> <span data-ttu-id="15982-109">BitDefender، على سبيل المثال، يحتوي على محتوى على إضافة استبعادات التطبيق هنا: [كيفية إضافة تطبيقات أو معالجة الاستثناءات في مركز التحكم Bitdefender](https://aka.ms/AA6098i).</span><span class="sxs-lookup"><span data-stu-id="15982-109">BitDefender, for example, has content on adding application exclusions here: [How to add application or process exclusions in Bitdefender Control Center](https://aka.ms/AA6098i).</span></span>
  
 <span data-ttu-id="15982-110">**هل يتم تعيين خصائص الملف للقراءة فقط؟**</span><span class="sxs-lookup"><span data-stu-id="15982-110">**Are the file properties set to read-only?**</span></span>
  
<span data-ttu-id="15982-111">يمكنك التحقق من خصائص الملف بالنقر بزر الماوس الأيمن فوق الملف واختيار خصائص.</span><span class="sxs-lookup"><span data-stu-id="15982-111">You can check the file properties by right-clicking on the file and choosing Properties.</span></span> <span data-ttu-id="15982-112">إذا تم تحديد السمة للقراءة فقط، يمكنك إلغاء تحديدها ثم انقر فوق موافق.</span><span class="sxs-lookup"><span data-stu-id="15982-112">If the Read-only attribute is checked, you can uncheck it and click OK.</span></span>
  
 <span data-ttu-id="15982-113">**المحتوى في طريقة العرض المحمية**</span><span class="sxs-lookup"><span data-stu-id="15982-113">**The content is in protected view**</span></span>
  
<span data-ttu-id="15982-114">يمكن أن تحتوي الملفات من الإنترنت ومن مواقع أخرى قد تكون غير آمنة على فيروسات أو ديمنات أو أنواع أخرى من البرامج الضارة التي يمكن أن تضر بالكمبيوتر.</span><span class="sxs-lookup"><span data-stu-id="15982-114">Files from the Internet and from other potentially unsafe locations can contain viruses, worms, or other kinds of malware that can harm your computer.</span></span> <span data-ttu-id="15982-115">هذا هو الحال أيضا عادة مع مرفقات البريد الإلكتروني أو الملفات التي قمت بتحميلها.</span><span class="sxs-lookup"><span data-stu-id="15982-115">This is also commonly the case with email attachments or files you've downloaded.</span></span> <span data-ttu-id="15982-116">للمساعدة في حماية الكمبيوتر، يتم فتح الملفات من هذه المواقع التي قد تكون غير آمنة في "طريقة العرض المحمية".</span><span class="sxs-lookup"><span data-stu-id="15982-116">To help protect your computer, files from these potentially unsafe locations are opened in Protected View.</span></span> <span data-ttu-id="15982-117">باستخدام "طريقة العرض المحمية"، يمكنك قراءة ملف ومشاهدة محتوياته مع تقليل المخاطر.</span><span class="sxs-lookup"><span data-stu-id="15982-117">By using Protected View, you can read a file and see its contents while reducing the risks.</span></span> <span data-ttu-id="15982-118">لمزيد من المعلومات حول طريقة العرض المحمية وكيفية تغيير الإعدادات، راجع هذه المقالة: [ما هو طريقة العرض المحمية؟](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span><span class="sxs-lookup"><span data-stu-id="15982-118">For more information on Protected view and how to change settings, see this article: [What is Protected View?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span></span>
  
 <span data-ttu-id="15982-119">**هل OneDrive ممتلئ؟**</span><span class="sxs-lookup"><span data-stu-id="15982-119">**Is OneDrive full?**</span></span>
  
<span data-ttu-id="15982-120">إذا تم تخزين الملف على أندريف وكانت مساحة التخزين OneDrive ممتلئة، لن تتمكن من حفظ المستند حتى تكون ضمن المساحة المخصصة.</span><span class="sxs-lookup"><span data-stu-id="15982-120">If the file is stored on OneDrive and your OneDrive storage space is full, you will be unable to save the document until you are under your allotted space.</span></span> <span data-ttu-id="15982-121">يمكنك التحقق من المساحة الحرة على OneDrive بالنقر فوق رمز OneDrive في مركز الإعلام [http://onedrive.live.com](http://onedrive.live.com)واختيار إدارة التخزين، أو يمكنك الانتقال إلى تسجيل الدخول وملاحظة مقدار المساحة المستخدمة في أسفل يسار الشاشة.</span><span class="sxs-lookup"><span data-stu-id="15982-121">You can check your free space on OneDrive by clicking the OneDrive icon in the notification center and choosing Manage storage, or you can go to [http://onedrive.live.com](http://onedrive.live.com), sign in, and note the amount of used space in the lower left of the screen.</span></span>
  
 <span data-ttu-id="15982-122">**هل تم تنشيط Office؟**</span><span class="sxs-lookup"><span data-stu-id="15982-122">**Is Office activated?**</span></span>
  
<span data-ttu-id="15982-123">إذا لم يتم تنشيط Office، أو إذا انتهت مدة صلاحية اشتراكك، فقد تكون في وضع الأداء الوظيفي المنخفض للقراءة فقط.</span><span class="sxs-lookup"><span data-stu-id="15982-123">If Office is not activated, or if your subscription has expired, you could be in read-only Reduced Functionality Mode.</span></span> <span data-ttu-id="15982-124">للحصول على معلومات حول كيفية تنشيط Office، راجع: [المنتج غير المرخص وأخطاء التنشيط في Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span><span class="sxs-lookup"><span data-stu-id="15982-124">For information on how to Activate Office, see: [Unlicensed Product and activation errors in Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>
  
 <span data-ttu-id="15982-125">**إذا فشل كل شيء آخر...**</span><span class="sxs-lookup"><span data-stu-id="15982-125">**If all else fails...**</span></span>
  
- <span data-ttu-id="15982-126">محاولة إعادة تشغيل الكمبيوتر</span><span class="sxs-lookup"><span data-stu-id="15982-126">Try restarting the computer</span></span>
    
- <span data-ttu-id="15982-127">تثبيت تحديثات Office</span><span class="sxs-lookup"><span data-stu-id="15982-127">Install Office updates</span></span>
    
- <span data-ttu-id="15982-128">إجراء إصلاح عبر الإنترنت لـ Office</span><span class="sxs-lookup"><span data-stu-id="15982-128">Perform an Online repair of Office</span></span>
    

