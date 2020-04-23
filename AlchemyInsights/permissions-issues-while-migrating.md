---
title: مشكلات الأذونات أثناء الترحيل
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: cbec51a7-5513-4848-a9ae-cdf993e000a8
ms.openlocfilehash: 077b7cf29ef6a40ef7f2aebef15e39a0f5df0fc3
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43758957"
---
# <a name="user-profile-and-photo-synchronization"></a><span data-ttu-id="05e9e-102">ملف تعريف المستخدم ومزامنة الصور</span><span class="sxs-lookup"><span data-stu-id="05e9e-102">User Profile and Photo synchronization</span></span>

 <span data-ttu-id="05e9e-103">**مزامنة صورة الملف الشخصي** - قد يلاحظ المستخدمون أن صورة ملفهم الشخصي لا تتم مزامنتها مع SharePoint.</span><span class="sxs-lookup"><span data-stu-id="05e9e-103">**Profile Photo Synchronization** - Users may notice that their profile photo is not synchronizing to SharePoint.</span></span> <span data-ttu-id="05e9e-104">أو ربما حاولوا تحديث صورة ملفهم الشخصي ولا تزال الصورة تظهر كالصورة القديمة.</span><span class="sxs-lookup"><span data-stu-id="05e9e-104">Or, they may have tried to update their profile photo and the photo still appears as the old photo.</span></span> <span data-ttu-id="05e9e-105">لضمان عرض صورة الملف الشخصي كما هو متوقع، سيحتاج المستخدم إلى بدء مزامنة صورة.</span><span class="sxs-lookup"><span data-stu-id="05e9e-105">To ensure the profile photo shows as expected, the user will need to initiate a photo sync.</span></span> 
  
<span data-ttu-id="05e9e-106">لمزيد من المعلومات حول عملية مزامنة الصور، راجع [معلومات حول مزامنة صورة الملف الشخصي في Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2022634)</span><span class="sxs-lookup"><span data-stu-id="05e9e-106">For more information about the photo synchronization process, see [Information about profile picture synchronization in Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2022634)</span></span>
  
- <span data-ttu-id="05e9e-107">**مزامنة ملف التعريف** - يعتمد الوقت المطلوب لإكمال مزامنة ملف التعريف على عدد التغييرات (العمل) التي يجب على مهمة استيراد الإعلانية معالجتها.</span><span class="sxs-lookup"><span data-stu-id="05e9e-107">**Profile Synchronization** - The time that's required to complete a profile synchronization depends on the number of changes (work) the AD Import Job has to process.</span></span> <span data-ttu-id="05e9e-108">إذا كان هناك العديد من التغييرات، فإن مهمة المؤقت لديها الكثير من العمل للقيام به، وسوف يستغرق وقتاً أطول للتغييرات أن تنعكس في تطبيق ملف تعريف المستخدم.</span><span class="sxs-lookup"><span data-stu-id="05e9e-108">If there are many changes, the timer job has a lot of work to do, and it will take longer for the changes to be reflected in the User Profile Application.</span></span> <span data-ttu-id="05e9e-109">إذا كان لمهمة المؤقت حجم صغير من العمل للقيام به، ستنعكس التغييرات في تطبيق ملف تعريف المستخدم بشكل أسرع بكثير.</span><span class="sxs-lookup"><span data-stu-id="05e9e-109">If the timer job has a small volume of work to do, the changes will be reflected in the User Profile Application much faster.</span></span> 
  
<span data-ttu-id="05e9e-110">لمزيد من المعلومات حول عملية مزامنة ملف التعريف، راجع [معلومات حول مزامنة ملف تعريف المستخدم في SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2022639)</span><span class="sxs-lookup"><span data-stu-id="05e9e-110">For more information about the profile synchronization process, see [Information about user profile synchronization in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2022639)</span></span>
    
- <span data-ttu-id="05e9e-111">**تحديث الملف الشخصي في Office Delve** - يمكن لمستخدمي Delve إدارة ملف تعريف Microsoft 365 الخاص بهم.</span><span class="sxs-lookup"><span data-stu-id="05e9e-111">**Update Profile in Office Delve** - Delve users can manage their Microsoft 365 Profile.</span></span> <span data-ttu-id="05e9e-112">لمزيد من المعلومات، راجع [عرض وتحديث ملفك الشخصي في Office Delve](https://support.office.com/article/View-and-update-your-profile-in-Office-Delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).</span><span class="sxs-lookup"><span data-stu-id="05e9e-112">For more information, see [View and Update your profile in Office Delve](https://support.office.com/article/View-and-update-your-profile-in-Office-Delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).</span></span>
    

