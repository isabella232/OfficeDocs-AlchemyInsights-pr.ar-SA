---
title: فشل تنشيط سير العمل المفقود
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: 2598111005c219c398b63ca374e8e99348efc02c
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43762088"
---
# <a name="missing-workflow-failed-to-activate"></a><span data-ttu-id="2287a-102">فشل تنشيط سير العمل المفقود</span><span class="sxs-lookup"><span data-stu-id="2287a-102">Missing Workflow Failed to Activate</span></span>

<span data-ttu-id="2287a-103">في مجموعة مواقع Microsoft SharePoint، لا يمكنك إضافة سير عمل قابل لإعادة للاستخدام عالميًا (مثل "الموافقة - SharePoint 2010") إلى قائمة أو مكتبة.</span><span class="sxs-lookup"><span data-stu-id="2287a-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="2287a-104">لحل هذه المشكلة، اتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="2287a-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="2287a-105">افتح موقع الويب الجذر لمجموعة الموقع في SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="2287a-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="2287a-106">ضمن **كائنات الموقع،** حدد **سير العمل**.</span><span class="sxs-lookup"><span data-stu-id="2287a-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="2287a-107">في القسم **الجديد** من شريط **سير العمل،** حدد **سير العمل القابل لإعادة للاستخدام**.</span><span class="sxs-lookup"><span data-stu-id="2287a-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="2287a-108">في نموذج **إنشاء سير عمل قابل لإعادة للاستخدام،** أدخل الاسم \*\* *Repair2010* \*\*.</span><span class="sxs-lookup"><span data-stu-id="2287a-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="2287a-109">لنوع **النظام الأساسي**، انقر فوق **SharePoint 2010 سير العمل**، ثم انقر فوق **موافق**.</span><span class="sxs-lookup"><span data-stu-id="2287a-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="2287a-110">في قسم **حفظ** شريط **سير العمل،** حدد **نشر**.</span><span class="sxs-lookup"><span data-stu-id="2287a-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="2287a-111">في **قسم إدارة** شريط **سير العمل،** حدد **النشر عالمياً**.</span><span class="sxs-lookup"><span data-stu-id="2287a-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="2287a-112">في مربع حوار التأكيد الذي يظهر، حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="2287a-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="2287a-113">في مستعرض ويب، حدد موقع الويب الجذر لمجموعة الموقع، ثم قم بالوصول إلى **ميزات مجموعة مواقع**إعدادات \> **الموقع** .</span><span class="sxs-lookup"><span data-stu-id="2287a-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="2287a-114">ثم قم بتبديل ميزة **سير العمل:**</span><span class="sxs-lookup"><span data-stu-id="2287a-114">Then, toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="2287a-115">· إذا تم *تنشيط* الميزة، انقر فوق **إلغاء التنشيط،** ثم انقر فوق **تنشيط**.</span><span class="sxs-lookup"><span data-stu-id="2287a-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="2287a-116">· إذا تم *إلغاء تنشيط* الميزة، انقر فوق **تنشيط**.</span><span class="sxs-lookup"><span data-stu-id="2287a-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="2287a-117">لمزيد من المعلومات يرجى الرجوع إلى [المادة](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)التالية.</span><span class="sxs-lookup"><span data-stu-id="2287a-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

