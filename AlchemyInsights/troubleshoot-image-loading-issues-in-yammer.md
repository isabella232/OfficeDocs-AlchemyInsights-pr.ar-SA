---
title: استكشاف مشاكل تحميل الصور وإصلاحها في Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6000"
- "9003112"
ms.openlocfilehash: cf330adbf3f3a92d4b90768c7dd8bada6333db80
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690230"
---
# <a name="troubleshoot-image-loading-issues-in-yammer"></a><span data-ttu-id="bb909-102">استكشاف مشاكل تحميل الصور وإصلاحها في Yammer</span><span class="sxs-lookup"><span data-stu-id="bb909-102">Troubleshoot image loading issues in Yammer</span></span>

<span data-ttu-id="bb909-103">عند حدوث مشاكل في الصور ومعاينه الملفات في Yammer ، يمكن استكشاف الأخطاء وإصلاحها من خلال التحقق مما إذا كانت المشكلة تحدث لجميع المستخدمين ، سواء تحدث علي الاجهزه المحمولة ، وإذا كانت قابله لأعاده الاستخدام عند تحميل المرفق.</span><span class="sxs-lookup"><span data-stu-id="bb909-103">When issues occur with photos and file previews in Yammer, troubleshoot by checking whether the issue occurs for all users, whether it occurs on mobile devices, and if it is reproducible when uploading the attachment.</span></span>  

<span data-ttu-id="bb909-104">**مشاكل صور ملف التعريف**</span><span class="sxs-lookup"><span data-stu-id="bb909-104">**Profile photo issues**</span></span>  

<span data-ttu-id="bb909-105">إذا قام المستخدمون بتسجيل الدخول إلى Yammer عبر Microsoft 365 ، فيجب تغيير ملف التعريف الخاص بهم ، بما في ذلك صوره ملف التعريف الخاص بهم.</span><span class="sxs-lookup"><span data-stu-id="bb909-105">If end users sign into Yammer via Microsoft 365, they must change their profile, including their profile photo.</span></span> <span data-ttu-id="bb909-106">إذا لم يسمح للمستخدمين باجراء تحديثات لملف التعريف ، فبامكان المسؤول اجراء التحديث للمستخدم.</span><span class="sxs-lookup"><span data-stu-id="bb909-106">If users are not permitted to make profile updates, an admin can make the update for the user.</span></span> <span data-ttu-id="bb909-107">للحصول علي مزيد من المعلومات ، راجع [عرض ملف التعريف وتحديثه في Office Delve](https://support.microsoft.com/office/view-and-update-your-profile-in-office-delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).</span><span class="sxs-lookup"><span data-stu-id="bb909-107">For more info, see [View and update your profile in Office Delve](https://support.microsoft.com/office/view-and-update-your-profile-in-office-delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).</span></span>

<span data-ttu-id="bb909-108">للحصول علي معلومات حول تحرير ملف التعريف ، بما في ذلك صور ملفات التعريف ، راجع [تغيير ملف تعريف Yammer وإعداداته](https://support.microsoft.com/office/classic-yammer-change-my-yammer-profile-and-settings-a3aeca0e-de34-4897-9b59-de6516542851).</span><span class="sxs-lookup"><span data-stu-id="bb909-108">For info about profile editing, including profile photos, see [Change my Yammer profile and settings](https://support.microsoft.com/office/classic-yammer-change-my-yammer-profile-and-settings-a3aeca0e-de34-4897-9b59-de6516542851).</span></span> 

<span data-ttu-id="bb909-109">تتم مزامنة صور ملف التعريف المحدثة بطريقه مختلفه عن سمات التشكيل الجانبي.</span><span class="sxs-lookup"><span data-stu-id="bb909-109">Updated profile photos are synced differently than profile attributes.</span></span> <span data-ttu-id="bb909-110">يجب علي المستخدمين تسجيل الدخول لبدء مزامنة صوره ملف التعريف الخاصة بهم.</span><span class="sxs-lookup"><span data-stu-id="bb909-110">Users must sign in to initiate a sync of their profile photo.</span></span> <span data-ttu-id="bb909-111">للحصول علي معلومات ، راجع [هل تم تحديث صور ملفات تعريف المستخدمين من Office 365 إلى Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle#q-are-user-profile-pictures-updated-from-office-365-to-yammer).</span><span class="sxs-lookup"><span data-stu-id="bb909-111">For info, see [are user profile pictures updated from Office 365 to Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle#q-are-user-profile-pictures-updated-from-office-365-to-yammer).</span></span>

<span data-ttu-id="bb909-112">للحصول علي معلومات حول دوره حياه المستخدم ل Yammer ، راجع [أداره مستخدمي yammer عبر دوره الحياة الخاصة بهم من Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle).</span><span class="sxs-lookup"><span data-stu-id="bb909-112">For info about the user lifecycle for Yammer, see [Manage Yammer users across their lifecycle from Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle).</span></span>  

<span data-ttu-id="bb909-113">للحصول علي تفاصيل حول كيفيه عمل مزامنة صوره ملف التعريف في Microsoft 365 ، راجع [المعلومات حول مزامنة صوره ملف التعريف في microsoft 365](https://support.microsoft.com/office/information-about-profile-picture-synchronization-in-microsoft-365-20594d76-d054-4af4-a660-401133e3d48a).</span><span class="sxs-lookup"><span data-stu-id="bb909-113">For details on how profile picture sync works in Microsoft 365, see [Information about profile picture synchronization in Microsoft 365](https://support.microsoft.com/office/information-about-profile-picture-synchronization-in-microsoft-365-20594d76-d054-4af4-a660-401133e3d48a).</span></span>  

<span data-ttu-id="bb909-114">**مشاكل معاينه المستندات والصور المصغرة**</span><span class="sxs-lookup"><span data-stu-id="bb909-114">**Document previews and image thumbnail issues**</span></span>  

<span data-ttu-id="bb909-115">عند نشر الملفات أو الصور إلى Yammer ، قد لا تظهر المعاينات بسبب:</span><span class="sxs-lookup"><span data-stu-id="bb909-115">When files or images are posted to Yammer, previews might not appear because:</span></span> 

- <span data-ttu-id="bb909-116">الملف تالف ولا يمكن معالجته.</span><span class="sxs-lookup"><span data-stu-id="bb909-116">The file is corrupt and cannot be processed.</span></span>
- <span data-ttu-id="bb909-117">لم يتم تحميل الملف مؤخرا إلى SharePoint Online ، أو يحتوي Yammer علي بيانات تعريف غير صالحه لأسباب أخرى.</span><span class="sxs-lookup"><span data-stu-id="bb909-117">The file has not been recently uploaded to SharePoint Online, or Yammer has invalid metadata for other reasons.</span></span>
- <span data-ttu-id="bb909-118">يتم حظر عناوين Url المطلوبة لتحميل صور المعاينة.</span><span class="sxs-lookup"><span data-stu-id="bb909-118">URLs required for loading the preview images are blocked.</span></span>
- <span data-ttu-id="bb909-119">تمت أزاله معاينه الملف بواسطة المستخدم قبل النشر.</span><span class="sxs-lookup"><span data-stu-id="bb909-119">The file preview was removed by the user before posting.</span></span>
- <span data-ttu-id="bb909-120">مشكله في الخدمة تسببت في منع إنشاء معاينه.</span><span class="sxs-lookup"><span data-stu-id="bb909-120">A service issue prevented a preview being generated.</span></span>

<span data-ttu-id="bb909-121">**ملاحظه** قد تتصرف المعاينات للارتباطات وتحميلات الملفات بطريقه مختلفه.</span><span class="sxs-lookup"><span data-stu-id="bb909-121">**Note** Previews for links and file uploads might behave differently.</span></span> <span data-ttu-id="bb909-122">قد لا يتم عرض الارتباطات الخاصة بالملفات الموجودة علي الإنترنت أو الارتباطات التي تتطلب مصادقه اضافيه بشكل صحيح.</span><span class="sxs-lookup"><span data-stu-id="bb909-122">Links to files on the internet or links that require additional authentication might not display correctly.</span></span>

<span data-ttu-id="bb909-123">للحصول علي مزيد من المعلومات ، راجع [إرفاق ملف أو صوره برسالة Yammer](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-message-f576d4d1-ad66-4ce4-9c43-46cf75978dbf).</span><span class="sxs-lookup"><span data-stu-id="bb909-123">For more info, see [Attach a file or image to a Yammer message](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-message-f576d4d1-ad66-4ce4-9c43-46cf75978dbf).</span></span> 