---
title: الفرق 4c7 خطا
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 0945a341c6456ee4178c0485f3bfb9232fa78a11
ms.sourcegitcommit: 802537a54ef8bde1bdd758ee9a60b6c19d37d6e1
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/19/2019
ms.locfileid: "40795928"
---
# <a name="4c7-error-in-microsoft-teams"></a>خطا 4c7 في فرق Microsoft

يحدث هذا الخطا لان "فرق Microsoft" تتطلب "مصادقه النماذج". عند نشر "خدمات الاتحاد خدمه Active Directory" (AD FS) ، لم يتم تمكين "مصادقه النماذج" لإنترانت بشكل افتراضي. في حاله فشل "المصادقة المتكاملة ل Windows" ، تتم مطالبتك بتسجيل الدخول باستخدام "مصادقه النماذج".

لحل هذه المشكلة ، تمكين "مصادقه النماذج" باستخدام الاداه الاضافيه AD FS التحكم بالاداره ل Microsoft (MMC) علي الكمبيوتر الذي يحتوي علي النسخة المحلية من "Active Directory". لعمل ذلك، اتبع الخطوات التالية: 

1. في جزء التنقل ، استعرض إلى **نهج المصادقة**.
2. ضمن **الإجراءات** الواردة في جزء التفاصيل ، حدد **تحرير المصادقة الاساسيه العمومية**.
3. ضمن علامة التبويب **إنترانت** ، حدد **مصادقه النماذج**.
4. حدد **موافق** (أو **تطبيق**).