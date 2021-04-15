---
title: خطأ في Teams 4c7
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
ms.openlocfilehash: 51f2aa936e803b63bcbdf73b89959cd3a1757751
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51786656"
---
# <a name="4c7-error-in-microsoft-teams"></a>خطأ 4c7 في Microsoft Teams

يحدث هذا الخطأ لأن Microsoft Teams يتطلب مصادقة النماذج. عند نشر خدمات اتحاد Active Directory (AD FS)، لا يتم تمكين مصادقة النماذج للانترانت بشكل افتراضي. إذا فشلت المصادقة المتكاملة ل Windows، فيطلب منك تسجيل الدخول باستخدام مصادقة النماذج.

لحل هذه المشكلة، قم بتمكين مصادقة النماذج باستخدام محاذاة وحدة تحكم إدارة AD FS (MMC) على الكمبيوتر الذي لديه النسخة المحلية من Active Directory. لعمل ذلك، اتبع الخطوات التالية: 

1. في جزء التنقل، استعرض بحثا عن **"سياسات المصادقة".**
2. ضمن **إجراءات** في جزء التفاصيل، حدد **تحرير المصادقة الأساسية العالمية**.
3. على علامة **التبويب إنترانت،** حدد **مصادقة النماذج**.
4. حدد **موافق** (أو **تطبيق).**