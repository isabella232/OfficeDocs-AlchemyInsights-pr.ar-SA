---
title: مشاكل الأذونات اثناء الترحيل
ms.author: pebaum
author: pebaum
ms.date: 9/18/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: cbec51a7-5513-4848-a9ae-cdf993e000a8
ms.openlocfilehash: 95bfbfdf002e457230479a860058c1cf7ab1f8c2
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/15/2019
ms.locfileid: "40054401"
---
# <a name="user-profile-and-photo-synchronization"></a><span data-ttu-id="18ae8-102">ملف تعريف المستخدم ومزامنة الصور</span><span class="sxs-lookup"><span data-stu-id="18ae8-102">User Profile and Photo synchronization</span></span>

 <span data-ttu-id="18ae8-103">**مزامنة الصور الشخصية** -قد يلاحظ المستخدمون ان صوره ملف التعريف الخاصة بهم لا يتم مزامنتها مع SharePoint.</span><span class="sxs-lookup"><span data-stu-id="18ae8-103">**Profile Photo Synchronization** - Users may notice that their profile photo is not synchronizing to SharePoint.</span></span> <span data-ttu-id="18ae8-104">أو ، قد حاولوا تحديث صورتهم الشخصية والصورة لا تزال تظهر كالصورة القديمة.</span><span class="sxs-lookup"><span data-stu-id="18ae8-104">Or, they may have tried to update their profile photo and the photo still appears as the old photo.</span></span> <span data-ttu-id="18ae8-105">لضمان إظهار صوره الملف الشخصي كما هو متوقع ، سيحتاج المستخدم إلى بدء مزامنة الصور.</span><span class="sxs-lookup"><span data-stu-id="18ae8-105">To ensure the profile photo shows as expected, the user will need to initiate a photo sync.</span></span> 
  
<span data-ttu-id="18ae8-106">لمزيد من المعلومات حول عمليه مزامنة الصور ، راجع [معلومات حول مزامنة صوره ملف التعريف في Office 365](https://go.microsoft.com/fwlink/?linkid=2022634)</span><span class="sxs-lookup"><span data-stu-id="18ae8-106">For more information about the photo synchronization process, see [Information about profile picture synchronization in Office 365](https://go.microsoft.com/fwlink/?linkid=2022634)</span></span>
  
- <span data-ttu-id="18ae8-107">**مزامنة ملف التعريف** -يعتمد الوقت المطلوب لإكمال مزامنة ملف التعريف علي عدد التغييرات (العمل) التي يجب ان تقوم مهمة استيراد AD بمعالجتها.</span><span class="sxs-lookup"><span data-stu-id="18ae8-107">**Profile Synchronization** - The time that's required to complete a profile synchronization depends on the number of changes (work) the AD Import Job has to process.</span></span> <span data-ttu-id="18ae8-108">إذا كان هناك العديد من التغييرات ، مهمة المؤقت لديه الكثير من العمل للقيام به ، وسوف يستغرق وقتا أطول للتغييرات التي ستنعكس في "تطبيق ملف تعريف المستخدم".</span><span class="sxs-lookup"><span data-stu-id="18ae8-108">If there are many changes, the timer job has a lot of work to do, and it will take longer for the changes to be reflected in the User Profile Application.</span></span> <span data-ttu-id="18ae8-109">إذا كانت مهمة المؤقت تحتوي علي حجم صغير من العمل للقيام به ، ستنعكس التغييرات في "تطبيق ملف تعريف المستخدم" بشكل أسرع بكثير.</span><span class="sxs-lookup"><span data-stu-id="18ae8-109">If the timer job has a small volume of work to do, the changes will be reflected in the User Profile Application much faster.</span></span> 
  
<span data-ttu-id="18ae8-110">لمزيد من المعلومات حول عمليه مزامنة ملف التعريف ، راجع [معلومات حول مزامنة ملف تعريف المستخدم في SharePoint علي الإنترنت](https://go.microsoft.com/fwlink/?linkid=2022639)</span><span class="sxs-lookup"><span data-stu-id="18ae8-110">For more information about the profile synchronization process, see [Information about user profile synchronization in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2022639)</span></span>
    
- <span data-ttu-id="18ae8-111">**تحديث ملف التعريف في office الخوض** -يمكن للمستخدمين أداره الملف الشخصي 365 office الخاصة بهم.</span><span class="sxs-lookup"><span data-stu-id="18ae8-111">**Update Profile in Office Delve** - Delve users can manage their Office 365 Profile.</span></span> <span data-ttu-id="18ae8-112">لمزيد من المعلومات ، راجع [عرض وتحديث ملف التعريف الخاص بك في الخوض في Office](https://support.office.com/article/View-and-update-your-profile-in-Office-Delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).</span><span class="sxs-lookup"><span data-stu-id="18ae8-112">For more information, see [View and Update your profile in Office Delve](https://support.office.com/article/View-and-update-your-profile-in-Office-Delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).</span></span>
    

