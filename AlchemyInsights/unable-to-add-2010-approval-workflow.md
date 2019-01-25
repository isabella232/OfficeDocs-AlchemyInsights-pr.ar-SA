---
title: غير قادر على إضافة "سير عمل الموافقة" 2010
ms.author: kirks
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: a83a9621ca0f7764d3f2c0a698dbffd80d55e80c
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/24/2019
ms.locfileid: "29456347"
---
# <a name="unable-to-add-2010-approval-workflow"></a><span data-ttu-id="800a2-102">غير قادر على إضافة "سير عمل الموافقة" 2010</span><span class="sxs-lookup"><span data-stu-id="800a2-102">Unable to add 2010 Approval Workflow</span></span>

<span data-ttu-id="800a2-103">في مجموعة موقع Microsoft SharePoint، لا يمكنك إضافة سير عمل القابل لإعادة الاستخدام على الصعيد العالمي (مثل "الموافقة-SharePoint 2010") إلى قائمة أو مكتبة.</span><span class="sxs-lookup"><span data-stu-id="800a2-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="800a2-104">لحل هذه المشكلة، اتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="800a2-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="800a2-105">افتح موقع ويب الجذر لمجموعة الموقع في SharePoint مصمم 2013.</span><span class="sxs-lookup"><span data-stu-id="800a2-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="800a2-106">ضمن **موقع الكائنات**، حدد **مهام سير العمل**.</span><span class="sxs-lookup"><span data-stu-id="800a2-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="800a2-107">في مقطع **جديد** في "الشريط" **مهام سير العمل** ، قم بتحديد **سير العمل القابل لإعادة الاستخدام**.</span><span class="sxs-lookup"><span data-stu-id="800a2-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="800a2-p101">في النموذج **إنشاء سير العمل القابل لإعادة الاستخدام** ، أدخل الاسم \* \* *Repair2010* \* \*. **نوع النظام الأساسي**، انقر فوق **سير العمل 2010 SharePoint**ومن ثم انقر فوق **موافق**.</span><span class="sxs-lookup"><span data-stu-id="800a2-p101">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*. For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="800a2-110">في المقطع **حفظ** **سير العمل** "الشريط"، حدد " **نشر**".</span><span class="sxs-lookup"><span data-stu-id="800a2-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="800a2-p102">في المقطع **إدارة** الشريط **سير العمل** ، حدد **نشر على الصعيد العالمي**. في مربع الحوار التأكيد التي تظهر، حدد **"موافق"**.</span><span class="sxs-lookup"><span data-stu-id="800a2-p102">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**. In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="800a2-p103">في مستعرض ويب، حدد موقع ويب الجذر لمجموعة الموقع ومن ثم الوصول إلى **إعدادات الموقع** \> **ميزات مجموعة الموقع**. تبديل ميزة **سير العمل** :</span><span class="sxs-lookup"><span data-stu-id="800a2-p103">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**. Toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="800a2-115">· إذا كانت الميزة *نشطة* ، انقر فوق **إلغاء تنشيط،** ومن ثم انقر فوق **تنشيط**.</span><span class="sxs-lookup"><span data-stu-id="800a2-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="800a2-116">· إذا كانت الميزة *Deactivated* ، انقر فوق **تنشيط**.</span><span class="sxs-lookup"><span data-stu-id="800a2-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="800a2-117">لمزيد من المعلومات الرجاء الرجوع إلى [المقالة](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)التالية.</span><span class="sxs-lookup"><span data-stu-id="800a2-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

