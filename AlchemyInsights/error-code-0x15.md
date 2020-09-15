---
title: رمز الخطا 0x15
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: إذا كنت تتلقي رسالة خطا اثناء تنشيط Office 2013 علي عمليات نشر خدمات سطح المكتب البعيد (RDS) ، فيمكنك تمكين ADAL عن طريق تحرير السجل.
ms.openlocfilehash: deb2ac4b0fb6a7b2e0045ff1b0ba95ad6e5e4a3a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709174"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a><span data-ttu-id="c1288-103">خطا اثناء تنشيط Office 2013 علي خدمات سطح المكتب البعيد</span><span class="sxs-lookup"><span data-stu-id="c1288-103">Error while activation Office 2013 on Remote Desktop Services</span></span>

<span data-ttu-id="c1288-104">إذا كنت تتلقي رسالة خطا اثناء تنشيط Office 2013 علي عمليات نشر خدمات سطح المكتب البعيد (RDS) ، فيمكنك تمكين ADAL عن طريق تحرير السجل.</span><span class="sxs-lookup"><span data-stu-id="c1288-104">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span>
  
|<span data-ttu-id="c1288-105">**مفتاح التسجيل**</span><span class="sxs-lookup"><span data-stu-id="c1288-105">**Registry key**</span></span>|<span data-ttu-id="c1288-106">**اكتب**</span><span class="sxs-lookup"><span data-stu-id="c1288-106">**Type**</span></span>|<span data-ttu-id="c1288-107">**Value**</span><span class="sxs-lookup"><span data-stu-id="c1288-107">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="c1288-108">HKEY_CURRENT_USER \Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="c1288-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="c1288-109">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="c1288-109">REG_DWORD</span></span>  <br/> |<span data-ttu-id="c1288-110">1</span><span class="sxs-lookup"><span data-stu-id="c1288-110">1</span></span>  <br/> |

<span data-ttu-id="c1288-111">لمزيد من المعلومات ، راجع [تمكين المصادقة الحديثة ل Office 2013 علي أجهزه Windows](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="c1288-111">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="c1288-112">يتم تمكين ADAL بشكل افتراضي في تطبيقات Microsoft 365 ل enterprise و Office 2016.</span><span class="sxs-lookup"><span data-stu-id="c1288-112">ADAL is enabled by default in Microsoft 365 Apps for enterprise and Office 2016.</span></span> <span data-ttu-id="c1288-113">تمت تسميه خدمات سطح المكتب البعيد (RDS) مسبقا بالخدمات الطرفية.</span><span class="sxs-lookup"><span data-stu-id="c1288-113">Remote Desktop Services (RDS) was previously named Terminal Services.</span></span>
  