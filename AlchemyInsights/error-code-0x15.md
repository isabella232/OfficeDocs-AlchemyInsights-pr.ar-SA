---
title: رمز الخطأ 0x15
ms.author: pebaum
author: pebaum
ms.date: 10/31/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: إذا كنت تتلقى خطأ أثناء تنشيط Office 2013 على عمليات نشر خدمات سطح المكتب البعيد (RDS)، خذ بعين الاعتبار تمكين إنبات عن طريق تحرير التسجيل.
ms.openlocfilehash: 4ef2943e5a529368fa2c614e4431cf180924fbb8
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/22/2019
ms.locfileid: "36526955"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a><span data-ttu-id="02c85-103">حدث خطأ أثناء تنشيط Office 2013 على "خدمات سطح المكتب البعيد"</span><span class="sxs-lookup"><span data-stu-id="02c85-103">Error while activation Office 2013 on Remote Desktop Services</span></span>

<span data-ttu-id="02c85-104">إذا كنت تتلقى خطأ أثناء تنشيط Office 2013 على عمليات نشر خدمات سطح المكتب البعيد (RDS)، خذ بعين الاعتبار تمكين إنبات عن طريق تحرير التسجيل.</span><span class="sxs-lookup"><span data-stu-id="02c85-104">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span>
  
|<span data-ttu-id="02c85-105">**مفتاح التسجيل**</span><span class="sxs-lookup"><span data-stu-id="02c85-105">**Registry key**</span></span>|<span data-ttu-id="02c85-106">**نوع**</span><span class="sxs-lookup"><span data-stu-id="02c85-106">**Type**</span></span>|<span data-ttu-id="02c85-107">**القيمة**</span><span class="sxs-lookup"><span data-stu-id="02c85-107">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="02c85-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="02c85-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="02c85-109">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="02c85-109">REG_DWORD</span></span>  <br/> |<span data-ttu-id="02c85-110">1</span><span class="sxs-lookup"><span data-stu-id="02c85-110">1</span></span>  <br/> |

<span data-ttu-id="02c85-111">لمزيد من المعلومات، راجع [تمكين مصادقة الحديثة ل 2013 Office على أجهزة Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="02c85-111">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="02c85-112">يتم تمكين إنبات افتراضياً في Office 365 ProPlus ومكتب عام 2016.</span><span class="sxs-lookup"><span data-stu-id="02c85-112">ADAL is enabled by default in Office 365 ProPlus and Office 2016.</span></span> <span data-ttu-id="02c85-113">تم مسبقاً يسمى خدمات سطح المكتب البعيد (RDS) "الخدمات الطرفية".</span><span class="sxs-lookup"><span data-stu-id="02c85-113">Remote Desktop Services (RDS) was previously named Terminal Services.</span></span>
  