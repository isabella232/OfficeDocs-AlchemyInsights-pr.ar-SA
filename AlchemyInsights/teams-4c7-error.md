---
title: Teams الخطأ 4c7
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: ea3e8f23c07103e604fc6b264047582b9c3e26b6b73237adc30eba574e06cfd3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54049295"
---
# <a name="4c7-error-in-microsoft-teams"></a>خطأ 4c7 في Microsoft Teams

يحدث هذا الخطأ لأن Microsoft Teams يتطلب مصادقة النماذج. عند نشر خدمات اتحاد Active Directory (AD FS)، لا يتم تمكين مصادقة النماذج للانترانت بشكل افتراضي. إذا Windows فشل المصادقة المتكاملة، سيطلب منك تسجيل الدخول باستخدام مصادقة النماذج.

لحل هذه المشكلة، قم بتمكين مصادقة النماذج باستخدام محاذاة وحدة تحكم إدارة AD FS (MMC) على الكمبيوتر الذي لديه النسخة المحلية من Active Directory. لعمل ذلك، اتبع الخطوات التالية: 

1. في جزء التنقل، استعرض بحثا عن **"سياسات المصادقة".**
2. ضمن **إجراءات** في جزء التفاصيل، حدد **تحرير المصادقة الأساسية العالمية**.
3. على علامة **التبويب إنترانت،** حدد **مصادقة النماذج**.
4. حدد **موافق** (أو **تطبيق).**