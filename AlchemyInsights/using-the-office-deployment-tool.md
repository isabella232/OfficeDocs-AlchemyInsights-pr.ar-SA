---
title: استخدام أداه النشر من Office
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: f3a5dbfc6b64ccd4f0b19a5f86236336e78838d4
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 11/17/2020
ms.locfileid: "49085819"
---
# <a name="using-the-office-deployment-tool-odt"></a><span data-ttu-id="c92e4-102">استخدام أداه النشر من Office (ODT)</span><span class="sxs-lookup"><span data-stu-id="c92e4-102">Using the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="c92e4-103">يمكنك استخدام أداه النشر من office (ODT) لنشر إصدارات Office 365 من Office.</span><span class="sxs-lookup"><span data-stu-id="c92e4-103">You use the Office Deployment Tool (ODT) to deploy Office 365 versions of Office.</span></span> <span data-ttu-id="c92e4-104">يتم تشغيل أداه نشر Office (setupodt.exe) من سطر الأوامر وتستخدم ملف XML تكوين لتحديد الإعدادات التي يجب تطبيقها عند نشر Office.</span><span class="sxs-lookup"><span data-stu-id="c92e4-104">The Office Deployment Tool (setupodt.exe) is run from the command line and uses a configuration XML file to determine what settings to apply when deploying Office.</span></span>
  
1. <span data-ttu-id="c92e4-105">قم بتنزيل أحدث إصدار من أداه نشر Office من [مركز التنزيل ل Microsoft](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="c92e4-105">Download the latest version of the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>

2. <span data-ttu-id="c92e4-106">استخدم [أداه تخصيص Office (OCT)](https://config.office.com) لتحديد تفضيلات النشر وإنشاء ملف XML للتكوين.</span><span class="sxs-lookup"><span data-stu-id="c92e4-106">Use the [Office Customization Tool (OCT)](https://config.office.com) to select your deployment preferences and create the configuration XML file.</span></span> <span data-ttu-id="c92e4-107">تصدير ملف التكوين ووضعه محليا علي المجلد نفسه الذي يتواجد فيه الsetupodt.exe.</span><span class="sxs-lookup"><span data-stu-id="c92e4-107">Export the configuration file and place it locally on the same folder where the setupodt.exe resides.</span></span>

    <span data-ttu-id="c92e4-108">**ملاحظه:** تحدث مشاكل تثبيت Office بشكل عام بسبب ملفات تكوين غير صحيحه أو مالفورماتيد.</span><span class="sxs-lookup"><span data-stu-id="c92e4-108">**Note:** Office installation issues commonly occur due to misconfigured or malformatted configuration files.</span></span> <span data-ttu-id="c92e4-109">لتجنب هذه المشاكل ، ننصحك باستخدام أداه تخصيص Office لإنشاء ملف التكوين.</span><span class="sxs-lookup"><span data-stu-id="c92e4-109">To avoid such issues, we recommend that you use the Office Customization Tool to create the configuration file.</span></span> <span data-ttu-id="c92e4-110">يمكنك أيضا استيراد ملفات التكوين الموجودة في أداه تخصيص Office.</span><span class="sxs-lookup"><span data-stu-id="c92e4-110">You can also import existing configuration files into the Office Customization Tool.</span></span>

3. <span data-ttu-id="c92e4-111">من موجه أوامر غير مقيد ، انتقل إلى الموقع الذي setupodt.exe فيه وقم بتشغيل أداه نشر Office في وضع التنزيل وحدد ملف التكوين الذي حفظته للتو.</span><span class="sxs-lookup"><span data-stu-id="c92e4-111">From an elevated command prompt, switch to the location where setupodt.exe resides and run the Office Deployment Tool in download mode and specify the configuration file you just saved.</span></span> <span data-ttu-id="c92e4-112">في هذا المثال ، يتم تسميه ملف التكوين Configuration.xml:</span><span class="sxs-lookup"><span data-stu-id="c92e4-112">In this example, the configuration file is named Configuration.xml:</span></span>

```setupodt.exe /download Configuration.xml```

<span data-ttu-id="c92e4-113">4. قم بتشغيل أداه نشر Office في وضع التكوين وحدد ملف التكوين.</span><span class="sxs-lookup"><span data-stu-id="c92e4-113">4.Run the Office Deployment Tool in configure mode and specify the configuration file.</span></span>

```setupodt.exe /configure Configuration.xml```

<span data-ttu-id="c92e4-114">**ملاحظه:** يجب تشغيل هذه الخطوة من الكمبيوتر العميل الذي تريد تثبيت Office عليه ، ويجب ان يكون لديك أذونات المسؤول المحلي علي هذا الكمبيوتر.</span><span class="sxs-lookup"><span data-stu-id="c92e4-114">**Note:** You must run this step from the client computer on which you want to install Office and you must have local administrator permissions on that computer.</span></span>

<span data-ttu-id="c92e4-115">للحصول علي مزيد من المعلومات حول استخدام أداه النشر من Office الخاصة بتطبيقات Microsoft 365 لسيناريوهات نشر المؤسسة ، راجع [نظره عامه حول أداه نشر Office](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool).</span><span class="sxs-lookup"><span data-stu-id="c92e4-115">To learn more about using Office Deployment Tool for your Microsoft 365 Apps for enterprise deployment scenarios, see [Overview of the Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool).</span></span> <span data-ttu-id="c92e4-116">للحصول علي مزيد من التفاصيل حول كيفيه استخدام أداه تخصيص Office ، راجع [نظره عامه حول أداه تخصيص office](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span><span class="sxs-lookup"><span data-stu-id="c92e4-116">For more details on how to use the Office Customization Tool, see [Overview of the Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span></span>
