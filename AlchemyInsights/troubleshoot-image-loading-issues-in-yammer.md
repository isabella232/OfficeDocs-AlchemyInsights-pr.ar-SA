---
title: استكشاف مشكلات تحميل الصور وإصلاحها في Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6000"
- "9003112"
ms.openlocfilehash: 93894eaa5818b591acd1c7b9a90bc1cabbe00450
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148164"
---
# <a name="troubleshoot-image-loading-issues-in-yammer"></a><span data-ttu-id="45f5f-102">استكشاف مشكلات تحميل الصور وإصلاحها في Yammer</span><span class="sxs-lookup"><span data-stu-id="45f5f-102">Troubleshoot image loading issues in Yammer</span></span>

<span data-ttu-id="45f5f-103">عند حدوث مشكلات مع الصور ومعاينات الملفات في Yammer استكشاف الأخطاء وإصلاحها عن طريق التحقق من حدوث المشكلة لكافة المستخدمين، ما إذا كان يحدث على الأجهزة المحمولة، وإذا كان يمكن إعادة إنتاجها عند تحميل المرفق.</span><span class="sxs-lookup"><span data-stu-id="45f5f-103">When issues occur with photos and file previews in Yammer, troubleshoot by checking whether the issue occurs for all users, whether it occurs on mobile devices, and if it is reproducible when uploading the attachment.</span></span>  

<span data-ttu-id="45f5f-104">**مشكلات صورة الملف الشخصي**</span><span class="sxs-lookup"><span data-stu-id="45f5f-104">**Profile photo issues**</span></span>  

<span data-ttu-id="45f5f-105">إذا قام المستخدمون النهائيون بتسجيل الدخول إلى Yammer عبر Microsoft 365، فيجب عليهم تغيير ملفهم الشخصي، بما في ذلك صورة ملف التعريف الخاصة بهم.</span><span class="sxs-lookup"><span data-stu-id="45f5f-105">If end users sign into Yammer via Microsoft 365, they must change their profile, including their profile photo.</span></span> <span data-ttu-id="45f5f-106">إذا لم يُسمح للمستخدمين بإجراء تحديثات لملف التعريف، يمكن لمسؤول إجراء التحديث للمستخدم.</span><span class="sxs-lookup"><span data-stu-id="45f5f-106">If users are not permitted to make profile updates, an admin can make the update for the user.</span></span> <span data-ttu-id="45f5f-107">لمزيد من المعلومات، راجع [عرض ملف التعريف الخاص بك وتحديثه في Office Delve](https://support.microsoft.com/office/view-and-update-your-profile-in-office-delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).</span><span class="sxs-lookup"><span data-stu-id="45f5f-107">For more info, see [View and update your profile in Office Delve](https://support.microsoft.com/office/view-and-update-your-profile-in-office-delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).</span></span>

<span data-ttu-id="45f5f-108">للحصول على معلومات حول تحرير ملف التعريف، بما في ذلك صور الملف الشخصي، راجع [تغيير ملف تعريف Yammer وإعداداته](https://support.microsoft.com/office/classic-yammer-change-my-yammer-profile-and-settings-a3aeca0e-de34-4897-9b59-de6516542851).</span><span class="sxs-lookup"><span data-stu-id="45f5f-108">For info about profile editing, including profile photos, see [Change my Yammer profile and settings](https://support.microsoft.com/office/classic-yammer-change-my-yammer-profile-and-settings-a3aeca0e-de34-4897-9b59-de6516542851).</span></span> 

<span data-ttu-id="45f5f-109">تتم مزامنة صور ملف التعريف المحدثة بشكل مختلف عن سمات ملف التعريف.</span><span class="sxs-lookup"><span data-stu-id="45f5f-109">Updated profile photos are synced differently than profile attributes.</span></span> <span data-ttu-id="45f5f-110">يجب على المستخدمين تسجيل الدخول لبدء مزامنة لصورة ملفهم الشخصي.</span><span class="sxs-lookup"><span data-stu-id="45f5f-110">Users must sign in to initiate a sync of their profile photo.</span></span> <span data-ttu-id="45f5f-111">للحصول على معلومات، [راجع صور ملف تعريف المستخدم التي تم تحديثها من Office 365 إلى Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle#q-are-user-profile-pictures-updated-from-office-365-to-yammer).</span><span class="sxs-lookup"><span data-stu-id="45f5f-111">For info, see [are user profile pictures updated from Office 365 to Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle#q-are-user-profile-pictures-updated-from-office-365-to-yammer).</span></span>

<span data-ttu-id="45f5f-112">للحصول على معلومات حول دورة حياة المستخدم لـ Yammer، راجع [إدارة مستخدمي Yammer عبر دورة حياتهم من Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle).</span><span class="sxs-lookup"><span data-stu-id="45f5f-112">For info about the user lifecycle for Yammer, see [Manage Yammer users across their lifecycle from Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle).</span></span>  

<span data-ttu-id="45f5f-113">للحصول على تفاصيل حول كيفية عمل مزامنة صورة ملف التعريف في Microsoft 365، راجع [معلومات حول مزامنة صورة ملف التعريف في Microsoft 365](https://support.microsoft.com/office/information-about-profile-picture-synchronization-in-microsoft-365-20594d76-d054-4af4-a660-401133e3d48a).</span><span class="sxs-lookup"><span data-stu-id="45f5f-113">For details on how profile picture sync works in Microsoft 365, see [Information about profile picture synchronization in Microsoft 365](https://support.microsoft.com/office/information-about-profile-picture-synchronization-in-microsoft-365-20594d76-d054-4af4-a660-401133e3d48a).</span></span>  

<span data-ttu-id="45f5f-114">**معاينات المستندات وقضايا الصورة المصغرة**</span><span class="sxs-lookup"><span data-stu-id="45f5f-114">**Document previews and image thumbnail issues**</span></span>  

<span data-ttu-id="45f5f-115">عند نشر الملفات أو الصور إلى Yammer، قد لا تظهر المعاينات بسبب:</span><span class="sxs-lookup"><span data-stu-id="45f5f-115">When files or images are posted to Yammer, previews might not appear because:</span></span> 

- <span data-ttu-id="45f5f-116">الملف تالف ولا يمكن معالجته.</span><span class="sxs-lookup"><span data-stu-id="45f5f-116">The file is corrupt and cannot be processed.</span></span>
- <span data-ttu-id="45f5f-117">لم يتم تحميل الملف مؤخراً إلى SharePoint Online أو لدى Yammer بيانات تعريف غير صالحة لأسباب أخرى.</span><span class="sxs-lookup"><span data-stu-id="45f5f-117">The file has not been recently uploaded to SharePoint Online, or Yammer has invalid metadata for other reasons.</span></span>
- <span data-ttu-id="45f5f-118">يتم حظر عناوين URL المطلوبة لتحميل صور المعاينة.</span><span class="sxs-lookup"><span data-stu-id="45f5f-118">URLs required for loading the preview images are blocked.</span></span>
- <span data-ttu-id="45f5f-119">تمت إزالة معاينة الملف من قبل المستخدم قبل النشر.</span><span class="sxs-lookup"><span data-stu-id="45f5f-119">The file preview was removed by the user before posting.</span></span>
- <span data-ttu-id="45f5f-120">حالت مشكلة في الخدمة دون إنشاء معاينة.</span><span class="sxs-lookup"><span data-stu-id="45f5f-120">A service issue prevented a preview being generated.</span></span>

<span data-ttu-id="45f5f-121">**ملاحظة** قد تتصرف معاينات الارتباطات وتحميل الملفات بشكل مختلف.</span><span class="sxs-lookup"><span data-stu-id="45f5f-121">**Note** Previews for links and file uploads might behave differently.</span></span> <span data-ttu-id="45f5f-122">قد لا يتم عرض الارتباطات إلى ملفات على الإنترنت أو ارتباطات تتطلب مصادقة إضافية بشكل صحيح.</span><span class="sxs-lookup"><span data-stu-id="45f5f-122">Links to files on the internet or links that require additional authentication might not display correctly.</span></span>

<span data-ttu-id="45f5f-123">لمزيد من المعلومات، راجع [إرفاق ملف أو صورة برسالة Yammer](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-message-f576d4d1-ad66-4ce4-9c43-46cf75978dbf).</span><span class="sxs-lookup"><span data-stu-id="45f5f-123">For more info, see [Attach a file or image to a Yammer message](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-message-f576d4d1-ad66-4ce4-9c43-46cf75978dbf).</span></span> 