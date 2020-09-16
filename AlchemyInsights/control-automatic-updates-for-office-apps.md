---
title: التحكم في التحديثات التلقائية لتطبيقات Office
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
- "1743"
- "9000140"
ms.openlocfilehash: ab3d6e60bc1b67220adbdf7ba61599a6b7aa663a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47747763"
---
# <a name="control-automatic-updates-for-office-apps"></a><span data-ttu-id="b0c98-102">التحكم في التحديثات التلقائية لتطبيقات Office</span><span class="sxs-lookup"><span data-stu-id="b0c98-102">Control automatic updates for Office Apps</span></span>

<span data-ttu-id="b0c98-103">بشكل افتراضي ، يتم تنزيل التحديثات الخاصة بتطبيقات Office تلقائيا وتطبيقها في الخلفية بدون تدخل اي مستخدم.</span><span class="sxs-lookup"><span data-stu-id="b0c98-103">By default, updates for Office Apps are downloaded automatically and applied in the background without any user intervention.</span></span> <span data-ttu-id="b0c98-104">ومع ذلك ، يمكن للمسؤولين التحكم في كيفيه تطبيق التحديثات باستخدام إعدادات Office Update.</span><span class="sxs-lookup"><span data-stu-id="b0c98-104">However, administrators can control how updates are applied by using Office Update settings.</span></span> <span data-ttu-id="b0c98-105">تسمح إعدادات التحديث للمسؤولين بتمكين التحديثات التلقائية أو تعطيلها ، أو إظهار الزر **التحديث الآن** أو إخفاؤه في Office ، وتعيين المواعيد النهائية للتحديث ، والمزيد.</span><span class="sxs-lookup"><span data-stu-id="b0c98-105">Update settings allow administrators to enable or disable automatic updates, show or hide the **Update Now** button in Office, set update deadlines, and more.</span></span> <span data-ttu-id="b0c98-106">للحصول علي معلومات مفصله ، راجع:</span><span class="sxs-lookup"><span data-stu-id="b0c98-106">For detailed information, see:</span></span>

- [<span data-ttu-id="b0c98-107">تكوين إعدادات التحديث ل Office</span><span class="sxs-lookup"><span data-stu-id="b0c98-107">Configure update settings for Office</span></span>](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus)  
- [<span data-ttu-id="b0c98-108">لم يتم تمكين التحديث التلقائي ل Office</span><span class="sxs-lookup"><span data-stu-id="b0c98-108">Automatic updating for Office is not enabled</span></span>](https://support.microsoft.com/help/2753538/automatic-updating-for-office-2013-and-office-2016-click-to-run-is-not)  
- [<span data-ttu-id="b0c98-109">تعريف كيفيه تحديث Office بعد تثبيته</span><span class="sxs-lookup"><span data-stu-id="b0c98-109">Define how Office is updated after it's installed</span></span>](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element)

<span data-ttu-id="b0c98-110">لمراجعه إعدادات التحديثات الموجودة المطبقة علي جهاز عميل ، اتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="b0c98-110">To review the existing updates settings applied to a client machine, follow these steps:</span></span>

1. <span data-ttu-id="b0c98-111">افتح محرر السجل بالانتقال إلى **بدء**  >  **تشغيل**  >  **regedit**.</span><span class="sxs-lookup"><span data-stu-id="b0c98-111">Open the Registry Editor by going to **Start** > **Run** > **regedit**.</span></span>
2. <span data-ttu-id="b0c98-112">انتقل إلى الموقع التالي وراجع إعدادات تحديث Office:</span><span class="sxs-lookup"><span data-stu-id="b0c98-112">Switch to the following location and review the Office Update settings:</span></span>  
    <span data-ttu-id="b0c98-113">علي.</span><span class="sxs-lookup"><span data-stu-id="b0c98-113">a.</span></span> <span data-ttu-id="b0c98-114">HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft\Office</span><span class="sxs-lookup"><span data-stu-id="b0c98-114">HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Office</span></span>\  
    <span data-ttu-id="b0c98-115">ب.</span><span class="sxs-lookup"><span data-stu-id="b0c98-115">b.</span></span> <span data-ttu-id="b0c98-116">clicktorun\configuration</span><span class="sxs-lookup"><span data-stu-id="b0c98-116">ClickToRun\Configuration</span></span>

<span data-ttu-id="b0c98-117">**ملاحظه**  إذا تم تعيين المفتاح أوفيسيمجمتكوم ، فقد تري الرسالة "تمت أداره التحديثات بواسطة مسؤول **Office**النظام" في  >  **Account**  >  **تحديثات office**لحساب office.</span><span class="sxs-lookup"><span data-stu-id="b0c98-117">**Note**  If the OfficeMgmtCOM key is set, you might see the "Updates are managed by your system administrator" message in **Office** > **Account** > **Office Updates**.</span></span> <span data-ttu-id="b0c98-118">لمزيد من المعلومات ، راجع [أداره التحديثات لتطبيقات microsoft 365 باستخدام أداره تكوين نقاط النهاية من microsoft](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).</span><span class="sxs-lookup"><span data-stu-id="b0c98-118">For more info, see [Manage updates to Microsoft 365 Apps with Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).</span></span>  