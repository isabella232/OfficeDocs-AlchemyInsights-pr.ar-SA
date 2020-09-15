---
title: تعذر أضافه سير عمل الموافقة علي 2010
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: aa61f1615b60d27cffad15f02f6ce5dbac1b607f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47699722"
---
# <a name="unable-to-add-2010-approval-workflow"></a><span data-ttu-id="0df58-102">تعذر أضافه سير عمل الموافقة علي 2010</span><span class="sxs-lookup"><span data-stu-id="0df58-102">Unable to add 2010 Approval Workflow</span></span>

<span data-ttu-id="0df58-103">في مجموعه مواقع مشتركه في Microsoft SharePoint ، لا يمكنك أضافه سير عمل قابل لأعاده الاستخدام بشكل عام (مثل "الموافقة علي SharePoint 2010") إلى قائمه أو مكتبه.</span><span class="sxs-lookup"><span data-stu-id="0df58-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="0df58-104">لحل هذه المشكلة ، اتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="0df58-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="0df58-105">افتح موقع ويب الجذر لمجموعه المواقع المشتركة في SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="0df58-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="0df58-106">ضمن **كائنات الموقع**، حدد **مهام سير العمل**.</span><span class="sxs-lookup"><span data-stu-id="0df58-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="0df58-107">في القسم **الجديد** من شريط **مهام سير العمل** ، حدد **سير العمل القابل لأعاده الاستخدام**.</span><span class="sxs-lookup"><span data-stu-id="0df58-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="0df58-108">في نموذج **إنشاء سير العمل القابل لأعاده الاستخدام** ، ادخل الاسم \* \* *Repair2010* \* \*.</span><span class="sxs-lookup"><span data-stu-id="0df58-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="0df58-109">بالنسبة إلى **نوع النظام الأساسي**، انقر فوق **سير عمل SharePoint 2010**، ثم انقر فوق **موافق**.</span><span class="sxs-lookup"><span data-stu-id="0df58-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="0df58-110">في القسم **حفظ** من شريط **سير العمل** ، حدد **نشر**.</span><span class="sxs-lookup"><span data-stu-id="0df58-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="0df58-111">في القسم **أداره** من شريط **سير العمل** ، حدد نشر بشكل **عام**.</span><span class="sxs-lookup"><span data-stu-id="0df58-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="0df58-112">في مربع حوار التاكيد الذي يظهر ، حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="0df58-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="0df58-113">في مستعرض ويب ، حدد موقع الموقع الجذر لمجموعه المواقع المشتركة **Site Settings** ، ثم قم بالوصول إلى \> **ميزات مجموعه المواقع المشتركة**لإعدادات الموقع.</span><span class="sxs-lookup"><span data-stu-id="0df58-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="0df58-114">تبديل ميزه **مهام سير العمل** :</span><span class="sxs-lookup"><span data-stu-id="0df58-114">Toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="0df58-115">· إذا تم  *تنشيط*  الميزة ، فانقر فوق **إلغاء تنشيط ،** ثم فوق **تنشيط**.</span><span class="sxs-lookup"><span data-stu-id="0df58-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="0df58-116">· إذا تم  *إلغاء تنشيط*  الميزة ، فانقر فوق **تنشيط**.</span><span class="sxs-lookup"><span data-stu-id="0df58-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="0df58-117">لمزيد من المعلومات ، يرجى مراجعه [المقالة](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)التالية.</span><span class="sxs-lookup"><span data-stu-id="0df58-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

