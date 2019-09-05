---
title: مشاكل الأذونات أثناء الترحيل
ms.author: pebaum
author: Techwriter40
ms.date: 9/18/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: cbec51a7-5513-4848-a9ae-cdf993e000a8
ms.openlocfilehash: 33e605ff3019f52bbd0be876d485ff389b260a44
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/04/2019
ms.locfileid: "36752595"
---
# <a name="user-profile-and-photo-synchronization"></a><span data-ttu-id="1be75-102">مزامنة ملف تعريف المستخدم والصور</span><span class="sxs-lookup"><span data-stu-id="1be75-102">User Profile and Photo synchronization</span></span>

 <span data-ttu-id="1be75-103">**مزامنة صور ملف التعريف** - قد يلاحظ المستخدمون أن صورة ملف التعريف الخاص بهم لا تتم مزامنتها مع SharePoint.</span><span class="sxs-lookup"><span data-stu-id="1be75-103">**Profile Photo Synchronization** - Users may notice that their profile photo is not synchronizing to SharePoint.</span></span> <span data-ttu-id="1be75-104">أو، ربما حاولوا تحديث صورة ملفهم الشخصي ولا تزال الصورة تظهر كصورة قديمة.</span><span class="sxs-lookup"><span data-stu-id="1be75-104">Or, they may have tried to update their profile photo and the photo still appears as the old photo.</span></span> <span data-ttu-id="1be75-105">لضمان عرض صورة الملف الشخصي كما هو متوقع، سيحتاج المستخدم إلى بدء مزامنة الصور.</span><span class="sxs-lookup"><span data-stu-id="1be75-105">To ensure the profile photo shows as expected, the user will need to initiate a photo sync.</span></span> 
  
<span data-ttu-id="1be75-106">لمزيد من المعلومات حول عملية مزامنة الصور، راجع [معلومات حول مزامنة صورة ملف التعريف في Office 365](https://go.microsoft.com/fwlink/?linkid=2022634)</span><span class="sxs-lookup"><span data-stu-id="1be75-106">For more information about the photo synchronization process, see [Information about profile picture synchronization in Office 365](https://go.microsoft.com/fwlink/?linkid=2022634)</span></span>
  
- <span data-ttu-id="1be75-107">**مزامنة ملف التعريف** - يعتمد الوقت المطلوب لإكمال مزامنة ملف تعريف على عدد التغييرات (العمل) التي يجب على AD Import Job معالجتها.</span><span class="sxs-lookup"><span data-stu-id="1be75-107">**Profile Synchronization** - The time that's required to complete a profile synchronization depends on the number of changes (work) the AD Import Job has to process.</span></span> <span data-ttu-id="1be75-108">إذا كان هناك العديد من التغييرات، مهمة المؤقت لديه الكثير من العمل للقيام به، وسوف يستغرق وقتاً أطول للتغييرات أن تنعكس في "تطبيق ملف تعريف المستخدم".</span><span class="sxs-lookup"><span data-stu-id="1be75-108">If there are many changes, the timer job has a lot of work to do, and it will take longer for the changes to be reflected in the User Profile Application.</span></span> <span data-ttu-id="1be75-109">إذا كانت مهمة جهاز ضبط الوقت يحتوي على حجم صغير من العمل للقيام به، سيتم عكس التغييرات في "تطبيق ملف تعريف المستخدم" أسرع بكثير.</span><span class="sxs-lookup"><span data-stu-id="1be75-109">If the timer job has a small volume of work to do, the changes will be reflected in the User Profile Application much faster.</span></span> 
  
<span data-ttu-id="1be75-110">لمزيد من المعلومات حول عملية مزامنة ملف التعريف، راجع [معلومات حول مزامنة ملف تعريف المستخدم في SharePoint على الإنترنت](https://go.microsoft.com/fwlink/?linkid=2022639)</span><span class="sxs-lookup"><span data-stu-id="1be75-110">For more information about the profile synchronization process, see [Information about user profile synchronization in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2022639)</span></span>
    
- <span data-ttu-id="1be75-111">**تحديث ملف التعريف في Office Delve** - يمكن للمستخدمين Delve إدارة ملف تعريف Office 365 الخاص بهم.</span><span class="sxs-lookup"><span data-stu-id="1be75-111">**Update Profile in Office Delve** - Delve users can manage their Office 365 Profile.</span></span> <span data-ttu-id="1be75-112">لمزيد من المعلومات، راجع [عرض ملفالتعريف الخاص بك وتحديثه في Office Delve](https://support.office.com/article/View-and-update-your-profile-in-Office-Delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).</span><span class="sxs-lookup"><span data-stu-id="1be75-112">For more information, see [View and Update your profile in Office Delve](https://support.office.com/article/View-and-update-your-profile-in-Office-Delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).</span></span>
    

