---
title: رمز 0x15
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
description: إذا كنت تتلقى رسالة خطأ أثناء تنشيط Office 2013 على عمليات نشر خدمات سطح المكتب البعيد (RDS)، فنظر في تمكين ADAL من خلال تحرير السجل.
ms.openlocfilehash: ed3770c001461c162ff5bbe24dc400a29380a03b
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/13/2021
ms.locfileid: "58316673"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>خطأ أثناء التنشيط Office 2013 على خدمات سطح المكتب البعيد

إذا كنت تتلقى رسالة خطأ أثناء تنشيط Office 2013 على عمليات نشر خدمات سطح المكتب البعيد (RDS)، فنظر في تمكين ADAL من خلال تحرير السجل.
  
|**مفتاح التسجيل**|**النوع**|**القيمة**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |

لمزيد من المعلومات، راجع تمكين المصادقة [الحديثة Office 2013 على Windows الأجهزة](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).
  
**ملاحظة:** يتم تمكين ADAL بشكل افتراضي في Microsoft 365 Apps for enterprise Office 2016. كانت خدمات سطح المكتب البعيد (RDS) تسمى سابقا خدمات المحطة الطرفية.
  