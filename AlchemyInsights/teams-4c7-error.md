---
title: خطا في الفرق 4 c7
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 08494b461a24eba8999a5edb99c89af7b17db9b3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700190"
---
# <a name="4c7-error-in-microsoft-teams"></a>خطا 4c7 في فرق Microsoft

يحدث هذا الخطا لان فرق Microsoft تتطلب مصادقه النماذج. عند نشر خدمات الأمان المشترك ل Active directory (AD FS) ، لا يتم تمكين مصادقه النماذج لإنترانت بشكل افتراضي. إذا فشلت عمليه المصادقة المتكاملة في Windows ، ستتم مطالبتك بتسجيل الدخول باستخدام مصادقه النماذج.

لحل هذه المشكلة ، قم بتمكين مصادقه النماذج باستخدام الاداه الاضافيه AD FS Console (MMC) علي الكمبيوتر الذي يحتوي علي النسخة المحلية من Active directory. لعمل ذلك، اتبع الخطوات التالية: 

1. في جزء التنقل ، استعرض بحثا عن **نهج المصادقة**.
2. ضمن **الإجراءات** في جزء التفاصيل ، حدد **تحرير المصادقة الاساسيه العامة**.
3. علي علامة التبويب **إنترانت** ، حدد **مصادقه النماذج**.
4. حدد **موافق** (أو **تطبيق**).