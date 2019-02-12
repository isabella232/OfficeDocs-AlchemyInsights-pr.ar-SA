---
title: فشل سير العمل مفقودة تنشيط
ms.author: kirks
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: ce088227a3206fa05b99331fdb022fbe4886203f
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/12/2019
ms.locfileid: "29917555"
---
# <a name="missing-workflow-failed-to-activate"></a><span data-ttu-id="b2242-102">فشل سير العمل مفقودة تنشيط</span><span class="sxs-lookup"><span data-stu-id="b2242-102">Missing Workflow Failed to Activate</span></span>

<span data-ttu-id="b2242-103">في مجموعة موقع Microsoft SharePoint، لا يمكنك إضافة سير عمل القابل لإعادة الاستخدام على الصعيد العالمي (مثل "الموافقة-SharePoint 2010") إلى قائمة أو مكتبة.</span><span class="sxs-lookup"><span data-stu-id="b2242-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="b2242-104">لحل هذه المشكلة، اتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="b2242-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="b2242-105">افتح موقع ويب الجذر لمجموعة الموقع في SharePoint مصمم 2013.</span><span class="sxs-lookup"><span data-stu-id="b2242-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="b2242-106">ضمن **موقع الكائنات**، حدد **مهام سير العمل**.</span><span class="sxs-lookup"><span data-stu-id="b2242-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="b2242-107">في مقطع **جديد** في "الشريط" **مهام سير العمل** ، قم بتحديد **سير العمل القابل لإعادة الاستخدام**.</span><span class="sxs-lookup"><span data-stu-id="b2242-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="b2242-p101">في النموذج **إنشاء سير العمل القابل لإعادة الاستخدام** ، أدخل الاسم \* \* *Repair2010* \* \*. **نوع النظام الأساسي**، انقر فوق **سير العمل 2010 SharePoint**ومن ثم انقر فوق **موافق**.</span><span class="sxs-lookup"><span data-stu-id="b2242-p101">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*. For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="b2242-110">في المقطع **حفظ** **سير العمل** "الشريط"، حدد " **نشر**".</span><span class="sxs-lookup"><span data-stu-id="b2242-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="b2242-p102">في المقطع **إدارة** الشريط **سير العمل** ، حدد **نشر على الصعيد العالمي**. في مربع الحوار التأكيد التي تظهر، حدد **"موافق"**.</span><span class="sxs-lookup"><span data-stu-id="b2242-p102">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**. In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="b2242-p103">في مستعرض ويب، حدد موقع ويب الجذر لمجموعة الموقع ومن ثم الوصول إلى **إعدادات الموقع** \> **ميزات مجموعة الموقع**. وبعد ذلك، تبديل ميزة **سير العمل** :</span><span class="sxs-lookup"><span data-stu-id="b2242-p103">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**. Then, toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="b2242-115">· إذا كانت الميزة *نشطة* ، انقر فوق **إلغاء تنشيط،** ومن ثم انقر فوق **تنشيط**.</span><span class="sxs-lookup"><span data-stu-id="b2242-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="b2242-116">· إذا كانت الميزة *Deactivated* ، انقر فوق **تنشيط**.</span><span class="sxs-lookup"><span data-stu-id="b2242-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="b2242-117">لمزيد من المعلومات الرجاء الرجوع إلى [المقالة](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)التالية.</span><span class="sxs-lookup"><span data-stu-id="b2242-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

