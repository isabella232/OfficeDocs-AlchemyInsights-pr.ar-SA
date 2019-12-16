---
title: إصلاح خطا 0x8004de40 في اندريف
ms.author: pebaum
author: pebaum
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 48b29f57763ca22a71a23b2afddcac0e8e8a95db
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/15/2019
ms.locfileid: "40052024"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>إصلاح خطا 0x8004de40 في اندريف

إذا تلقيت خطا 0x8004de40 مع اندريف:

- أعاده تمهيد الكمبيوتر المتاثر اثناء الاتصال بمجال دليل Acitve.
- إذا لم يصلح أعاده التشغيل المشكلة ، قم بإلغاء الانضمام والانضمام إلى جهازك من Azure AD. 

**ملاحظه**: يجب ان تكون علي شبكه الشركة اثناء تنفيذ هذه الخطوات. لا تقم بتنفيذ هذه الخطوات عندما لا تتمكن من الاتصال بالبنية الاساسيه للشركة (علي سبيل المثال ، اثناء السفر). 

- افتح موجه أوامر غير مقيد. 
- لفتح موجه أوامر غير مقيد ، انقر فوق **أبدا**، انقر بزر الماوس الأيمن فوق **موجه الأوامر**، ثم انقر فوق **تشغيل كمسؤول**.
- اكتب *dsregcmd/اترك* واضغط **Enter**.
- عند الاكتمال ، اكتب *dsregcmd/join* واضغط **Enter**.
- عند الاكتمال ، اغلق موجه الأوامر.
- أعاده تمهيد الكمبيوتر ، وتسجيل الدخول إلى OneDrive.