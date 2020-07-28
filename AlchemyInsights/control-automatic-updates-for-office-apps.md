---
title: التحكم في التحديثات التلقائية لتطبيقات Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1743"
- "9000140"
ms.openlocfilehash: 5c56c3adcc9a06db43d4df6f367657cb8ff0c8c8
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 07/28/2020
ms.locfileid: "45438692"
---
# <a name="control-automatic-updates-for-office-apps"></a><span data-ttu-id="7c634-102">التحكم في التحديثات التلقائية لتطبيقات Office</span><span class="sxs-lookup"><span data-stu-id="7c634-102">Control automatic updates for Office Apps</span></span>

<span data-ttu-id="7c634-103">يتم بشكل افتراضي تنزيل تحديثات تطبيقات Office تلقائياً وتطبيقها في الخلفية دون أي تدخل من المستخدم.</span><span class="sxs-lookup"><span data-stu-id="7c634-103">By default, updates for Office Apps are downloaded automatically and applied in the background without any user intervention.</span></span> <span data-ttu-id="7c634-104">ومع ذلك، يمكن للمسؤولين التحكم في كيفية تطبيق التحديثات باستخدام إعدادات Office Update.</span><span class="sxs-lookup"><span data-stu-id="7c634-104">However, administrators can control how updates are applied by using Office Update settings.</span></span> <span data-ttu-id="7c634-105">تسمح إعدادات التحديث للمسؤولين بتمكين التحديثات التلقائية أو تعطيلها، وإظهار الزر **Update Now** في Office أو إخفائه، وتعيين المواعيد النهائية للتحديث، وغير ذلك الكثير.</span><span class="sxs-lookup"><span data-stu-id="7c634-105">Update settings allow administrators to enable or disable automatic updates, show or hide the **Update Now** button in Office, set update deadlines, and more.</span></span> <span data-ttu-id="7c634-106">للحصول على معلومات مفصلة، انظر:</span><span class="sxs-lookup"><span data-stu-id="7c634-106">For detailed information, see:</span></span>

- [<span data-ttu-id="7c634-107">تكوين إعدادات التحديث لـ Office</span><span class="sxs-lookup"><span data-stu-id="7c634-107">Configure update settings for Office</span></span>](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus)  
- [<span data-ttu-id="7c634-108">لم يتم تمكين التحديث التلقائي لـ Office</span><span class="sxs-lookup"><span data-stu-id="7c634-108">Automatic updating for Office is not enabled</span></span>](https://support.microsoft.com/help/2753538/automatic-updating-for-office-2013-and-office-2016-click-to-run-is-not)  
- [<span data-ttu-id="7c634-109">تحديد كيفية تحديث Office بعد تثبيته</span><span class="sxs-lookup"><span data-stu-id="7c634-109">Define how Office is updated after it's installed</span></span>](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element)

<span data-ttu-id="7c634-110">لمراجعة إعدادات التحديثات الموجودة المطبقة على جهاز عميل، اتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="7c634-110">To review the existing updates settings applied to a client machine, follow these steps:</span></span>

1. <span data-ttu-id="7c634-111">فتح محرر التسجيل بواسطة الانتقال إلى **بدء**  >  **تشغيل**  >  **regedit**.</span><span class="sxs-lookup"><span data-stu-id="7c634-111">Open the Registry Editor by going to **Start** > **Run** > **regedit**.</span></span>
2. <span data-ttu-id="7c634-112">التبديل إلى الموقع التالي ومراجعة إعدادات Office Update:</span><span class="sxs-lookup"><span data-stu-id="7c634-112">Switch to the following location and review the Office Update settings:</span></span>  
    <span data-ttu-id="7c634-113">(أ)</span><span class="sxs-lookup"><span data-stu-id="7c634-113">a.</span></span> <span data-ttu-id="7c634-114">HKEY_LOCAL_MACHINE\SOFTWARE\\مايكروسوفت\Office</span><span class="sxs-lookup"><span data-stu-id="7c634-114">HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Office</span></span>\  
    <span data-ttu-id="7c634-115">ب.</span><span class="sxs-lookup"><span data-stu-id="7c634-115">b.</span></span> <span data-ttu-id="7c634-116">انقر فوق التشغيل\تكوين</span><span class="sxs-lookup"><span data-stu-id="7c634-116">ClickToRun\Configuration</span></span>

<span data-ttu-id="7c634-117">**ملاحظة**  إذا تم تعيين مفتاح OfficeMgmtCOM، قد ترى رسالة "يتم إدارة التحديثات من قبل مسؤول النظام الخاص بك" في تحديثات Office **Office**  >  **حساب**  >  **Office**.</span><span class="sxs-lookup"><span data-stu-id="7c634-117">**Note**  If the OfficeMgmtCOM key is set, you might see the "Updates are managed by your system administrator" message in **Office** > **Account** > **Office Updates**.</span></span> <span data-ttu-id="7c634-118">لمزيد من المعلومات، راجع [إدارة التحديثات إلى تطبيقات Microsoft 365 مع إدارة تكوين نقطة النهاية ل Microsoft](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).</span><span class="sxs-lookup"><span data-stu-id="7c634-118">For more info, see [Manage updates to Microsoft 365 Apps with Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).</span></span>  