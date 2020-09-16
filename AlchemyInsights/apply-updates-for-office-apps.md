---
title: تطبيق التحديثات لتطبيقات Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1747"
- "9000140"
ms.openlocfilehash: 8306d1acafe48f8779a8c02db8e3fe2f5d5f0e95
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47716736"
---
# <a name="apply-updates-for-office-apps"></a><span data-ttu-id="34066-102">تطبيق التحديثات لتطبيقات Office</span><span class="sxs-lookup"><span data-stu-id="34066-102">Apply updates for Office apps</span></span>

<span data-ttu-id="34066-103">بشكل افتراضي ، تكون تحديثات تطبيقات Office مجانية ، ويتم تنزيلها تلقائيا ، وتطبيقها في الخلفية بدون تدخل اي مستخدم.</span><span class="sxs-lookup"><span data-stu-id="34066-103">By default, updates for Office Apps are free, downloaded automatically, and applied in the background without any user intervention.</span></span> <span data-ttu-id="34066-104">لتشغيل التحديثات يدويا إذا كنت تعمل علي مشاكل اثناء تطبيق التحديثات ، فراجع [تثبيت تحديثات Office](https://support.office.com/article/install-office-updates-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="34066-104">To run updates manually if you are running into issues applying updates, see [Install Office updates](https://support.office.com/article/install-office-updates-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span> <span data-ttu-id="34066-105">لمزيد من المعلومات ، راجع [استكشاف أخطاء تثبيت Office وإصلاحها](https://support.microsoft.com/office/troubleshoot-installing-office-35ff2def-e0b2-4dac-9784-4cf212c1f6c2?ui=en-us&rs=en-us&ad=us#O365Plans=signinorgid).</span><span class="sxs-lookup"><span data-stu-id="34066-105">For more information, see [Troubleshoot installing Office](https://support.microsoft.com/office/troubleshoot-installing-office-35ff2def-e0b2-4dac-9784-4cf212c1f6c2?ui=en-us&rs=en-us&ad=us#O365Plans=signinorgid).</span></span>

<span data-ttu-id="34066-106">لأداره تحديثات Office للمستخدمين ، ضع في اعتبارك الخيارات التالية:</span><span class="sxs-lookup"><span data-stu-id="34066-106">To manage Office updates for your users, consider these options:</span></span>

- <span data-ttu-id="34066-107">اختر قناه تحديث Office المناسبة لمؤسسك استنادا إلى التكرار المطلوب من التحديثات.</span><span class="sxs-lookup"><span data-stu-id="34066-107">Choose the right Office Update Channel for your organization based on the desired frequency of updates.</span></span> <span data-ttu-id="34066-108">لمعرفه كيفيه اجراء ذلك ، راجع [نظره عامه حول تحديث القناات لتطبيقات Microsoft 365](https://docs.microsoft.com/deployoffice/overview-of-update-channels-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="34066-108">To learn how, see [Overview of update channels for Microsoft 365 Apps](https://docs.microsoft.com/deployoffice/overview-of-update-channels-for-office-365-proplus).</span></span>

- <span data-ttu-id="34066-109">حدد ما إذا كنت تريد تطبيق التحديثات تلقائيا من الإنترنت أو من مشاركه محليه.</span><span class="sxs-lookup"><span data-stu-id="34066-109">Decide whether to apply updates automatically from the internet or from an on-premises share.</span></span> <span data-ttu-id="34066-110">لمعرفه كيفيه [أداره التحديثات لتطبيقات Microsoft 365](https://docs.microsoft.com/deployoffice/choose-how-to-manage-updates-to-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="34066-110">To learn how, see [Choose how to manage updates to Microsoft 365 Apps](https://docs.microsoft.com/deployoffice/choose-how-to-manage-updates-to-office-365-proplus).</span></span>

- <span data-ttu-id="34066-111">مراجعه إعدادات تحديث Office للتحكم في كيفيه تطبيق التحديثات علي أجهزه المستخدم النهائية:</span><span class="sxs-lookup"><span data-stu-id="34066-111">Review Office Update Settings to control how updates are applied to end user machines:</span></span>

    - <span data-ttu-id="34066-112">قم [بتكوين إعدادات التحديث لتطبيقات Microsoft 365](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="34066-112">[Configure update settings for Microsoft 365 Apps](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus).</span></span>
    - <span data-ttu-id="34066-113">[تعرف كيفيه تحديث Office بعد تثبيته](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element).</span><span class="sxs-lookup"><span data-stu-id="34066-113">[Define how Office is updated after it's installed](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element).</span></span>

<span data-ttu-id="34066-114">عند نشر تطبيقات Office لعده مستخدمين ، استخدم أداه تخصيص Office لإنشاء ملفات التكوين للنشر ، وتكوين تحديثات Office باستخدام أداه نشر Office.</span><span class="sxs-lookup"><span data-stu-id="34066-114">When deploying Office apps to multiple users, use the Office Customization tool to build configuration files for deployment, and configure Office updates by using the Office Deployment tool.</span></span> <span data-ttu-id="34066-115">للحصول علي مزيد من المعلومات ، راجع [نظره عامه حول أداه تخصيص office](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run) [وأداه نشر office](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="34066-115">For more info, see [Overview of the Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run) and the [Office Deployment tool](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>

- <span data-ttu-id="34066-116">للحصول علي مثال حول كيفيه اعداد مجموعات المستخدمين لنشر تحديثات Office ، راجع [نشر تطبيقات Microsoft 365 من مصدر محلي](https://docs.microsoft.com/deployoffice/deploy-office-365-proplus-from-a-local-source).</span><span class="sxs-lookup"><span data-stu-id="34066-116">For an example of how to setup user groups to deploy Office updates, see [Deploy Microsoft 365 Apps from a local source](https://docs.microsoft.com/deployoffice/deploy-office-365-proplus-from-a-local-source).</span></span>
-   <span data-ttu-id="34066-117">يمكنك استخدام اعداد فورسيبشوتدوون في حاله عدم تطبيق تحديثات Office علي بعض المستخدمين نظرا لفتح تطبيقات Office.</span><span class="sxs-lookup"><span data-stu-id="34066-117">Consider using the ForceAppShutdown setting in case Office updates are not getting applied to a few users because of open Office apps.</span></span> <span data-ttu-id="34066-118">للحصول علي مزيد من المعلومات ، راجع [الخاصية فورسيبشوتدوون (جزء من عنصر الخاصية)](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#forceappshutdown-property-part-of-property-element).</span><span class="sxs-lookup"><span data-stu-id="34066-118">For more info, see the [FORCEAPPSHUTDOWN property (part of Property element)](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#forceappshutdown-property-part-of-property-element).</span></span> 

<span data-ttu-id="34066-119">**راجع أيضا**</span><span class="sxs-lookup"><span data-stu-id="34066-119">**See also**</span></span>

<span data-ttu-id="34066-120">[نظره عامه حول عمليه التحديث لتطبيقات Microsoft 365](https://docs.microsoft.com/deployoffice/overview-of-the-update-process-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="34066-120">[Overview of the update process for Microsoft 365 Apps](https://docs.microsoft.com/deployoffice/overview-of-the-update-process-for-office-365-proplus).</span></span>  
<span data-ttu-id="34066-121">[إصدار معلومات حول التحديثات لتطبيقات Microsoft 365](https://docs.microsoft.com/officeupdates/release-notes-office365-proplus).</span><span class="sxs-lookup"><span data-stu-id="34066-121">[Release information for updates to Microsoft 365 Apps](https://docs.microsoft.com/officeupdates/release-notes-office365-proplus).</span></span>  
<span data-ttu-id="34066-122">[أداره التحديثات لتطبيقات microsoft 365 باستخدام أداره تكوين نقاط النهاية من microsoft](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager).</span><span class="sxs-lookup"><span data-stu-id="34066-122">[Manage updates to Microsoft 365 Apps with Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager).</span></span>  
