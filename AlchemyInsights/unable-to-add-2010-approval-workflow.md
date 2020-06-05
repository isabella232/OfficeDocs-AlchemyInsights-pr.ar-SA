---
title: غير قادر على إضافة سير عمل الموافقة لعام 2010
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: f40716dd399fe7bea1b606cd725676268dc0a66d
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582834"
---
# <a name="unable-to-add-2010-approval-workflow"></a><span data-ttu-id="c0bd6-102">غير قادر على إضافة سير عمل الموافقة لعام 2010</span><span class="sxs-lookup"><span data-stu-id="c0bd6-102">Unable to add 2010 Approval Workflow</span></span>

<span data-ttu-id="c0bd6-103">في مجموعة مواقع Microsoft SharePoint، لا يمكنك إضافة سير عمل قابل لإعادة للاستخدام عالميًا (مثل "الموافقة - SharePoint 2010") إلى قائمة أو مكتبة.</span><span class="sxs-lookup"><span data-stu-id="c0bd6-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="c0bd6-104">لحل هذه المشكلة، اتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="c0bd6-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="c0bd6-105">افتح موقع الويب الجذر لمجموعة الموقع في SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="c0bd6-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="c0bd6-106">ضمن **كائنات الموقع،** حدد **سير العمل**.</span><span class="sxs-lookup"><span data-stu-id="c0bd6-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="c0bd6-107">في القسم **الجديد** من شريط **سير العمل،** حدد **سير العمل القابل لإعادة للاستخدام**.</span><span class="sxs-lookup"><span data-stu-id="c0bd6-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="c0bd6-108">في نموذج **إنشاء سير عمل قابل لإعادة للاستخدام،** أدخل الاسم \*\* *Repair2010* \*\*.</span><span class="sxs-lookup"><span data-stu-id="c0bd6-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="c0bd6-109">لنوع **النظام الأساسي**، انقر فوق **SharePoint 2010 سير العمل**، ثم انقر فوق **موافق**.</span><span class="sxs-lookup"><span data-stu-id="c0bd6-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="c0bd6-110">في قسم **حفظ** شريط **سير العمل،** حدد **نشر**.</span><span class="sxs-lookup"><span data-stu-id="c0bd6-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="c0bd6-111">في **قسم إدارة** شريط **سير العمل،** حدد **النشر عالمياً**.</span><span class="sxs-lookup"><span data-stu-id="c0bd6-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="c0bd6-112">في مربع حوار التأكيد الذي يظهر، حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="c0bd6-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="c0bd6-113">في مستعرض ويب، حدد موقع الويب الجذر لمجموعة الموقع، ثم قم بالوصول إلى ميزات مجموعة مواقع إعدادات **الموقع** \> **Site Collection Features**.</span><span class="sxs-lookup"><span data-stu-id="c0bd6-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="c0bd6-114">تبديل ميزة **سير العمل:**</span><span class="sxs-lookup"><span data-stu-id="c0bd6-114">Toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="c0bd6-115">· إذا تم *تنشيط* الميزة، انقر فوق **إلغاء التنشيط،** ثم انقر فوق **تنشيط**.</span><span class="sxs-lookup"><span data-stu-id="c0bd6-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="c0bd6-116">· إذا تم *إلغاء تنشيط* الميزة، انقر فوق **تنشيط**.</span><span class="sxs-lookup"><span data-stu-id="c0bd6-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="c0bd6-117">لمزيد من المعلومات يرجى الرجوع إلى [المادة](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)التالية.</span><span class="sxs-lookup"><span data-stu-id="c0bd6-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

