---
title: إصلاح 0x8004de40 خطأ في OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 5da4271f242597b195ef61d553fd4a2ffb313025
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716015"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>إصلاح 0x8004de40 خطأ في OneDrive

إذا تلقيت خطأ 0x8004de40 مع OneDrive:

- إعادة تشغيل الكمبيوتر المتأثر أثناء الاتصال بمجال دليل Acitve.
- إذا لم تعمل إعادة التشغيل على حل المشكلة، فإلغاء الانضمام إلى جهازك وإعادة الانضمام إليه من Azure AD. 

**ملاحظة:** يجب أن تكون على شبكة الشركة أثناء تنفيذ هذه الخطوات. لا تقم بتنفيذ هذه الخطوات عندما لا تتمكن من الاتصال بالبنية التحتية للشركة (على سبيل المثال، أثناء السفر). 

- افتح موجه أمر مرتفع. 
- لفتح مطالبة أمر مرتفعة، انقر فوق - **ابدأ،** انقر بزر الماوس الأيمن **موجه الأوامر،** ثم انقر فوق **تشغيل كمسؤول**.
- نوع *dsregcmd / ترك* واضغط **أدخل**.
- عند الانتهاء، اكتب *dsregcmd / الانضمام* واضغط **أدخل**.
- عند الانتهاء، أغلق موجه الأمر.
- إعادة تشغيل الكمبيوتر، وتسجيل الدخول إلى OneDrive.