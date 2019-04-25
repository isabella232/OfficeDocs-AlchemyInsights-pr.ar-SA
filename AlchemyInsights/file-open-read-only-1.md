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
ms.assetid: 69705825-723a-4c1e-ae85-d16b5051d2fe
ms.openlocfilehash: 117b1e24d6250a1d5eb092a01a0d5146d09ea2e5
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/23/2019
ms.locfileid: "32401624"
---
# <a name="file-open-read-only"></a><span data-ttu-id="65161-102">فتح الملف للقراءة فقط</span><span class="sxs-lookup"><span data-stu-id="65161-102">File open read-only</span></span>

<span data-ttu-id="65161-103">قد تجد أنه عند فتح ملفات، فتح للقراءة فقط.</span><span class="sxs-lookup"><span data-stu-id="65161-103">You may find that when you are opening files, they open as read-only.</span></span> <span data-ttu-id="65161-104">في بعض الحالات، وهذا لمزيد من الأمان، مثل عند فتح الملفات من الإنترنت، وفي أوقات أخرى، فإنه يمكن أن يكون سبب إعداد التي يمكن تغييرها.</span><span class="sxs-lookup"><span data-stu-id="65161-104">In some cases, this is for added security, such as when you are opening files from the internet, and other times, it can be due to a setting that can be changed.</span></span> <span data-ttu-id="65161-105">فيما يلي بعض السيناريوهات حيث يفتح ملف القراءة فقط وبعض الخطوات التي يمكنك اتخاذها لتغيير ذلك.</span><span class="sxs-lookup"><span data-stu-id="65161-105">Here are some scenarios where a file opens read-only and some steps you can take to change that.</span></span>
  
 <span data-ttu-id="65161-106">**برنامج مكافحة الفيروسات الخاص بي هو مما أدى إلى فتح للقراءة فقط**</span><span class="sxs-lookup"><span data-stu-id="65161-106">**My antivirus is causing them to open read-only**</span></span>
  
<span data-ttu-id="65161-107">بعض برامج مكافحة الفيروسات قد حماية من الملفات غير الآمنة بفتحها في القراءة فقط.</span><span class="sxs-lookup"><span data-stu-id="65161-107">Some antivirus programs may protect you from potentially unsafe files by opening them read-only.</span></span> <span data-ttu-id="65161-108">قد تحتاج إلى التحقق بواسطة موفر برامج مكافحة الفيروسات لمعرفة كيفية ضبط هذه الإعدادات.</span><span class="sxs-lookup"><span data-stu-id="65161-108">You may need to check with your antivirus provider to learn how to adjust these settings.</span></span> <span data-ttu-id="65161-109">بيتدفندر، على سبيل المثال، يحتوي المحتوى على إضافة استثناءات التطبيق هنا: [كيفية إضافة التطبيق أو معالجة الاستثناءات في مركز التحكم بيتدفندر](https://www.bitdefender.com/support/how-to-add-application-or-process-exclusions-in-bitdefender-control-center-1119.mdl).</span><span class="sxs-lookup"><span data-stu-id="65161-109">BitDefender, for example, has content on adding application exclusions here: [How to add application or process exclusions in Bitdefender Control Center](https://www.bitdefender.com/support/how-to-add-application-or-process-exclusions-in-bitdefender-control-center-1119.mdl).</span></span>
  
 <span data-ttu-id="65161-110">**خصائص الملف معدّة القراءة فقط؟**</span><span class="sxs-lookup"><span data-stu-id="65161-110">**Are the file properties set to read-only?**</span></span>
  
<span data-ttu-id="65161-111">يمكنك التحقق من خصائص الملف عن طريق النقر بالزر الأيمن على الملف واختيار خصائص.</span><span class="sxs-lookup"><span data-stu-id="65161-111">You can check the file properties by right-clicking on the file and choosing Properties.</span></span> <span data-ttu-id="65161-112">إذا تم تحديد سمة القراءة فقط، يمكنك قم بإلغاء تحديده وانقر فوق موافق.</span><span class="sxs-lookup"><span data-stu-id="65161-112">If the Read-only attribute is checked, you can uncheck it and click OK.</span></span>
  
 <span data-ttu-id="65161-113">**كان المحتوى في طريقة عرض محمية**</span><span class="sxs-lookup"><span data-stu-id="65161-113">**The content is in protected view**</span></span>
  
<span data-ttu-id="65161-114">يمكن أن تحتوي الملفات من الإنترنت ومن مواقع أخرى قد تكون غير آمنة على الفيروسات والفيروسات المتنقلة، أو أنواع أخرى من البرامج الضارة التي يمكن أن تضر الكمبيوتر.</span><span class="sxs-lookup"><span data-stu-id="65161-114">Files from the Internet and from other potentially unsafe locations can contain viruses, worms, or other kinds of malware that can harm your computer.</span></span> <span data-ttu-id="65161-115">وهذا أيضا عادة الحالة مع مرفقات البريد الإلكتروني أو الملفات التي قمت بتنزيله.</span><span class="sxs-lookup"><span data-stu-id="65161-115">This is also commonly the case with email attachments or files you've downloaded.</span></span> <span data-ttu-id="65161-116">للمساعدة على حماية جهاز الكمبيوتر الخاص بك، يتم فتح الملفات من هذه المواقع غير الآمنة في "طريقة عرض محمية".</span><span class="sxs-lookup"><span data-stu-id="65161-116">To help protect your computer, files from these potentially unsafe locations are opened in Protected View.</span></span> <span data-ttu-id="65161-117">باستخدام "طريقة عرض محمية"، يمكنك قراءة ملف وعرض محتوياته مع الحد من المخاطر.</span><span class="sxs-lookup"><span data-stu-id="65161-117">By using Protected View, you can read a file and see its contents while reducing the risks.</span></span> <span data-ttu-id="65161-118">لمزيد من المعلومات حول عرض محمي وكيفية تغيير الإعدادات، راجع هذا المقال: [ما هو "طريقة عرض محمية"؟](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span><span class="sxs-lookup"><span data-stu-id="65161-118">For more information on Protected view and how to change settings, see this article: [What is Protected View?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span></span>
  
 <span data-ttu-id="65161-119">**ممتلئ أندريف؟**</span><span class="sxs-lookup"><span data-stu-id="65161-119">**Is OneDrive full?**</span></span>
  
<span data-ttu-id="65161-120">إذا تم تخزين الملف على أندريف ومساحة التخزين أندريف كامل، لن تتمكن من حفظ المستند حتى تكون ضمن المساحة المخصصة الخاصة بك.</span><span class="sxs-lookup"><span data-stu-id="65161-120">If the file is stored on OneDrive and your OneDrive storage space is full, you will be unable to save the document until you are under your allotted space.</span></span> <span data-ttu-id="65161-121">يمكنك التحقق من المساحة الحرة على أونيدريفي عن طريق النقر فوق رمز أونيدريفي في مركز الإعلام واختيار إدارة التخزين، أو يمكنك الانتقال إلى [http://onedrive.live.com](http://onedrive.live.com)وتسجيل الدخول، ولاحظ مقدار المساحة المستخدمة في أسفل يمين الشاشة.</span><span class="sxs-lookup"><span data-stu-id="65161-121">You can check your free space on OneDrive by clicking the OneDrive icon in the notification center and choosing Manage storage, or you can go to [http://onedrive.live.com](http://onedrive.live.com), sign in, and note the amount of used space in the lower left of the screen.</span></span>
  
 <span data-ttu-id="65161-122">**تنشيط برنامج Office**</span><span class="sxs-lookup"><span data-stu-id="65161-122">**Is Office activated?**</span></span>
  
<span data-ttu-id="65161-123">إذا لم يتم تنشيط Office، أو إذا انتهت صلاحية الاشتراك الخاص بك، قد يكون في القراءة فقط "وضع الأداء الوظيفي المنخفض".</span><span class="sxs-lookup"><span data-stu-id="65161-123">If Office is not activated, or if your subscription has expired, you could be in read-only Reduced Functionality Mode.</span></span> <span data-ttu-id="65161-124">لمزيد من المعلومات حول كيفية تنشيط Office، راجع: ["المنتج غير مرخص" وتنشيط الأخطاء في Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span><span class="sxs-lookup"><span data-stu-id="65161-124">For information on how to Activate Office, see: [Unlicensed Product and activation errors in Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>
  
 <span data-ttu-id="65161-125">**إذا فشل كل شيء آخر...**</span><span class="sxs-lookup"><span data-stu-id="65161-125">**If all else fails...**</span></span>
  
- <span data-ttu-id="65161-126">حاول إعادة تشغيل الكمبيوتر</span><span class="sxs-lookup"><span data-stu-id="65161-126">Try restarting the computer</span></span>
    
- <span data-ttu-id="65161-127">تثبيت تحديثات Office</span><span class="sxs-lookup"><span data-stu-id="65161-127">Install Office updates</span></span>
    
- <span data-ttu-id="65161-128">إجراء إصلاح على إنترنت لمكتب</span><span class="sxs-lookup"><span data-stu-id="65161-128">Perform an Online repair of Office</span></span>
    

