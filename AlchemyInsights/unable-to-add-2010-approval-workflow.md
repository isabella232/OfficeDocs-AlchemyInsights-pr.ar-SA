---
title: غير قادر على إضافة "سير عمل الموافقة" 2010
ms.author: kirks
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: 3741b1169ddf731725c18fbaed80bfb321e5db46
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/23/2019
ms.locfileid: "32366822"
---
# <a name="unable-to-add-2010-approval-workflow"></a><span data-ttu-id="f83bf-102">غير قادر على إضافة "سير عمل الموافقة" 2010</span><span class="sxs-lookup"><span data-stu-id="f83bf-102">Unable to add 2010 Approval Workflow</span></span>

<span data-ttu-id="f83bf-103">في مجموعة موقع Microsoft SharePoint، لا يمكنك إضافة سير عمل القابل لإعادة الاستخدام على الصعيد العالمي (مثل "الموافقة-SharePoint 2010") إلى قائمة أو مكتبة.</span><span class="sxs-lookup"><span data-stu-id="f83bf-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="f83bf-104">لحل هذه المشكلة، اتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="f83bf-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="f83bf-105">افتح موقع ويب الجذر لمجموعة الموقع في SharePoint مصمم 2013.</span><span class="sxs-lookup"><span data-stu-id="f83bf-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="f83bf-106">ضمن **موقع الكائنات**، حدد **مهام سير العمل**.</span><span class="sxs-lookup"><span data-stu-id="f83bf-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="f83bf-107">في مقطع **جديد** في "الشريط" **مهام سير العمل** ، قم بتحديد **سير العمل القابل لإعادة الاستخدام**.</span><span class="sxs-lookup"><span data-stu-id="f83bf-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="f83bf-108">في النموذج **إنشاء سير العمل القابل لإعادة الاستخدام** ، أدخل الاسم \* \* *Repair2010* \* \*.</span><span class="sxs-lookup"><span data-stu-id="f83bf-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="f83bf-109">**نوع النظام الأساسي**، انقر فوق **سير العمل 2010 SharePoint**ومن ثم انقر فوق **موافق**.</span><span class="sxs-lookup"><span data-stu-id="f83bf-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="f83bf-110">في المقطع **حفظ** **سير العمل** "الشريط"، حدد " **نشر**".</span><span class="sxs-lookup"><span data-stu-id="f83bf-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="f83bf-111">في المقطع **إدارة** الشريط **سير العمل** ، حدد **نشر على الصعيد العالمي**.</span><span class="sxs-lookup"><span data-stu-id="f83bf-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="f83bf-112">في مربع الحوار التأكيد التي تظهر، حدد **"موافق"**.</span><span class="sxs-lookup"><span data-stu-id="f83bf-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="f83bf-113">في مستعرض ويب، حدد موقع ويب الجذر لمجموعة الموقع ومن ثم الوصول إلى **إعدادات الموقع** \> **ميزات مجموعة الموقع**.</span><span class="sxs-lookup"><span data-stu-id="f83bf-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="f83bf-114">تبديل ميزة **سير العمل** :</span><span class="sxs-lookup"><span data-stu-id="f83bf-114">Toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="f83bf-115">· إذا كانت الميزة *نشطة* ، انقر فوق **إلغاء تنشيط،** ومن ثم انقر فوق **تنشيط**.</span><span class="sxs-lookup"><span data-stu-id="f83bf-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="f83bf-116">· إذا كانت الميزة *Deactivated* ، انقر فوق **تنشيط**.</span><span class="sxs-lookup"><span data-stu-id="f83bf-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="f83bf-117">لمزيد من المعلومات الرجاء الرجوع إلى [المقالة](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)التالية.</span><span class="sxs-lookup"><span data-stu-id="f83bf-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

