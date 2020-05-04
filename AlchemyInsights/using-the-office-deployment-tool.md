---
title: استخدام أداة نشر Office
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: d941bce524dc797d5dcbb7213bded6919fd01b7d
ms.sourcegitcommit: 7e06d9ec1dd462cbd882f088c997d012a032f04d
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/04/2020
ms.locfileid: "44010830"
---
# <a name="using-the-office-deployment-tool-odt"></a><span data-ttu-id="54649-102">استخدام أداة نشر Office (ODT)</span><span class="sxs-lookup"><span data-stu-id="54649-102">Using the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="54649-103">يمكنك استخدام أداة نشر Office (ODT) لنشر إصدارات Office 365 من Office.</span><span class="sxs-lookup"><span data-stu-id="54649-103">You use the Office Deployment Tool (ODT) to deploy Office 365 versions of Office.</span></span> <span data-ttu-id="54649-104">يتم تشغيل أداة نشر Office (setup.exe) من سطر الأوامر وتستخدم ملف XML التكوين لتحديد الإعدادات التي يجب تطبيقها عند نشر Office.</span><span class="sxs-lookup"><span data-stu-id="54649-104">The Office Deployment Tool (setup.exe) is run from the command line and uses a configuration XML file to determine what settings to apply when deploying Office.</span></span>
  
1. <span data-ttu-id="54649-105">قم بتنزيل أحدث إصدار من أداة نشر Office من [مركز تنزيل Microsoft](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="54649-105">Download the latest version of the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>

2. <span data-ttu-id="54649-106">استخدم [أداة تخصيص Office (OCT)](https://config.office.com) لتحديد تفضيلات النشر وإنشاء ملف XML التكوين.</span><span class="sxs-lookup"><span data-stu-id="54649-106">Use the [Office Customization Tool (OCT)](https://config.office.com) to select your deployment preferences and create the configuration XML file.</span></span> <span data-ttu-id="54649-107">تصدير ملف التكوين ووضعه محلياً على نفس المجلد حيث يقيم setup.exe.</span><span class="sxs-lookup"><span data-stu-id="54649-107">Export the configuration file and place it locally on the same folder where the setup.exe resides.</span></span>

    <span data-ttu-id="54649-108">**ملاحظة:** تحدث مشكلات تثبيت Office عادةً بسبب ملفات التكوين التي تم تكوينها بشكل خاطئ أو مالفّنة.</span><span class="sxs-lookup"><span data-stu-id="54649-108">**Note:** Office installation issues commonly occur due to misconfigured or malformatted configuration files.</span></span> <span data-ttu-id="54649-109">لتجنب مثل هذه المشكلات، نوصي باستخدام أداة تخصيص Office لإنشاء ملف التكوين.</span><span class="sxs-lookup"><span data-stu-id="54649-109">To avoid such issues, we recommend that you use the Office Customization Tool to create the configuration file.</span></span> <span data-ttu-id="54649-110">يمكنك أيضًا استيراد ملفات التكوين الموجودة إلى أداة تخصيص Office.</span><span class="sxs-lookup"><span data-stu-id="54649-110">You can also import existing configuration files into the Office Customization Tool.</span></span>

3. <span data-ttu-id="54649-111">من مطالبة الأمر المرتفعة، قم بالتبديل إلى الموقع الذي يتواجد فيه setup.exe واشغّل أداة نشر Office في وضع التنزيل وحدد ملف التكوين الذي قمت بحفظه للتو.</span><span class="sxs-lookup"><span data-stu-id="54649-111">From an elevated command prompt, switch to the location where setup.exe resides and run the Office Deployment Tool in download mode and specify the configuration file you just saved.</span></span> <span data-ttu-id="54649-112">في هذا المثال، يتم تسمية ملف التكوين Configuration.xml:</span><span class="sxs-lookup"><span data-stu-id="54649-112">In this example, the configuration file is named Configuration.xml:</span></span>
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. <span data-ttu-id="54649-113">تشغيل أداة نشر Office في وضع التكوين وتحديد ملف التكوين.</span><span class="sxs-lookup"><span data-stu-id="54649-113">Run the Office Deployment Tool in configure mode and specify the configuration file.</span></span>
    
  ```
  setup.exe /configure Configuration.xml
  ```

    <span data-ttu-id="54649-114">**ملاحظة:** يجب تشغيل هذه الخطوة من الكمبيوتر العميل الذي تريد تثبيت Office ويجب أن يكون لديك أذونات المسؤول المحلي على هذا الكمبيوتر.</span><span class="sxs-lookup"><span data-stu-id="54649-114">**Note:** You must run this step from the client computer on which you want to install Office and you must have local administrator permissions on that computer.</span></span>

<span data-ttu-id="54649-115">لمعرفة المزيد حول استخدام أداة نشر Office لتطبيقات Microsoft 365 لسيناريوهات نشر المؤسسة، راجع [نظرة عامة على أداة نشر Office](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool).</span><span class="sxs-lookup"><span data-stu-id="54649-115">To learn more about using Office Deployment Tool for your Microsoft 365 Apps for enterprise deployment scenarios, see [Overview of the Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool).</span></span> <span data-ttu-id="54649-116">لمزيد من التفاصيل حول كيفية استخدام أداة تخصيص Office، راجع [نظرة عامة على أداة تخصيص Office](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span><span class="sxs-lookup"><span data-stu-id="54649-116">For more details on how to use the Office Customization Tool, see [Overview of the Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span></span>
