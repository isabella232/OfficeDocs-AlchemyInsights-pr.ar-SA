---
title: Exchange PowerShell وإهمال المصادقة الأساسية
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "4577"
ms.openlocfilehash: 7b5acf4dd3061c7d9ed23d52a8355865592b9a1d743025fc9300dcda5a18831a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54069231"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a>Exchange PowerShell وإهمال المصادقة الأساسية

للحصول على أحدث المعلومات حول كيفية الاتصال بـ Exchange Online PowerShell بدون استخدام المصادقة الأساسية، [الرجاء الانتقال إلى هنا](https://aka.ms/exops-docs). لا تستخدم الوحدة النمطية PowerShell V2 المصادقة الأساسية.

الرجاء ملاحظة أن تمكين المصادقة الأساسية ما زال مطلوباً على جهاز العميل.
تستخدم الوحدة النمطية الجديدة للإصدار 2 من PowerShell المصادقة الحديثة لإنشاء اتصال لتمكين كل أوامر Cmdlet للإصدار 2 المستندة إلى REST. بالإضافة إلى أوامر Cmdlet للإصدار 2، يتم السماح لك أيضاً بالوصول إلى أوامر Cmdlet لـ "PowerShell عن بُعد" (RPS) القديمة التي تتطلب إنشاء جلسة "PowerShell عن بُعد". يتطلب إنشاء جلسة "PowerShell عن بُعد" (RPS) على جهاز Windows تمكين المصادقة الأساسية للإدارة عن بعد من Windows "WinRM BasicAuth" على جهاز العميل حتى لو كانت الوحدة النمطية تستخدم آلية المصادقة الحديثة "Modern Auth" لمصادقة الخدمة. يُستخدم مسار المصادقة الأساسية لـ "WinRM" لنقل الرموز المميزة للمصادقة الحديثة. إذا تم تعطيل المصادقة الأساسية لـ "WinRM" على جهاز العميل، فإن أوامر cmdlet للإصدار 2 الجديدة ستستمر في العمل (ولكن لن تعمل أوامر cmdlet لـ RPS القديمة).
