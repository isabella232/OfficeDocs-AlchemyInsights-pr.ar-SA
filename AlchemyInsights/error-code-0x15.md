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
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>خطا اثناء تنشيط Office 2013 علي خدمات سطح المكتب البعيد

إذا كنت تتلقي رسالة خطا اثناء تنشيط Office 2013 علي عمليات نشر خدمات سطح المكتب البعيد (RDS) ، فيمكنك تمكين ADAL عن طريق تحرير السجل.
  
|**مفتاح التسجيل**|**اكتب**|**Value**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER \Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |

لمزيد من المعلومات ، راجع [تمكين المصادقة الحديثة ل Office 2013 علي أجهزه Windows](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).
  
> [!NOTE]
>  يتم تمكين ADAL بشكل افتراضي في تطبيقات Microsoft 365 ل enterprise و Office 2016. تمت تسميه خدمات سطح المكتب البعيد (RDS) مسبقا بالخدمات الطرفية.
  