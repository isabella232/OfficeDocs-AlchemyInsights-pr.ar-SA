---
title: باستخدام أداة نشر Office
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: c7e0e96f225030590fdd516eaf3115c93a6335b6
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/23/2019
ms.locfileid: "32423170"
---
# <a name="using-the-office-deployment-tool-odt"></a><span data-ttu-id="9f86d-102">باستخدام أداة نشر Office (ODT)</span><span class="sxs-lookup"><span data-stu-id="9f86d-102">Using the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="9f86d-103">يمكنك استخدام أداة نشر Office (ODT) لنشر إصدارات Office 365 من Office.</span><span class="sxs-lookup"><span data-stu-id="9f86d-103">You use the Office Deployment Tool (ODT) to deploy Office 365 versions of Office.</span></span> <span data-ttu-id="9f86d-104">أداة نشر Office (setup.exe) من سطر الأوامر ويستخدم ملف تكوين XML لتحديد الإعدادات لتطبيق مستندات Office.</span><span class="sxs-lookup"><span data-stu-id="9f86d-104">The Office Deployment Tool (setup.exe) is run from the command line and uses a configuration XML file to determine what settings to apply when deploying Office.</span></span>
  
1. <span data-ttu-id="9f86d-105">تنزيل أحدث إصدار من "الأداة Office النشر" من ["مركز تحميل microsoft"](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="9f86d-105">Download the latest version of the Office Deployment Tool from the [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
    
2. <span data-ttu-id="9f86d-106">استخدام [أداة تخصيص Office (OCT)](https://config.office.com) لتحديد تفضيلات التوزيع وإنشاء ملف تكوين XML.</span><span class="sxs-lookup"><span data-stu-id="9f86d-106">Use the [Office Customization Tool (OCT)](https://config.office.com) to select your deployment preferences and create the configuration XML file.</span></span> <span data-ttu-id="9f86d-107">تصدير ملف التكوين ووضعه محلياً في نفس المجلد حيث يوجد setup.exe.</span><span class="sxs-lookup"><span data-stu-id="9f86d-107">Export the configuration file and place it locally on the same folder where the setup.exe resides.</span></span> 
    
    <span data-ttu-id="9f86d-108">**ملاحظة:** عادة ما تحدث مشكلات المستحقة لصحيح تثبيت office أو ملفات التكوين مالفورماتيد.</span><span class="sxs-lookup"><span data-stu-id="9f86d-108">**Note:** Office installation issues commonly occur due to misconfigured or malformatted configuration files.</span></span> <span data-ttu-id="9f86d-109">لتجنب مثل هذه المشكلات، نوصي باستخدام "أداة تخصيص Office" لإنشاء ملف التكوين.</span><span class="sxs-lookup"><span data-stu-id="9f86d-109">To avoid such issues, we recommend that you use the Office Customization Tool to create the configuration file.</span></span> <span data-ttu-id="9f86d-110">يمكنك أيضا استيراد ملفات التكوين الموجودة في أداة تخصيص Office.</span><span class="sxs-lookup"><span data-stu-id="9f86d-110">You can also import existing configuration files into the Office Customization Tool.</span></span> 
    
3. <span data-ttu-id="9f86d-111">من موجه أوامر غير مقيد، قم بالتبديل إلى المجلد حيث يوجد setup.exe وتشغيل أداة نشر Office في وضع الخطوط وتحديد ملف التكوين الذي قمت بحفظه.</span><span class="sxs-lookup"><span data-stu-id="9f86d-111">From an elevated command prompt, switch to the location where setup.exe resides and run the Office Deployment Tool in download mode and specify the configuration file you just saved.</span></span> <span data-ttu-id="9f86d-112">في هذا المثال، يتم تسمية ملف التكوين Configuration.xml:</span><span class="sxs-lookup"><span data-stu-id="9f86d-112">In this example, the configuration file is named Configuration.xml:</span></span>
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. <span data-ttu-id="9f86d-113">تشغيل أداة نشر Office في تكوين وضع وحدد ملف التكوين.</span><span class="sxs-lookup"><span data-stu-id="9f86d-113">Run the Office Deployment Tool in configure mode and specify the configuration file.</span></span>
    
  ```
  setup.exe /configure Configuration.xml
  ```

    <span data-ttu-id="9f86d-114">**ملاحظة:** يجب تشغيل هذه الخطوة من جهاز الكمبيوتر العميل الذي تريد تثبيت Office ويجب أن يكون لديك أذونات المسؤول المحلية على هذا الكمبيوتر.</span><span class="sxs-lookup"><span data-stu-id="9f86d-114">**Note:** You must run this step from the client computer on which you want to install Office and you must have local administrator permissions on that computer.</span></span> 
    
<span data-ttu-id="9f86d-115">لمزيد من المعلومات حول استخدام أداة نشر Office لسيناريوهات النشر Office 365 ProPlus، راجع [نظرة عامة حول أداة نشر Office](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool).</span><span class="sxs-lookup"><span data-stu-id="9f86d-115">To learn more about using Office Deployment Tool for your Office 365 ProPlus deployment scenarios, see [Overview of the Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool).</span></span> <span data-ttu-id="9f86d-116">للحصول على مزيد من التفاصيل حول كيفية استخدام أداة تخصيص Office، راجع [نظرة عامة حول أداة تخصيص Office](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span><span class="sxs-lookup"><span data-stu-id="9f86d-116">For more details on how to use the Office Customization Tool, see [Overview of the Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span></span>
  

