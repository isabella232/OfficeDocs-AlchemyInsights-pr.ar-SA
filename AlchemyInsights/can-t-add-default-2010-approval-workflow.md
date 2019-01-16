---
title: لا يمكن إضافة الافتراضي 2010 "سير عمل الموافقة"
ms.author: kirks
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 2060c9a1-e714-4d93-925e-629c82c35986
ms.openlocfilehash: 758b0339b842478f9609eb716b5b4ddab6579c80
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/15/2019
ms.locfileid: "28272833"
---
# <a name="cant-add-default-2010-approval-workflow"></a><span data-ttu-id="9ba7f-102">لا يمكن إضافة الافتراضي 2010 "سير عمل الموافقة"</span><span class="sxs-lookup"><span data-stu-id="9ba7f-102">Can't add default 2010 Approval Workflow</span></span>

<span data-ttu-id="9ba7f-103">في مجموعة موقع Microsoft SharePoint، لا يمكنك إضافة سير عمل القابل لإعادة الاستخدام على الصعيد العالمي (مثل "الموافقة-SharePoint 2010") إلى قائمة أو مكتبة.</span><span class="sxs-lookup"><span data-stu-id="9ba7f-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="9ba7f-104">لحل هذه المشكلة، اتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="9ba7f-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="9ba7f-105">افتح موقع ويب الجذر لمجموعة الموقع في SharePoint مصمم 2013.</span><span class="sxs-lookup"><span data-stu-id="9ba7f-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="9ba7f-106">ضمن **موقع الكائنات**، حدد **مهام سير العمل**.</span><span class="sxs-lookup"><span data-stu-id="9ba7f-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="9ba7f-107">في مقطع **جديد** في "الشريط" **مهام سير العمل** ، قم بتحديد **سير العمل القابل لإعادة الاستخدام**.</span><span class="sxs-lookup"><span data-stu-id="9ba7f-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="9ba7f-p101">في النموذج **إنشاء سير العمل القابل لإعادة الاستخدام** ، أدخل الاسم \* \*\*Repair2010\*\*\*. **نوع النظام الأساسي**، حدد **سير العمل 2010 SharePoint**ومن ثم حدد **"موافق"**.</span><span class="sxs-lookup"><span data-stu-id="9ba7f-p101">On the **Create Reusable Workflow** form, enter the name  \* **Repair2010**\* . For **Platform Type**, select **SharePoint 2010 Workflow**, and then select **OK**.</span></span> 
  
5. <span data-ttu-id="9ba7f-110">في المقطع **حفظ** **سير العمل** "الشريط"، حدد " **نشر**".</span><span class="sxs-lookup"><span data-stu-id="9ba7f-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
6. <span data-ttu-id="9ba7f-p102">في المقطع **إدارة** الشريط **سير العمل** ، حدد **نشر على الصعيد العالمي**. في مربع الحوار التأكيد التي تظهر، حدد **"موافق"**.</span><span class="sxs-lookup"><span data-stu-id="9ba7f-p102">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**. In the confirmation dialog box that appears, select **OK**.</span></span> 
  
7. <span data-ttu-id="9ba7f-p103">في مستعرض ويب، حدد موقع ويب الجذر لمجموعة الموقع ومن ثم الوصول إلى **إعدادات الموقع** \> **ميزات مجموعة الموقع**. وبعد ذلك، تبديل ميزة **سير العمل** :</span><span class="sxs-lookup"><span data-stu-id="9ba7f-p103">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**. Then, toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="9ba7f-115">· إذا كانت الميزة *نشطة* ، انقر فوق **إلغاء تنشيط،** ومن ثم انقر فوق **تنشيط**.</span><span class="sxs-lookup"><span data-stu-id="9ba7f-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="9ba7f-116">· إذا كانت الميزة *Deactivated* ، انقر فوق **تنشيط**.</span><span class="sxs-lookup"><span data-stu-id="9ba7f-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="9ba7f-117">لمزيد من المعلومات الرجاء الرجوع إلى [المقالة](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)التالية.</span><span class="sxs-lookup"><span data-stu-id="9ba7f-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

