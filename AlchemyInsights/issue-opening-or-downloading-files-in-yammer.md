---
title: مشكلة فتح الملفات أو تنزيلها في Yammer
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
- "6041"
- "9003112"
ms.openlocfilehash: 6dfcbe9abfc23219a61e81785d31c11f7a0fa95c
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148168"
---
# <a name="issue-opening-or-downloading-files-in-yammer"></a><span data-ttu-id="4bca6-102">مشكلة فتح الملفات أو تنزيلها في Yammer</span><span class="sxs-lookup"><span data-stu-id="4bca6-102">Issue opening or downloading files in Yammer</span></span>

<span data-ttu-id="4bca6-103">يدعم Yammer الكلاسيكي خيارًا متعددًا لتحميل الملفات إلى الرسائل والمجموعات.</span><span class="sxs-lookup"><span data-stu-id="4bca6-103">Classic Yammer supports multiple option for file uploads to messages and groups.</span></span> <span data-ttu-id="4bca6-104">اعتماداً على تكوين شبكة الاتصال، الافتراضي الملفات إلى التخزين في SharePoint.</span><span class="sxs-lookup"><span data-stu-id="4bca6-104">Depending on network configuration, files default to storage in SharePoint.</span></span>

<span data-ttu-id="4bca6-105">لا يعتمد منتقي الملفات في Yammer الجديدة بعد كافة الخيارات المتوفرة في Yammer الكلاسيكية.</span><span class="sxs-lookup"><span data-stu-id="4bca6-105">The file picker in new Yammer does not yet support all the options available in classic Yammer.</span></span> <span data-ttu-id="4bca6-106">سوف يضيف التحديث المستقبلي ميزات إضافية.</span><span class="sxs-lookup"><span data-stu-id="4bca6-106">A future update will add additional features.</span></span> <span data-ttu-id="4bca6-107">لمزيد من المعلومات، راجع [إرفاق ملف أو صورة إلى مشاركة محادثة Yammer](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8).</span><span class="sxs-lookup"><span data-stu-id="4bca6-107">For more info, see [Attach a file or image to a Yammer conversation post](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8).</span></span>

<span data-ttu-id="4bca6-108">**تعذر فتح ملف أو تنزيله**</span><span class="sxs-lookup"><span data-stu-id="4bca6-108">**Unable to open or download a file**</span></span>  

<span data-ttu-id="4bca6-109">قد يتم تحميل ملف إلى Yammer ولكن أيضاً الارتباط بملف في SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="4bca6-109">A file might upload to Yammer but also be linking to a file in SharePoint Online.</span></span> <span data-ttu-id="4bca6-110">لاستكشاف الأخطاء وإصلاحها، يجب أولاً تحديد موقع الملف.</span><span class="sxs-lookup"><span data-stu-id="4bca6-110">To troubleshoot, first you must determine the location of the file.</span></span> <span data-ttu-id="4bca6-111">إذا تم تحميل الملف إلى Yammer، سيكون له عنوان URL \*.yammer.com.</span><span class="sxs-lookup"><span data-stu-id="4bca6-111">If the file has been uploaded to Yammer, it will have a \*.yammer.com URL.</span></span> <span data-ttu-id="4bca6-112">تأكد من إلغاء حظر عناوين URL وعناوين IP المطلوبة.</span><span class="sxs-lookup"><span data-stu-id="4bca6-112">Ensure that required URLs and IP addresses are unblocked.</span></span> <span data-ttu-id="4bca6-113">لمزيد من المعلومات، راجع نشر المدونة [باستخدام عناوين IP المشفرة الثابتة لـ Yammer غير مستحسن](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592).</span><span class="sxs-lookup"><span data-stu-id="4bca6-113">For more info, see the blog post [Using hard coded IP addresses for Yammer is not recommended](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592).</span></span>

<span data-ttu-id="4bca6-114">تحقق من ما إذا كان بإمكان المستخدم الذي هو مسؤول عمومي أيضًا تنزيل الملف.</span><span class="sxs-lookup"><span data-stu-id="4bca6-114">Check whether a user who is also a global admin can download the file.</span></span> <span data-ttu-id="4bca6-115">إذا كان الملف خاصًا، قد تحتاج إلى استخدام وضع المحتوى الخاص.</span><span class="sxs-lookup"><span data-stu-id="4bca6-115">If the file is private, you might have to use Private Content Mode.</span></span> <span data-ttu-id="4bca6-116">لمزيد من المعلومات، راجع ثم [مراقبة المحتوى الخاص في Yammer](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content).</span><span class="sxs-lookup"><span data-stu-id="4bca6-116">For more info, see then [Monitor private content in Yammer](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content).</span></span>  

<span data-ttu-id="4bca6-117">**Yammer على مستوى الشبكة الضيوف والملفات في SharePoint عبر الإنترنت**</span><span class="sxs-lookup"><span data-stu-id="4bca6-117">**Yammer network-level guests and files in SharePoint Online**</span></span>  

<span data-ttu-id="4bca6-118">لا يستخدم [الضيوف على مستوى الشبكة في Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) Azure AD B2B وهم داخليون لخدمة Yammer، بحيث لا يمكنهم الوصول إلى ملفات Yammer المخزنة في SharePoint.</span><span class="sxs-lookup"><span data-stu-id="4bca6-118">[Network-level guests in Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) do not use Azure AD B2B and are internal to the Yammer service, so they can't access Yammer files stored in SharePoint.</span></span> <span data-ttu-id="4bca6-119">إنشاء مستخدم AAD B2B خارجي الذين يمكنهم الوصول إلى مكتبات المستندات في SharePoint عبر الإنترنت باستخدام تلك الهوية.</span><span class="sxs-lookup"><span data-stu-id="4bca6-119">Create an external AAD B2B user who can access document libraries in SharePoint Online by using that identity.</span></span> <span data-ttu-id="4bca6-120">للحصول على معلومات حول دعم ضيف Azure A2B في Yammer، راجع [دعم الضيف بين الشركات (B2B) في Yammer Preview - شروط العملاء والأسئلة الشائعة](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer).</span><span class="sxs-lookup"><span data-stu-id="4bca6-120">For information about future Azure AD B2B guest support in Yammer, see [Business-to-business (B2B) Guest support in Yammer Preview - Customer Terms and FAQ](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer).</span></span>