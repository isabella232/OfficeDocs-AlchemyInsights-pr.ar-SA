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
ms.openlocfilehash: 468d13e59602cf173ed2e17af44c66babfc28703
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506833"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>خطأ أثناء تفعيل Office 2013 على خدمات سطح المكتب البعيد

إذا كنت تتلقى خطأ أثناء تنشيط Office 2013 على عمليات نشر خدمات سطح المكتب البعيد (RDS)، ففكر في تمكين ADAL عن طريق تحرير التسجيل.
  
|**مفتاح التسجيل**|**نوع**|**قيمه**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |Reg_dword  <br/> |1  <br/> |

لمزيد من المعلومات، راجع [تمكين المصادقة الحديثة لـ Office 2013 على أجهزة Windows](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).
  
> [!NOTE]
>  يتم تمكين ADAL بشكل افتراضي في تطبيقات Microsoft 365 للمؤسسات وOffice 2016. تم تسمية خدمات سطح المكتب البعيد (RDS) سابقاً خدمات المحطة الطرفية.
  