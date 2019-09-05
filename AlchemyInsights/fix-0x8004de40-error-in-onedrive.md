---
title: إصلاح 0x8004de40 خطأ في أندريف
ms.author: pebaum
author: Techwriter40
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: aa0e0a63ac1e365a7cdce018626740446040a664
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/04/2019
ms.locfileid: "36755835"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>إصلاح 0x8004de40 خطأ في أندريف

إذا تلقيت خطأ 0x8004de40 مع أندريف:

- إعادة تمهيد الكمبيوتر المتأثر أثناء الاتصال بمجال دليل Acitve.
- إذا لم تنجح إعادة التشغيل في حل المشكلة، قم بإلغاء الانضمام إلى جهازك والانضمام إليه من إعلان Azure. 

**ملاحظة:** يجب أن تكون على شبكة الشركة أثناء تنفيذ هذه الخطوات. لا تقم بتنفيذ هذه الخطوات عندما لا تتمكن من الاتصال بالبنية التحتية للشركة (على سبيل المثال، أثناء السفر). 

- افتح موجه أوامر غير مقيد. 
- لفتح موجه أوامر غير مقيد، انقر فوق - **ابدأ**، انقر بزر الماوس الأيمن فوق **موجه الأوامر**، ثم انقر فوق **تشغيل كمسؤول**.
- اكتب *dsregcmd /leave* واضغط **على Enter**.
- عند الاكتمال، اكتب *dsregcmd /join* واضغط **على Enter**.
- عند الاكتمال، أغلق موجه الأوامر.
- إعادة تمهيد الكمبيوتر ثم قم بتسجيل الدخول إلى أندريف.