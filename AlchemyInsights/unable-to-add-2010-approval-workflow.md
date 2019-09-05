---
title: غير قادر على إضافة سير عمل الموافقة 2010
ms.author: pebaum
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: 13e3ed6db8c31adb1eb5a556c0e5fbc437b3fdb1
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/04/2019
ms.locfileid: "36748671"
---
# <a name="unable-to-add-2010-approval-workflow"></a><span data-ttu-id="78109-102">غير قادر على إضافة سير عمل الموافقة 2010</span><span class="sxs-lookup"><span data-stu-id="78109-102">Unable to add 2010 Approval Workflow</span></span>

<span data-ttu-id="78109-103">في مجموعة موقع Microsoft SharePoint، لا يمكنك إضافة سير عمل قابل لإعادة الاستخدام بشكل عام (مثل "الموافقة - SharePoint 2010") إلى قائمة أو مكتبة.</span><span class="sxs-lookup"><span data-stu-id="78109-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="78109-104">لحل هذه المشكلة، اتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="78109-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="78109-105">فتح موقع ويب الجذر من مجموعة الموقع في 2013 مصمم SharePoint.</span><span class="sxs-lookup"><span data-stu-id="78109-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="78109-106">ضمن **كائنات الموقع**، حدد مهام سير **العمل**.</span><span class="sxs-lookup"><span data-stu-id="78109-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="78109-107">في المقطع **جديد** من شريط **مهام سير العمل،** حدد سير العمل القابل **لإعادة الاستخدام**.</span><span class="sxs-lookup"><span data-stu-id="78109-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="78109-108">في النموذج **إنشاء سير عمل قابل لإعادة الاستخدام،** أدخل الاسم \*\* *Repair2010* \*\*.</span><span class="sxs-lookup"><span data-stu-id="78109-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="78109-109">لنوع **النظام الأساسي**، انقر فوق سير عمل **SharePoint 2010**، ثم انقر فوق **موافق**.</span><span class="sxs-lookup"><span data-stu-id="78109-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="78109-110">في المقطع **حفظ** من شريط **سير العمل،** حدد **نشر**.</span><span class="sxs-lookup"><span data-stu-id="78109-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="78109-111">في المقطع **إدارة** شريط **سير العمل،** حدد **نشر بشكل عمومي**.</span><span class="sxs-lookup"><span data-stu-id="78109-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="78109-112">في مربع حوار التأكيد الذي يظهر، حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="78109-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="78109-113">في مستعرض ويب، حدد موقع ويب الجذر لمجموعة الموقع، ثم قم بالوصول إلى **ميزات مجموعة موقع**إعدادات \> **الموقع** .</span><span class="sxs-lookup"><span data-stu-id="78109-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="78109-114">تبديل ميزة **مهام سير العمل:**</span><span class="sxs-lookup"><span data-stu-id="78109-114">Toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="78109-115">· إذا تم *تنشيط* الميزة ، انقر فوق **إلغاء التنشيط،** ثم انقر فوق **تنشيط**.</span><span class="sxs-lookup"><span data-stu-id="78109-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="78109-116">· إذا تم *إلغاء تنشيط* الميزة ، انقر فوق **تنشيط**.</span><span class="sxs-lookup"><span data-stu-id="78109-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="78109-117">لمزيد من المعلومات يرجى الرجوع إلى [المقالة](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)التالية .</span><span class="sxs-lookup"><span data-stu-id="78109-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

