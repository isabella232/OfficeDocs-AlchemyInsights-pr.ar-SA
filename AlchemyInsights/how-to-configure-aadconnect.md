---
title: 646 كيفية تكوين AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 713cda26e55f07f0438cb9ebe5aa9da86c4ebb3a
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43722508"
---
# <a name="configure-sync-features"></a>تكوين ميزات المزامنة

يتضمن Azure AD Connect العديد من الميزات التي يتم تمكينها بشكل افتراضي، أو التي يمكنك تمكينها لاحقًا. تتطلب بعض الميزات تكوينًا إضافيًا في بيئات معينة.

- [تصفية](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) حدود تتم مزامنة الكائنات إلى Azure AD. بشكل افتراضي، تتم مزامنة كافة المستخدمين وجهات الاتصال والمجموعات وحسابات الكمبيوتر Windows 10. يمكنك تضمين الكائنات أو استبعادها استنادًا إلى المجالات أو OUs أو السمات الأخرى.

- [مزامنة تجزئة كلمة المرور](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) مزامنة تجزئة كلمة المرور من الدليل النشط الداخلي إلى Azure AD. يسمح هذا بإدارة كلمة المرور في موقع واحد، ولكن استخدام نفس كلمة المرور في كل من البيئات الداخلية والسحابية. لأن "الدليل النشط" هو المصدر الموثوق به، يمكنك استخدام نُهج كلمة المرور الخاصة بك.

- تسمح [إعادة تعيين كلمة مرور الخدمة الذاتية (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) للمستخدمين بإعادة تعيين كلمات المرور الخاصة بهم في السحابة أثناء تطبيق نهج كلمة المرور الداخلي الخاص بك.

- يسمح [رد كتابة الجهاز](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) بكتابة الأجهزة المسجلة في Azure AD مرة أخرى إلى الدليل النشط الداخلي بحيث يمكن استخدامها للوصول المشروط.

- منع [حذف عرضي](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) يتم تمكين بشكل افتراضي للمساعدة في منع حذف الكائنات في وقت واحد كثيرة جداً (أكثر من 500 كائن لكل مزامنة). يمكنك تغيير هذا الإعداد لتلبية احتياجات مؤسستك.

- يتم تمكين [الترقية التلقائية](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) بشكل افتراضي للتثبيتات السريعة وتساعد على ضمان تحديث إصدار Azure AD Connect دائمًا.
