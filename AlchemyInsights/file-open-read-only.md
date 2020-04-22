---
title: ملف مفتوح للقراءة فقط
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 39748581-d319-403c-8501-9b785e4a0ed8
ms.custom:
- "765"
- "2200014"
ms.openlocfilehash: c045188af15fcec0f868eb0e5b399bd1fb42a09a
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43702761"
---
# <a name="file-open-read-only"></a><span data-ttu-id="fd536-102">ملف مفتوح للقراءة فقط</span><span class="sxs-lookup"><span data-stu-id="fd536-102">File open read-only</span></span>

<span data-ttu-id="fd536-103">قد تجد أنه عند فتح الملفات، فإنها تفتح كقراءة فقط.</span><span class="sxs-lookup"><span data-stu-id="fd536-103">You may find that when you are opening files, they open as read-only.</span></span> <span data-ttu-id="fd536-104">في بعض الحالات، هذا لمزيد من الأمان، مثل عند فتح الملفات من الإنترنت، وفي أوقات أخرى، يمكن أن يكون ذلك بسبب إعداد يمكن تغييره.</span><span class="sxs-lookup"><span data-stu-id="fd536-104">In some cases, this is for added security, such as when you are opening files from the internet, and other times, it can be due to a setting that can be changed.</span></span> <span data-ttu-id="fd536-105">فيما يلي بعض السيناريوهات حيث يفتح ملف للقراءة فقط وبعض الخطوات التي يمكنك اتخاذها لتغيير ذلك.</span><span class="sxs-lookup"><span data-stu-id="fd536-105">Here are some scenarios where a file opens read-only and some steps you can take to change that.</span></span>
  
 <span data-ttu-id="fd536-106">**يتسبب برنامج مكافحة الفيروسات في فتحها للقراءة فقط**</span><span class="sxs-lookup"><span data-stu-id="fd536-106">**My antivirus is causing them to open read-only**</span></span>
  
<span data-ttu-id="fd536-107">قد تحميك بعض برامج مكافحة الفيروسات من الملفات التي قد تكون غير آمنة عن طريق فتحها للقراءة فقط.</span><span class="sxs-lookup"><span data-stu-id="fd536-107">Some antivirus programs may protect you from potentially unsafe files by opening them read-only.</span></span> <span data-ttu-id="fd536-108">قد تحتاج إلى التحقق مع موفر مكافحة الفيروسات لمعرفة كيفية ضبط هذه الإعدادات.</span><span class="sxs-lookup"><span data-stu-id="fd536-108">You may need to check with your antivirus provider to learn how to adjust these settings.</span></span> <span data-ttu-id="fd536-109">BitDefender، على سبيل المثال، لديه محتوى على إضافة استثناءات التطبيق هنا: [كيفية إضافة تطبيقات أو معالجة الاستبعادات في مركز التحكم بيتدفندر](https://aka.ms/AA6098i).</span><span class="sxs-lookup"><span data-stu-id="fd536-109">BitDefender, for example, has content on adding application exclusions here: [How to add application or process exclusions in Bitdefender Control Center](https://aka.ms/AA6098i).</span></span>
  
 <span data-ttu-id="fd536-110">**هل تم تعيين خصائص الملف للقراءة فقط؟**</span><span class="sxs-lookup"><span data-stu-id="fd536-110">**Are the file properties set to read-only?**</span></span>
  
<span data-ttu-id="fd536-111">يمكنك التحقق من خصائص الملف عن طريق النقر بزر الماوس الأيمن على الملف واختيار الخصائص.</span><span class="sxs-lookup"><span data-stu-id="fd536-111">You can check the file properties by right-clicking on the file and choosing Properties.</span></span> <span data-ttu-id="fd536-112">إذا تم التحقق من السمة للقراءة فقط، يمكنك إلغاء تحديدها وانقر فوق موافق.</span><span class="sxs-lookup"><span data-stu-id="fd536-112">If the Read-only attribute is checked, you can uncheck it and click OK.</span></span>
  
 <span data-ttu-id="fd536-113">**المحتوى في طريقة عرض محمية**</span><span class="sxs-lookup"><span data-stu-id="fd536-113">**The content is in protected view**</span></span>
  
<span data-ttu-id="fd536-114">يمكن أن تحتوي الملفات من الإنترنت ومن مواقع أخرى قد تكون غير آمنة على فيروسات أو ديدان أو أنواع أخرى من البرامج الضارة التي يمكن أن تضر بالكمبيوتر.</span><span class="sxs-lookup"><span data-stu-id="fd536-114">Files from the Internet and from other potentially unsafe locations can contain viruses, worms, or other kinds of malware that can harm your computer.</span></span> <span data-ttu-id="fd536-115">هذا هو الحال عادة أيضا مع مرفقات البريد الإلكتروني أو الملفات التي قمت بتنزيلها.</span><span class="sxs-lookup"><span data-stu-id="fd536-115">This is also commonly the case with email attachments or files you've downloaded.</span></span> <span data-ttu-id="fd536-116">للمساعدة في حماية الكمبيوتر، يتم فتح ملفات من هذه المواقع التي قد تكون غير آمنة في "العرض المحمي".</span><span class="sxs-lookup"><span data-stu-id="fd536-116">To help protect your computer, files from these potentially unsafe locations are opened in Protected View.</span></span> <span data-ttu-id="fd536-117">باستخدام العرض المحمي، يمكنك قراءة ملف ورؤية محتوياته مع تقليل المخاطر.</span><span class="sxs-lookup"><span data-stu-id="fd536-117">By using Protected View, you can read a file and see its contents while reducing the risks.</span></span> <span data-ttu-id="fd536-118">لمزيد من المعلومات حول طريقة العرض المحمية وكيفية تغيير الإعدادات، راجع هذه المقالة: [ما هو العرض المحمي؟](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span><span class="sxs-lookup"><span data-stu-id="fd536-118">For more information on Protected view and how to change settings, see this article: [What is Protected View?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span></span>
  
 <span data-ttu-id="fd536-119">**هل OneDrive ممتلئ؟**</span><span class="sxs-lookup"><span data-stu-id="fd536-119">**Is OneDrive full?**</span></span>
  
<span data-ttu-id="fd536-120">إذا تم تخزين الملف على OneDrive وكانت مساحة تخزين OneDrive ممتلئة، فلن تتمكن من حفظ المستند حتى تكون تحت المساحة المخصصة.</span><span class="sxs-lookup"><span data-stu-id="fd536-120">If the file is stored on OneDrive and your OneDrive storage space is full, you will be unable to save the document until you are under your allotted space.</span></span> <span data-ttu-id="fd536-121">يمكنك التحقق من المساحة الحرة على OneDrive عن طريق النقر على رمز OneDrive [https://onedrive.live.com](https://onedrive.live.com)في مركز الإعلام واختيار إدارة التخزين ، أو يمكنك الانتقال إلى ، تسجيل الدخول ، وملاحظة مقدار المساحة المستخدمة في أسفل يسار الشاشة.</span><span class="sxs-lookup"><span data-stu-id="fd536-121">You can check your free space on OneDrive by clicking the OneDrive icon in the notification center and choosing Manage storage, or you can go to [https://onedrive.live.com](https://onedrive.live.com), sign in, and note the amount of used space in the lower left of the screen.</span></span>
  
 <span data-ttu-id="fd536-122">**هل تم تنشيط Office؟**</span><span class="sxs-lookup"><span data-stu-id="fd536-122">**Is Office activated?**</span></span>
  
<span data-ttu-id="fd536-123">إذا لم يتم تنشيط Office، أو إذا انتهت صلاحية اشتراكك، فقد تكون في وضع الأداء الوظيفي المنخفض للقراءة فقط.</span><span class="sxs-lookup"><span data-stu-id="fd536-123">If Office is not activated, or if your subscription has expired, you could be in read-only Reduced Functionality Mode.</span></span> <span data-ttu-id="fd536-124">للحصول على معلومات حول كيفية تنشيط Office، راجع: [أخطاء المنتج غير المرخص ة والتنشيط في Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span><span class="sxs-lookup"><span data-stu-id="fd536-124">For information on how to Activate Office, see: [Unlicensed Product and activation errors in Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>
  
 <span data-ttu-id="fd536-125">**إذا فشل كل شيء آخر...**</span><span class="sxs-lookup"><span data-stu-id="fd536-125">**If all else fails...**</span></span>
  
- <span data-ttu-id="fd536-126">حاول إعادة تشغيل الكمبيوتر</span><span class="sxs-lookup"><span data-stu-id="fd536-126">Try restarting the computer</span></span>
    
- <span data-ttu-id="fd536-127">تثبيت تحديثات Office</span><span class="sxs-lookup"><span data-stu-id="fd536-127">Install Office updates</span></span>
    
- <span data-ttu-id="fd536-128">إجراء إصلاح عبر الإنترنت للمكتب</span><span class="sxs-lookup"><span data-stu-id="fd536-128">Perform an Online repair of Office</span></span>
    

