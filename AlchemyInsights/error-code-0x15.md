---
title: رمز الخطأ 0x15
ms.author: pebaum
author: pebaum
ms.date: 10/31/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: إذا كنت تتلقى خطأ أثناء تنشيط Office 2013 على عمليات نشر خدمات سطح المكتب البعيد (RDS)، خذ بعين الاعتبار تمكين إنبات عن طريق تحرير التسجيل.
ms.openlocfilehash: 89f9270169e13fd7706f7826c624ef8ae4d47b3f
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/24/2019
ms.locfileid: "29499369"
---
<span data-ttu-id="d3c1d-103">إذا كنت تتلقى خطأ أثناء تنشيط Office 2013 على عمليات نشر خدمات سطح المكتب البعيد (RDS)، خذ بعين الاعتبار تمكين إنبات عن طريق تحرير التسجيل.</span><span class="sxs-lookup"><span data-stu-id="d3c1d-103">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span> 
  
|<span data-ttu-id="d3c1d-104">**مفتاح التسجيل**</span><span class="sxs-lookup"><span data-stu-id="d3c1d-104">**Registry key**</span></span>|<span data-ttu-id="d3c1d-105">اكتب </span><span class="sxs-lookup"><span data-stu-id="d3c1d-105">**Type**</span></span>|<span data-ttu-id="d3c1d-106">القيمة</span><span class="sxs-lookup"><span data-stu-id="d3c1d-106">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="d3c1d-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="d3c1d-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="d3c1d-108">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="d3c1d-108">REG_DWORD</span></span>  <br/> |<span data-ttu-id="d3c1d-109">1</span><span class="sxs-lookup"><span data-stu-id="d3c1d-109">1</span></span>  <br/> |
   
<span data-ttu-id="d3c1d-110">لمزيد من المعلومات، راجع [تمكين مصادقة الحديثة ل 2013 Office على أجهزة Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="d3c1d-110">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="d3c1d-p101">يتم تمكين إنبات افتراضياً في Office 365 ProPlus ومكتب عام 2016. تم مسبقاً يسمى > خدمات سطح المكتب البعيد (RDS) "الخدمات الطرفية".</span><span class="sxs-lookup"><span data-stu-id="d3c1d-p101">ADAL is enabled by default in Office 365 ProPlus and Office 2016. >  Remote Desktop Services (RDS) was previously named Terminal Services.</span></span> 
  

