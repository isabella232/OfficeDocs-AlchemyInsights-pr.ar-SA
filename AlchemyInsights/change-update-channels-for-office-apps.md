---
title: تغيير قنوات التحديث لتطبيقات Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1740"
- "9000140"
ms.openlocfilehash: 4939682a6ca95c4f5475ee6aedea48c9ce83df7f
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 07/28/2020
ms.locfileid: "45438700"
---
# <a name="change-update-channels-for-office-apps"></a><span data-ttu-id="1d01d-102">تغيير قنوات التحديث لتطبيقات Office</span><span class="sxs-lookup"><span data-stu-id="1d01d-102">Change update channels for Office apps</span></span>

<span data-ttu-id="1d01d-103">بالنسبة إلى عمليات تثبيت Office الجديدة، استخدم إعدادات تنزيل برامج Office لتحديد قناة التحديث المطلوبة، ثم قم بتثبيت (أو إعادة تثبيت) تطبيقات Office.</span><span class="sxs-lookup"><span data-stu-id="1d01d-103">For new Office installations, use Office Software Download Settings to select the desired update channel, and then install (or re-install) Office apps.</span></span> <span data-ttu-id="1d01d-104">لمزيد من المعلومات، راجع [إدارة إعدادات تنزيل البرامج في Office 365](https://docs.microsoft.com/deployoffice/manage-software-download-settings-office-365).</span><span class="sxs-lookup"><span data-stu-id="1d01d-104">For more info, see [Manage software download settings in Office 365](https://docs.microsoft.com/deployoffice/manage-software-download-settings-office-365).</span></span> 

<span data-ttu-id="1d01d-105">**ملاحظة** يتم تطبيق قناة التحديث المحددة باستخدام إعدادات تحميل برامج Office على كافة المستخدمين الذين يقومون بإجراء عمليات تثبيت جديدة باستخدام المدخل O365.</span><span class="sxs-lookup"><span data-stu-id="1d01d-105">**Note** The update channel selected using the Office Software Download Settings applies to all users performing new installations using the O365 portal.</span></span> <span data-ttu-id="1d01d-106">لمزيد من المعلومات، راجع [تنزيل وتثبيت أو إعادة تثبيت Microsoft 365 أو Office 2019 على كمبيوتر شخصي أو Mac](https://support.microsoft.com/office/download-and-install-or-reinstall-microsoft-365-or-office-2019-on-a-pc-or-mac-4414eaaf-0478-48be-9c42-23adc4716658).</span><span class="sxs-lookup"><span data-stu-id="1d01d-106">For more info, see [Download and install or reinstall Microsoft 365 or Office 2019 on a PC or Mac](https://support.microsoft.com/office/download-and-install-or-reinstall-microsoft-365-or-office-2019-on-a-pc-or-mac-4414eaaf-0478-48be-9c42-23adc4716658).</span></span>   

<span data-ttu-id="1d01d-107">لتثبيتات Office الموجودة، استخدم أداة نشر Office (ODT) للتبديل إلى قناة تحديث مختلفة:</span><span class="sxs-lookup"><span data-stu-id="1d01d-107">For existing Office installations, use the Office Deployment Tool (ODT) to switch to a different update channel:</span></span>  

1. <span data-ttu-id="1d01d-108">قم بتنزيل أحدث إصدار من أداة نشر Office (setup.exe) من [مركز تحميل Microsoft](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="1d01d-108">Download the latest version of the Office Deployment Tool (setup.exe) from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
2. <span data-ttu-id="1d01d-109">حدد اسم القناة التي تريد التبديل إليها.</span><span class="sxs-lookup"><span data-stu-id="1d01d-109">Identify the name of the channel that you want to switch to.</span></span> <span data-ttu-id="1d01d-110">لمزيد من المعلومات، راجع [خيارات التكوين لأداة نشر Office](https://docs.microsoft.com/DeployOffice/configuration-options-for-the-office-2016-deployment-tool#channel-attribute-part-of-add-element).</span><span class="sxs-lookup"><span data-stu-id="1d01d-110">For more info, see [Configuration options for the Office Deployment Tool](https://docs.microsoft.com/DeployOffice/configuration-options-for-the-office-2016-deployment-tool#channel-attribute-part-of-add-element).</span></span>
3. <span data-ttu-id="1d01d-111">إنشاء ملف XML تكوين تحديد اسم القناة المناسبة، على سبيل المثال، update.xml.</span><span class="sxs-lookup"><span data-stu-id="1d01d-111">Create a configuration XML file specifying the appropriate channel name, for example, update.xml.</span></span>  
    <span data-ttu-id="1d01d-112">(أ)</span><span class="sxs-lookup"><span data-stu-id="1d01d-112">a.</span></span> <Configuration>  
    <span data-ttu-id="1d01d-113">ب.</span><span class="sxs-lookup"><span data-stu-id="1d01d-113">b.</span></span> <span data-ttu-id="1d01d-114"><قناة التحديثات **="شهريا"** /></span><span class="sxs-lookup"><span data-stu-id="1d01d-114"><Updates **Channel="Monthly"** /></span></span>  
    <span data-ttu-id="1d01d-115">ج.</span><span class="sxs-lookup"><span data-stu-id="1d01d-115">c.</span></span> </Configuration>
4. <span data-ttu-id="1d01d-116">من موجه أوامر مرتفعة، قم بالتبديل إلى موقع المجلد حيث يوجد setup.exe ثم قم بتشغيل الأمر التالي:</span><span class="sxs-lookup"><span data-stu-id="1d01d-116">From an elevated command prompt, switch to the folder location where setup.exe resides and run the following command:</span></span>  
    <span data-ttu-id="1d01d-117">(أ)</span><span class="sxs-lookup"><span data-stu-id="1d01d-117">a.</span></span> <span data-ttu-id="1d01d-118">setup.exe /تكوين update.xml</span><span class="sxs-lookup"><span data-stu-id="1d01d-118">setup.exe /configure update.xml</span></span>
5. <span data-ttu-id="1d01d-119">بدء تشغيل تطبيق Office (مثل Excel)، ثم حدد **حساب ملف**  >  **Account**.</span><span class="sxs-lookup"><span data-stu-id="1d01d-119">Start an Office application (such as Excel), and then select **File** > **Account**.</span></span> <span data-ttu-id="1d01d-120">في المقطع معلومات المنتج، حدد **تحديث خيارات التحديث**  >  **الآن**.</span><span class="sxs-lookup"><span data-stu-id="1d01d-120">In the Product Information section, select **Update Options** > **Update Now**.</span></span>

<span data-ttu-id="1d01d-121">لمزيد من المعلومات، راجع [كيفية تبديل قنوات التحديث لتطبيقات Office الحالية](https://support.microsoft.com/help/3185078/how-to-switch-from-semi-annual-channel-to-monthly-channel).</span><span class="sxs-lookup"><span data-stu-id="1d01d-121">For more information, see [How to switch update channels for existing Office Apps](https://support.microsoft.com/help/3185078/how-to-switch-from-semi-annual-channel-to-monthly-channel).</span></span> 

<span data-ttu-id="1d01d-122">للتبديل قنوات التحديث لمجموعة محددة من المستخدمين أو باستخدام إدارة التكوين (SCCM) ، تكوين إعداد قناة التحديث باستخدام كائن نهج المجموعة.</span><span class="sxs-lookup"><span data-stu-id="1d01d-122">For switching update channels for a selected group of users or by using Configuration Manager (SCCM), configure the Update Channel setting using GPO.</span></span> <span data-ttu-id="1d01d-123">لمزيد من المعلومات، راجع [نظرة عامة على قنوات التحديث لتطبيقات Microsoft 365](https://docs.microsoft.com/deployoffice/overview-update-channels#group-policy).</span><span class="sxs-lookup"><span data-stu-id="1d01d-123">For more info, see [Overview of update channels for Microsoft 365 Apps](https://docs.microsoft.com/deployoffice/overview-update-channels#group-policy).</span></span> <span data-ttu-id="1d01d-124">للحصول على تفاصيل، راجع [كيفية إدارة قنوات Office 365 ProPlus لمحترفي تكنولوجيا المعلومات](https://techcommunity.microsoft.com/t5/office-365-blog/how-to-manage-office-365-proplus-channels-for-it-pros/ba-p/795813) وإدارة [التحديثات إلى تطبيقات Microsoft 365 مع Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-microsoft-365-apps-updates-configuration-manager).</span><span class="sxs-lookup"><span data-stu-id="1d01d-124">For details, see [How to manage Office 365 ProPlus Channels for IT Pros](https://techcommunity.microsoft.com/t5/office-365-blog/how-to-manage-office-365-proplus-channels-for-it-pros/ba-p/795813) and [Manage updates to Microsoft 365 Apps with Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-microsoft-365-apps-updates-configuration-manager).</span></span>