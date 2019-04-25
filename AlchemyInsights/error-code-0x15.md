---
title: رمز الخطأ 0x15
ms.author: pebaum
author: pebaum
ms.date: 10/31/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: إذا كنت تتلقى خطأ أثناء تنشيط Office 2013 على عمليات نشر خدمات سطح المكتب البعيد (RDS)، خذ بعين الاعتبار تمكين إنبات عن طريق تحرير التسجيل.
ms.openlocfilehash: 6d4076ecb5c6ee3c3cf4c4610ad4aa29ab477d8a
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/23/2019
ms.locfileid: "32402726"
---
<span data-ttu-id="7ddd8-103">إذا كنت تتلقى خطأ أثناء تنشيط Office 2013 على عمليات نشر خدمات سطح المكتب البعيد (RDS)، خذ بعين الاعتبار تمكين إنبات عن طريق تحرير التسجيل.</span><span class="sxs-lookup"><span data-stu-id="7ddd8-103">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span> 
  
|<span data-ttu-id="7ddd8-104">**مفتاح التسجيل**</span><span class="sxs-lookup"><span data-stu-id="7ddd8-104">**Registry key**</span></span>|<span data-ttu-id="7ddd8-105">**نوع**</span><span class="sxs-lookup"><span data-stu-id="7ddd8-105">**Type**</span></span>|<span data-ttu-id="7ddd8-106">**القيمة**</span><span class="sxs-lookup"><span data-stu-id="7ddd8-106">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="7ddd8-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="7ddd8-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="7ddd8-108">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="7ddd8-108">REG_DWORD</span></span>  <br/> |<span data-ttu-id="7ddd8-109">1</span><span class="sxs-lookup"><span data-stu-id="7ddd8-109">1</span></span>  <br/> |
   
<span data-ttu-id="7ddd8-110">لمزيد من المعلومات، راجع [تمكين مصادقة الحديثة ل 2013 Office على أجهزة Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="7ddd8-110">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="7ddd8-111">يتم تمكين إنبات افتراضياً في Office 365 ProPlus ومكتب عام 2016.</span><span class="sxs-lookup"><span data-stu-id="7ddd8-111">ADAL is enabled by default in Office 365 ProPlus and Office 2016.</span></span> <span data-ttu-id="7ddd8-112">تم مسبقاً يسمى > خدمات سطح المكتب البعيد (RDS) "الخدمات الطرفية".</span><span class="sxs-lookup"><span data-stu-id="7ddd8-112">>  Remote Desktop Services (RDS) was previously named Terminal Services.</span></span> 
  

