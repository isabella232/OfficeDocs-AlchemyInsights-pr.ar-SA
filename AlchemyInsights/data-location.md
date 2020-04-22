---
title: موقع البيانات
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "945"
- "5300023"
ms.assetid: 3bab036c-dbaa-406a-8b73-1e5f31993436
ms.openlocfilehash: c769c17796d805f88afb4d5b32adb7d4a9bb3ce0
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/21/2020
ms.locfileid: "43655269"
---
# <a name="data-location"></a>موقع البيانات

يمكنك عرض موقع المستأجر الخاص بك في مركز المشرف أو عن طريق الاتصال بExchange Online عبر PowerShell.


**مركز المشرف:**
1. تسجيل الدخول إلى [مركز المشرف](https://admin.microsoft.com/Adminportal/Home).
2. حدد**ملف تعريف مؤسسة** **الإعدادات** > .
3. ضمن **موقع البيانات،** حدد **عرض التفاصيل**.


**Powershell:**
1. الاتصال بالتبادل عبر الإنترنت باستخدام Windows PowerShell.
2. تنفيذ [cmdlet الحصول على التنظيمية](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit) لعرض قائمة خصائص المستأجر الخاص بك. 
3. انظر إلى خاصية OrganizationId.

عندما يكون لديك موقع البيانات لEXO و SPO، يمكنك تحديد موقع البيانات للخدمات الأخرى التي قد تستخدمها من [حيث توجد البيانات الخاصة بك](https://products.office.com/where-is-your-data-located).