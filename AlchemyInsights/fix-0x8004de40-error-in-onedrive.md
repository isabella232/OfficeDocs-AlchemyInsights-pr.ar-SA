---
title: إصلاح خطا 0x8004de40 في OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: b9bd6dff48f78063e3d47f5fe2f834f59eb9868a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47745117"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>إصلاح خطا 0x8004de40 في OneDrive

إذا تلقيت رسالة الخطا 0x8004de40 في OneDrive:

- أعد تشغيل الكمبيوتر المتاثر اثناء الاتصال بمجال دليل أسيتفي.
- إذا لم يؤد أعاده التشغيل إلى حل المشكلة ، فقم بأونجوين الجهاز وأعاده الانضمام اليه من Azure AD. 

**ملاحظه**: يجب ان تكون علي شبكه الشركة لديك اثناء تنفيذ هذه الخطوات. لا تقم بتنفيذ هذه الخطوات إذا لم تتمكن من الاتصال بالبنية الاساسيه لشركك (علي سبيل المثال ، اثناء السفر). 

- افتح موجه أوامر غير مقيد. 
- لفتح موجه أوامر غير مقيد ، انقر فوق- **بدء**، وانقر بزر الماوس الأيمن فوق **موجه الأوامر**، ثم انقر فوق **تشغيل كمسؤول**.
- اكتب *دسريجكمد/leave خروج* واضغط علي مفتاح **الإدخال Enter**.
- عند الانتهاء ، اكتب *دسريجكمد/join* واضغط علي مفتاح **الإدخال Enter**.
- عند الانتهاء ، اغلق موجه الأوامر.
- أعد تشغيل الكمبيوتر ، ثم سجل دخولك إلى OneDrive.