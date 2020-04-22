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
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>خطأ أثناء تفعيل Office 2013 على خدمات سطح المكتب البعيد

إذا كنت تتلقى خطأ أثناء تنشيط Office 2013 على عمليات نشر خدمات سطح المكتب البعيد (RDS)، ففكر في تمكين ADAL عن طريق تحرير التسجيل.
  
|**مفتاح التسجيل**|**نوع**|**قيمه**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |Reg_dword  <br/> |1  <br/> |

لمزيد من المعلومات، راجع [تمكين المصادقة الحديثة لـ Office 2013 على أجهزة Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).
  
> [!NOTE]
>  يتم تمكين ADAL بشكل افتراضي في تطبيقات Microsoft 365 للمؤسسات وOffice 2016. تم تسمية خدمات سطح المكتب البعيد (RDS) سابقاً خدمات المحطة الطرفية.
  