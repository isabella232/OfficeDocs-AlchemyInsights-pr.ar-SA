---
title: فشل تنشيط سير العمل المفقود
ms.author: pebaum
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: f03d7e1441465050c4b0608f4100f217b183d2e2
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 11/15/2019
ms.locfileid: "36753783"
---
# <a name="missing-workflow-failed-to-activate"></a><span data-ttu-id="9e5b2-102">فشل تنشيط سير العمل المفقود</span><span class="sxs-lookup"><span data-stu-id="9e5b2-102">Missing Workflow Failed to Activate</span></span>

<span data-ttu-id="9e5b2-103">في مجموعه موقع Microsoft SharePoint ، لا يمكنك أضافه سير عمل قابل لأعاده الاستخدام عالميا (مثل "الموافقة-SharePoint 2010") إلى قائمه أو مكتبه.</span><span class="sxs-lookup"><span data-stu-id="9e5b2-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="9e5b2-104">لحل هذه المشكلة ، اتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="9e5b2-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="9e5b2-105">فتح موقع ويب الجذر لمجموعه الموقع في SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="9e5b2-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="9e5b2-106">ضمن **كائنات الموقع**، حدد **مهام سير**العمل.</span><span class="sxs-lookup"><span data-stu-id="9e5b2-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="9e5b2-107">في المقطع **الجديد** من "الشريط **مهام سير** العمل" ، حدد سير الاستخدام **القابل**لأعاده الاستخدام.</span><span class="sxs-lookup"><span data-stu-id="9e5b2-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="9e5b2-108">في نموذج " **إنشاء سير العمل القابل** لأعاده الاستخدام" ، ادخل الاسم \* \* *Repair2010* \* \*.</span><span class="sxs-lookup"><span data-stu-id="9e5b2-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="9e5b2-109">**لنوع النظام الأساسي**، انقر فوق **سير العمل 2010 SharePoint**، ثم انقر فوق **موافق**.</span><span class="sxs-lookup"><span data-stu-id="9e5b2-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="9e5b2-110">في المقطع **حفظ** من شريط **سير العمل** ، حدد **نشر**.</span><span class="sxs-lookup"><span data-stu-id="9e5b2-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="9e5b2-111">في قسم **أداره** الشريط **سير العمل** ، حدد **نشر علي الصعيد العالمي**.</span><span class="sxs-lookup"><span data-stu-id="9e5b2-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="9e5b2-112">في مربع حوار التاكيد الذي يظهر ، حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="9e5b2-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="9e5b2-113">في مستعرض ويب ، حدد موقع ويب الجذر لمجموعه الموقع ، ثم قم بالوصول إلى **ميزات مجموعه موقع** **إعدادات** \> الموقع.</span><span class="sxs-lookup"><span data-stu-id="9e5b2-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="9e5b2-114">ثم ، تبديل ميزه **مهام سير** العمل:</span><span class="sxs-lookup"><span data-stu-id="9e5b2-114">Then, toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="9e5b2-115">· إذا تم *تنشيط* الميزة ، انقر فوق **إلغاء تنشيط ،** ثم انقر فوق **تنشيط**.</span><span class="sxs-lookup"><span data-stu-id="9e5b2-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="9e5b2-116">· إذا تم *إلغاء تنشيط* الميزة ، انقر فوق **تنشيط**.</span><span class="sxs-lookup"><span data-stu-id="9e5b2-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="9e5b2-117">لمزيد من المعلومات الرجاء الرجوع إلى [المقالة](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)التالية.</span><span class="sxs-lookup"><span data-stu-id="9e5b2-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

