---
title: رمز الخطأ 0x15
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: إذا كنت تتلقى خطأ أثناء تنشيط Office 2013 على عمليات نشر خدمات سطح المكتب البعيد (RDS)، ففكر في تمكين ADAL عن طريق تحرير التسجيل.
ms.openlocfilehash: 566d63cbe37d295b3546b9d7d5b14dfc8e8fe0ec
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703125"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a><span data-ttu-id="01bcf-103">خطأ أثناء تفعيل Office 2013 على خدمات سطح المكتب البعيد</span><span class="sxs-lookup"><span data-stu-id="01bcf-103">Error while activation Office 2013 on Remote Desktop Services</span></span>

<span data-ttu-id="01bcf-104">إذا كنت تتلقى خطأ أثناء تنشيط Office 2013 على عمليات نشر خدمات سطح المكتب البعيد (RDS)، ففكر في تمكين ADAL عن طريق تحرير التسجيل.</span><span class="sxs-lookup"><span data-stu-id="01bcf-104">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span>
  
|<span data-ttu-id="01bcf-105">**مفتاح التسجيل**</span><span class="sxs-lookup"><span data-stu-id="01bcf-105">**Registry key**</span></span>|<span data-ttu-id="01bcf-106">**نوع**</span><span class="sxs-lookup"><span data-stu-id="01bcf-106">**Type**</span></span>|<span data-ttu-id="01bcf-107">**قيمه**</span><span class="sxs-lookup"><span data-stu-id="01bcf-107">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="01bcf-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="01bcf-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="01bcf-109">Reg_dword</span><span class="sxs-lookup"><span data-stu-id="01bcf-109">REG_DWORD</span></span>  <br/> |<span data-ttu-id="01bcf-110">1</span><span class="sxs-lookup"><span data-stu-id="01bcf-110">1</span></span>  <br/> |

<span data-ttu-id="01bcf-111">لمزيد من المعلومات، راجع [تمكين المصادقة الحديثة لـ Office 2013 على أجهزة Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="01bcf-111">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="01bcf-112">يتم تمكين ADAL بشكل افتراضي في تطبيقات Microsoft 365 للمؤسسات وOffice 2016.</span><span class="sxs-lookup"><span data-stu-id="01bcf-112">ADAL is enabled by default in Microsoft 365 Apps for enterprise and Office 2016.</span></span> <span data-ttu-id="01bcf-113">تم تسمية خدمات سطح المكتب البعيد (RDS) سابقاً خدمات المحطة الطرفية.</span><span class="sxs-lookup"><span data-stu-id="01bcf-113">Remote Desktop Services (RDS) was previously named Terminal Services.</span></span>
  