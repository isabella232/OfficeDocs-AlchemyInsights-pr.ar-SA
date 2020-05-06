---
title: Exchange PowerShell وإهمال المصادقة الأساسية
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "4577"
ms.openlocfilehash: 24d59860732b42e8d62da8c1a8c37f2018a0d126
ms.sourcegitcommit: 264b782ac2fba8ffd84524180dc4f7d60b45e9a4
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/04/2020
ms.locfileid: "44015676"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a>Exchange PowerShell وإهمال المصادقة الأساسية

للحصول على أحدث المعلومات حول كيفية الاتصال بـ Exchange Online PowerShell بدون استخدام المصادقة الأساسية، [الرجاء الانتقال إلى هنا](https://aka.ms/psbasicauth).

الرجاء ملاحظة أن تمكين المصادقة الأساسية ما زال مطلوباً على جهاز العميل.
تستخدم الوحدة النمطية الجديدة للإصدار 2 من PowerShell المصادقة الحديثة لإنشاء اتصال لتمكين كل أوامر Cmdlet للإصدار 2 المستندة إلى REST. بالإضافة إلى أوامر Cmdlet للإصدار 2، يتم السماح لك أيضاً بالوصول إلى أوامر Cmdlet لـ "PowerShell عن بُعد" (RPS) القديمة التي تتطلب إنشاء جلسة "PowerShell عن بُعد". يتطلب إنشاء جلسة "PowerShell عن بُعد" (RPS) على جهاز Windows تمكين المصادقة الأساسية للإدارة عن بعد من Windows "WinRM BasicAuth" على جهاز العميل حتى لو كانت الوحدة النمطية تستخدم آلية المصادقة الحديثة "Modern Auth" لمصادقة الخدمة. يُستخدم مسار المصادقة الأساسية لـ "WinRM" لنقل الرموز المميزة للمصادقة الحديثة. إذا تم تعطيل المصادقة الأساسية لـ "WinRM" على جهاز العميل، فإن أوامر cmdlet للإصدار 2 الجديدة ستستمر في العمل (ولكن لن تعمل أوامر cmdlet لـ RPS القديمة).
