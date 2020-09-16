---
title: فتح ملف للقراءة فقط
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 2fdb4f048c2bee022a49c2cca2ce9770f42a87a2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47745558"
---
# <a name="file-open-read-only"></a><span data-ttu-id="90757-102">فتح ملف للقراءة فقط</span><span class="sxs-lookup"><span data-stu-id="90757-102">File open read-only</span></span>

<span data-ttu-id="90757-103">قد تجد انه يتم فتح الملفات عند فتحها للقراءة فقط.</span><span class="sxs-lookup"><span data-stu-id="90757-103">You may find that when you are opening files, they open as read-only.</span></span> <span data-ttu-id="90757-104">في بعض الحالات ، هذا هو الأمان الإضافي ، علي سبيل المثال عندما تفتح الملفات من الإنترنت ، والأوقات الأخرى ، يمكن ان يكون ذلك بسبب الاعداد الذي يمكن تغييره.</span><span class="sxs-lookup"><span data-stu-id="90757-104">In some cases, this is for added security, such as when you are opening files from the internet, and other times, it can be due to a setting that can be changed.</span></span> <span data-ttu-id="90757-105">اليك بعض السيناريوهات التي يفتح فيها ملف للقراءة فقط وبعض الخطوات التي يمكنك اتخاذها لتغيير ذلك.</span><span class="sxs-lookup"><span data-stu-id="90757-105">Here are some scenarios where a file opens read-only and some steps you can take to change that.</span></span>
  
 <span data-ttu-id="90757-106">**برنامج مكافحه الفيروسات الخاص بي هو الذي يتسبب في فتحه للقراءة فقط**</span><span class="sxs-lookup"><span data-stu-id="90757-106">**My antivirus is causing them to open read-only**</span></span>
  
<span data-ttu-id="90757-107">قد تحميك بعض برامج الحماية من الفيروسات من الملفات التي من المحتمل ان تكون غير أمنه عن طريق فتحها للقراءة فقط.</span><span class="sxs-lookup"><span data-stu-id="90757-107">Some antivirus programs may protect you from potentially unsafe files by opening them read-only.</span></span> <span data-ttu-id="90757-108">قد تحتاج إلى التحقق من موفر برامج الحماية من الفيروسات لمعرفه كيفيه ضبط هذه الإعدادات.</span><span class="sxs-lookup"><span data-stu-id="90757-108">You may need to check with your antivirus provider to learn how to adjust these settings.</span></span> <span data-ttu-id="90757-109">علي سبيل المثال ، يحتوي البيتديفيندير علي المحتوي في أضافه استثناءات التطبيق هنا: [كيفيه أضافه استثناءات التطبيقات أو العمليات في مركز التحكم بالبيتديفيندير](https://aka.ms/AA6098i).</span><span class="sxs-lookup"><span data-stu-id="90757-109">BitDefender, for example, has content on adding application exclusions here: [How to add application or process exclusions in Bitdefender Control Center](https://aka.ms/AA6098i).</span></span>
  
 <span data-ttu-id="90757-110">**هل تم تعيين خصائص الملف للقراءة فقط ؟**</span><span class="sxs-lookup"><span data-stu-id="90757-110">**Are the file properties set to read-only?**</span></span>
  
<span data-ttu-id="90757-111">يمكنك التحقق من خصائص الملف بالنقر بزر الماوس الأيمن فوق الملف واختيار الخصائص.</span><span class="sxs-lookup"><span data-stu-id="90757-111">You can check the file properties by right-clicking on the file and choosing Properties.</span></span> <span data-ttu-id="90757-112">إذا كانت السمة للقراءة فقط محدده ، فيمكنك إلغاء تحديدها والنقر فوق موافق.</span><span class="sxs-lookup"><span data-stu-id="90757-112">If the Read-only attribute is checked, you can uncheck it and click OK.</span></span>
  
 <span data-ttu-id="90757-113">**المحتوي في طريقه عرض محمية**</span><span class="sxs-lookup"><span data-stu-id="90757-113">**The content is in protected view**</span></span>
  
<span data-ttu-id="90757-114">يمكن ان تحتوي الملفات الموجودة علي الإنترنت ومن مواقع أخرى قد تكون غير أمنه علي فيروسات ، أو worms ، أو أنواع أخرى من البرامج الضارة التي قد تضر بالكمبيوتر لديك.</span><span class="sxs-lookup"><span data-stu-id="90757-114">Files from the Internet and from other potentially unsafe locations can contain viruses, worms, or other kinds of malware that can harm your computer.</span></span> <span data-ttu-id="90757-115">وهذا أيضا هو الحال مع مرفقات البريد الكتروني أو الملفات التي قمت بتنزيلها.</span><span class="sxs-lookup"><span data-stu-id="90757-115">This is also commonly the case with email attachments or files you've downloaded.</span></span> <span data-ttu-id="90757-116">للمساعدة في حماية الكمبيوتر ، يتم فتح الملفات من هذه المواقع التي قد تكون غير أمنه في "طريقه عرض محمية".</span><span class="sxs-lookup"><span data-stu-id="90757-116">To help protect your computer, files from these potentially unsafe locations are opened in Protected View.</span></span> <span data-ttu-id="90757-117">باستخدام طريقه عرض محمية ، يمكنك قراءه ملف وعرض محتوياته مع تقليل المخاطر.</span><span class="sxs-lookup"><span data-stu-id="90757-117">By using Protected View, you can read a file and see its contents while reducing the risks.</span></span> <span data-ttu-id="90757-118">لمزيد من المعلومات حول طريقه العرض المحمية وكيفيه تغيير الإعدادات ، راجع هذه المقالة: [ما هو "طريقه عرض محمية" ؟](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span><span class="sxs-lookup"><span data-stu-id="90757-118">For more information on Protected view and how to change settings, see this article: [What is Protected View?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span></span>
  
 <span data-ttu-id="90757-119">**هل هو OneDrive ممتلئ ؟**</span><span class="sxs-lookup"><span data-stu-id="90757-119">**Is OneDrive full?**</span></span>
  
<span data-ttu-id="90757-120">إذا تم تخزين الملف علي OneDrive وكانت مساحة تخزين OneDrive ممتلئة ، فلن تتمكن من حفظ المستند حتى تكون ضمن المساحة المخصصة.</span><span class="sxs-lookup"><span data-stu-id="90757-120">If the file is stored on OneDrive and your OneDrive storage space is full, you will be unable to save the document until you are under your allotted space.</span></span> <span data-ttu-id="90757-121">يمكنك التحقق من المساحة الحرة علي OneDrive بالنقر فوق أيقونه OneDrive في مركز الاعلامات واختيار أداره التخزين ، أو يمكنك [https://onedrive.live.com](https://onedrive.live.com) الانتقال إلى ، وتسجيل الدخول ، وملاحظه مقدار المساحة المستخدمة في الجزء السفلي الأيمن من الشاشة.</span><span class="sxs-lookup"><span data-stu-id="90757-121">You can check your free space on OneDrive by clicking the OneDrive icon in the notification center and choosing Manage storage, or you can go to [https://onedrive.live.com](https://onedrive.live.com), sign in, and note the amount of used space in the lower left of the screen.</span></span>
  
 <span data-ttu-id="90757-122">**هل تم تنشيط Office ؟**</span><span class="sxs-lookup"><span data-stu-id="90757-122">**Is Office activated?**</span></span>
  
<span data-ttu-id="90757-123">إذا لم يتم تنشيط Office ، أو إذا انتهت صلاحيه اشتراكك ، فيمكنك في وضع الأداء الوظيفي المنخفض للقراءة فقط.</span><span class="sxs-lookup"><span data-stu-id="90757-123">If Office is not activated, or if your subscription has expired, you could be in read-only Reduced Functionality Mode.</span></span> <span data-ttu-id="90757-124">للحصول علي معلومات حول كيفيه تنشيط Office ، راجع: [المنتج غير المرخص وأخطاء التنشيط في Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span><span class="sxs-lookup"><span data-stu-id="90757-124">For information on how to Activate Office, see: [Unlicensed Product and activation errors in Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>
  
 <span data-ttu-id="90757-125">**إذا فشل كل شيء آخر...**</span><span class="sxs-lookup"><span data-stu-id="90757-125">**If all else fails...**</span></span>
  
- <span data-ttu-id="90757-126">حاول أعاده تشغيل الكمبيوتر</span><span class="sxs-lookup"><span data-stu-id="90757-126">Try restarting the computer</span></span>
    
- <span data-ttu-id="90757-127">تثبيت تحديثات Office</span><span class="sxs-lookup"><span data-stu-id="90757-127">Install Office updates</span></span>
    
- <span data-ttu-id="90757-128">اجراء إصلاح عبر الإنترنت ل Office</span><span class="sxs-lookup"><span data-stu-id="90757-128">Perform an Online repair of Office</span></span>
    

