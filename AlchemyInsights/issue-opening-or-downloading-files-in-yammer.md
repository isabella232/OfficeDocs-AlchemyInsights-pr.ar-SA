---
title: مشكله في فتح الملفات أو تنزيلها في Yammer
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
- "6041"
- "9003112"
ms.openlocfilehash: de335e27624caf5a91bdc2913570eba92f627282
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695636"
---
# <a name="issue-opening-or-downloading-files-in-yammer"></a><span data-ttu-id="f3b18-102">مشكله في فتح الملفات أو تنزيلها في Yammer</span><span class="sxs-lookup"><span data-stu-id="f3b18-102">Issue opening or downloading files in Yammer</span></span>

<span data-ttu-id="f3b18-103">يدعم Yammer الكلاسيكي خيارات متعددة لتحميل الملفات إلى الرسائل والمجموعات.</span><span class="sxs-lookup"><span data-stu-id="f3b18-103">Classic Yammer supports multiple option for file uploads to messages and groups.</span></span> <span data-ttu-id="f3b18-104">وفقا لتكوين الشبكة ، الملفات الافتراضية للتخزين في SharePoint.</span><span class="sxs-lookup"><span data-stu-id="f3b18-104">Depending on network configuration, files default to storage in SharePoint.</span></span>

<span data-ttu-id="f3b18-105">لا يدعم منتقي الملفات في Yammer الجديد بعد كل الخيارات المتوفرة في Yammer الكلاسيكي.</span><span class="sxs-lookup"><span data-stu-id="f3b18-105">The file picker in new Yammer does not yet support all the options available in classic Yammer.</span></span> <span data-ttu-id="f3b18-106">سيقوم التحديث المستقبلي باضافه ميزات اضافيه.</span><span class="sxs-lookup"><span data-stu-id="f3b18-106">A future update will add additional features.</span></span> <span data-ttu-id="f3b18-107">للحصول علي مزيد من المعلومات ، راجع [إرفاق ملف أو صوره بمنشور محادثه Yammer](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8).</span><span class="sxs-lookup"><span data-stu-id="f3b18-107">For more info, see [Attach a file or image to a Yammer conversation post](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8).</span></span>

<span data-ttu-id="f3b18-108">**تعذر فتح ملف أو تنزيله**</span><span class="sxs-lookup"><span data-stu-id="f3b18-108">**Unable to open or download a file**</span></span>  

<span data-ttu-id="f3b18-109">قد يتم تحميل ملف إلى Yammer ولكنه أيضا يكون مرتبطا بملف في SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="f3b18-109">A file might upload to Yammer but also be linking to a file in SharePoint Online.</span></span> <span data-ttu-id="f3b18-110">لاستكشاف الأخطاء وإصلاحها ، يجب عليك أولا تحديد موقع الملف.</span><span class="sxs-lookup"><span data-stu-id="f3b18-110">To troubleshoot, first you must determine the location of the file.</span></span> <span data-ttu-id="f3b18-111">إذا تم تحميل الملف إلى Yammer ، سيكون لديه عنوان URL \* yammer.com.</span><span class="sxs-lookup"><span data-stu-id="f3b18-111">If the file has been uploaded to Yammer, it will have a \*.yammer.com URL.</span></span> <span data-ttu-id="f3b18-112">تاكد من إلغاء حظر عناوين Url و IP المطلوبة.</span><span class="sxs-lookup"><span data-stu-id="f3b18-112">Ensure that required URLs and IP addresses are unblocked.</span></span> <span data-ttu-id="f3b18-113">للحصول علي مزيد من المعلومات ، راجع منشور المدونة [باستخدام عناوين IP المرمزة بشكل ثابت ل Yammer غير مستحسن](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592).</span><span class="sxs-lookup"><span data-stu-id="f3b18-113">For more info, see the blog post [Using hard coded IP addresses for Yammer is not recommended](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592).</span></span>

<span data-ttu-id="f3b18-114">تحقق مما إذا كان بإمكان المستخدم الذي يملك المسؤول العام تنزيل الملف.</span><span class="sxs-lookup"><span data-stu-id="f3b18-114">Check whether a user who is also a global admin can download the file.</span></span> <span data-ttu-id="f3b18-115">إذا كان الملف خاصا ، فقد تحتاج إلى استخدام وضع المحتوي الخاص.</span><span class="sxs-lookup"><span data-stu-id="f3b18-115">If the file is private, you might have to use Private Content Mode.</span></span> <span data-ttu-id="f3b18-116">للحصول علي مزيد من المعلومات ، راجع [عرض المحتوي الخاص في Yammer](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content).</span><span class="sxs-lookup"><span data-stu-id="f3b18-116">For more info, see then [Monitor private content in Yammer](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content).</span></span>  

<span data-ttu-id="f3b18-117">**Yammer علي مستوي الشبكة والملفات في SharePoint Online**</span><span class="sxs-lookup"><span data-stu-id="f3b18-117">**Yammer network-level guests and files in SharePoint Online**</span></span>  

<span data-ttu-id="f3b18-118">لا تستخدم [الضيوف علي مستوي الشبكة في Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) الخاص ب AZURE AD B2B وتكون داخلية لخدمه yammer ، التالي لا يمكنهم الوصول إلى ملفات yammer المخزنة في SharePoint.</span><span class="sxs-lookup"><span data-stu-id="f3b18-118">[Network-level guests in Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) do not use Azure AD B2B and are internal to the Yammer service, so they can't access Yammer files stored in SharePoint.</span></span> <span data-ttu-id="f3b18-119">يمكنك إنشاء مستخدم خاص بموقع AAD الخارجي الذي يمكنه الوصول إلى مكتبات المستندات في SharePoint Online باستخدام تلك الهوية.</span><span class="sxs-lookup"><span data-stu-id="f3b18-119">Create an external AAD B2B user who can access document libraries in SharePoint Online by using that identity.</span></span> <span data-ttu-id="f3b18-120">للحصول علي معلومات حول دعم الضيوف المستقبلي في Azure AD B2B في Yammer ، راجع [دعم الضيف للشركات (B2B) في معاينه Yammer-شروط العميل والاسئله المتداولة](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer).</span><span class="sxs-lookup"><span data-stu-id="f3b18-120">For information about future Azure AD B2B guest support in Yammer, see [Business-to-business (B2B) Guest support in Yammer Preview - Customer Terms and FAQ](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer).</span></span>