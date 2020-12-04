---
title: كيفيه أضافه مفوض أو ازالته في Outlook for Windows
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800004"
- "7334"
ms.openlocfilehash: fcbd6082c104f0e1bca022a23cbbeb6e3363a6c5
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573272"
---
# <a name="how-to-add-or-remove-a-delegate-in-outlook-for-windows"></a><span data-ttu-id="3197e-102">كيفيه أضافه مفوض أو ازالته في Outlook for Windows</span><span class="sxs-lookup"><span data-stu-id="3197e-102">How to add or remove a Delegate in Outlook for Windows</span></span>

<span data-ttu-id="3197e-103">لأضافه مفوض في Outlook for Windows:</span><span class="sxs-lookup"><span data-stu-id="3197e-103">To add a Delegate in Outlook for Windows:</span></span> 

1. <span data-ttu-id="3197e-104">انقر فوق علامة التبويب **ملف** متبوعا **بإعدادات الحساب**، ثم اختر **تفويض الوصول**.</span><span class="sxs-lookup"><span data-stu-id="3197e-104">Click on the **File** tab followed by **Account Settings**, and then choose **Delegate Access**.</span></span>
2. <span data-ttu-id="3197e-105">انقر فوق **أضافه**.</span><span class="sxs-lookup"><span data-stu-id="3197e-105">Click on **Add**.</span></span> <span data-ttu-id="3197e-106">إذا لم يظهر **الاضافه** ، فقد لا يوجد اتصال نشط بين Outlook و Exchange.</span><span class="sxs-lookup"><span data-stu-id="3197e-106">If **Add** doesn’t appear, an active connection might not exist between Outlook and Exchange.</span></span> <span data-ttu-id="3197e-107">يعرض شريط معلومات Outlook حاله الاتصال.</span><span class="sxs-lookup"><span data-stu-id="3197e-107">The Outlook status bar displays the connection status.</span></span>
3. <span data-ttu-id="3197e-108">اكتب اسم الشخص الذي تريد تعيينه كمفوض أو ابحث واختر الاسم في قائمه نتائج البحث.</span><span class="sxs-lookup"><span data-stu-id="3197e-108">Type the name of the person you want to designate as your delegate, or search and choose the name in the search results list.</span></span>

    > [!NOTE]
    > <span data-ttu-id="3197e-109">يجب ان يكون المفوض شخصا في قائمه العناوين العمومية في Exchange الخاصة بمؤسسك (GAL).</span><span class="sxs-lookup"><span data-stu-id="3197e-109">The delegate must be a person in your organization's Exchange Global Address List (GAL).</span></span>
4. <span data-ttu-id="3197e-110">انقر فوق **أضافه** متبوعه **بموافق**.</span><span class="sxs-lookup"><span data-stu-id="3197e-110">Click on **Add** followed by **OK**.</span></span>
5. <span data-ttu-id="3197e-111">في مربع الحوار **أذونات المفوضين** ، اقبل إعدادات الأذونات الافتراضية أو حدد مستويات الوصول المخصصة لمجلدات Exchange.</span><span class="sxs-lookup"><span data-stu-id="3197e-111">In the **Delegate Permissions** dialog box, accept the default permission settings or select custom access levels for Exchange folders.</span></span>

    - <span data-ttu-id="3197e-112">إذا كان المفوض يحتاج إلى الاذن للعمل فقط مع طلبات الاجتماعات والاستجابات ، فان إعدادات الأذونات الافتراضية مثل **المفوض الذي يتلقى نسخا من الرسائل المرتبطة بالاجتماعات التي يتم إرسالها آليي** كافيه.</span><span class="sxs-lookup"><span data-stu-id="3197e-112">If a delegate needs permission to work only with meeting requests and responses, the default permission settings such as **Delegate receives copies of meeting-related messages sent to me** are sufficient.</span></span> <span data-ttu-id="3197e-113">يمكنك ترك اعداد أذونات **علبه الوارد** في " **بلا**".</span><span class="sxs-lookup"><span data-stu-id="3197e-113">You can leave the **Inbox** permission setting at **None**.</span></span> <span data-ttu-id="3197e-114">ستنتقل طلبات الاجتماع والاستجابات مباشره إلى علبه الوارد الخاصة بالمفوض.</span><span class="sxs-lookup"><span data-stu-id="3197e-114">Meeting requests and responses will go directly to the delegate's inbox.</span></span>

    > [!NOTE]
    > <span data-ttu-id="3197e-115">بشكل افتراضي ، يتم منح المفوض الاذن " **المحرر" (يمكنه قراءه العناصر وإنشاءها وتعديلها)** في مجلد **التقويم** .</span><span class="sxs-lookup"><span data-stu-id="3197e-115">By default, the delegate is granted **Editor (can read, create, and modify items)** permission to your **Calendar** folder.</span></span> <span data-ttu-id="3197e-116">عندما يستجيب المفوض إلى اجتماع بالنيابة عنك ، تتم اضافته تلقائيا إلى مجلد **التقويم** .</span><span class="sxs-lookup"><span data-stu-id="3197e-116">When the delegate responds to a meeting on your behalf, it is automatically added to your **Calendar** folder.</span></span>

5. <span data-ttu-id="3197e-117">لإرسال رسالة لاعلام المفوض بالأذونات التي تم تغييرها ، حدد خانه الاختيار **إرسال رسالة إلى المفوض الذي يلخص هذه الأذونات تلقائيا** .</span><span class="sxs-lookup"><span data-stu-id="3197e-117">To send a message to notify the delegate of the changed permissions, select the **Automatically send a message to delegate summarizing these permissions** check box.</span></span>
6. <span data-ttu-id="3197e-118">إذا أردت ، حدد خانه الاختيار **يمكن للمفوض عرض العناصر الخاصة بي** .</span><span class="sxs-lookup"><span data-stu-id="3197e-118">If you want, select the **Delegate can see my private items** check box.</span></span>

    > [!IMPORTANT]
    > <span data-ttu-id="3197e-119">يؤثر هذا الاعداد علي كل مجلدات Exchange.</span><span class="sxs-lookup"><span data-stu-id="3197e-119">This setting affects all Exchange folders.</span></span> <span data-ttu-id="3197e-120">يتضمن ذلك كافة البريد وجات الاتصال والتقويم والمهام والملاحظات ومجلدات اليومية.</span><span class="sxs-lookup"><span data-stu-id="3197e-120">This includes all Mail, Contacts, Calendar, Tasks, Notes, and Journal folders.</span></span> <span data-ttu-id="3197e-121">لا توجد طريقه لمنح حق الوصول إلى العناصر الخاصة في المجلدات المحددة فقط.</span><span class="sxs-lookup"><span data-stu-id="3197e-121">There is no way to grant access to private items in only specified folders.</span></span>

7. <span data-ttu-id="3197e-122">اختر **موافق**.</span><span class="sxs-lookup"><span data-stu-id="3197e-122">Choose **OK**.</span></span>

    > [!NOTE]
    >
    > - <span data-ttu-id="3197e-123">تتضمن الرسائل المرسلة بالأذونات إرسال بالنيابة عن كلا المفوضين وأسماءك إلى جانب **من**.</span><span class="sxs-lookup"><span data-stu-id="3197e-123">Messages sent with Send on Behalf permissions include both the delegate's and your names next to **From**.</span></span> <span data-ttu-id="3197e-124">عند إرسال رسالة باستخدام الأذونات "إرسال باسم" ، يظهر اسمك فقط.</span><span class="sxs-lookup"><span data-stu-id="3197e-124">When a message is sent with Send As permissions, only your name appears.</span></span>
    > - <span data-ttu-id="3197e-125">بمجرد أضافه شخص كمفوض ، يمكنه أضافه علبه بريد Exchange إلى ملف تعريف Outlook الخاص به.</span><span class="sxs-lookup"><span data-stu-id="3197e-125">Once you add someone as a delegate, they can add your Exchange mailbox to their Outlook profile.</span></span> <span data-ttu-id="3197e-126">للحصول علي الإرشادات ، راجع [أداره البريد وعناصر التقويم الخاصة بشخص آخر](https://support.microsoft.com/office/manage-another-person-s-mail-and-calendar-items-afb79d6b-2967-43b9-a944-a6b953190af5).</span><span class="sxs-lookup"><span data-stu-id="3197e-126">For instructions, see [Manage another person's mail and calendar items](https://support.microsoft.com/office/manage-another-person-s-mail-and-calendar-items-afb79d6b-2967-43b9-a944-a6b953190af5).</span></span>

<span data-ttu-id="3197e-127">لأزاله مفوض في Outlook for Windows:</span><span class="sxs-lookup"><span data-stu-id="3197e-127">To remove a Delegate in Outlook for Windows:</span></span>

1. <span data-ttu-id="3197e-128">انقر فوق علامة التبويب **ملف** .</span><span class="sxs-lookup"><span data-stu-id="3197e-128">Click on the **File** tab.</span></span>
2. <span data-ttu-id="3197e-129">انقر فوق **إعدادات الحسابات** متبوعه **بحق الوصول للمفوض**.</span><span class="sxs-lookup"><span data-stu-id="3197e-129">Click on **Account Settings** followed by **Delegate Access**.</span></span>
3. <span data-ttu-id="3197e-130">اختر اسم المفوض الذي تريد تغيير الأذونات الخاصة به ، ثم انقر فوق عند **الازاله** متبوعا **بموافق**.</span><span class="sxs-lookup"><span data-stu-id="3197e-130">Choose the name of the delegate for whom you want to change permissions, and then click on **Remove** followed by **OK**.</span></span>
