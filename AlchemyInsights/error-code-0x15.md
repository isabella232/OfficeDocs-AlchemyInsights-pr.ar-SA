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
ms.openlocfilehash: e2249d8ebbd2313c64dda5656a3243fa76d97a9a
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/28/2019
ms.locfileid: "35388232"
---
إذا كنت تتلقى خطأ أثناء تنشيط Office 2013 على عمليات نشر خدمات سطح المكتب البعيد (RDS)، خذ بعين الاعتبار تمكين إنبات عن طريق تحرير التسجيل.
  
|**مفتاح التسجيل**|**نوع**|**القيمة**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |

لمزيد من المعلومات، راجع [تمكين مصادقة الحديثة ل 2013 Office على أجهزة Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).
  
> [!NOTE]
>  يتم تمكين إنبات افتراضياً في Office 365 ProPlus ومكتب عام 2016. تم مسبقاً يسمى > خدمات سطح المكتب البعيد (RDS) "الخدمات الطرفية".
  