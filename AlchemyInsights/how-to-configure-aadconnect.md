---
title: 646 كيفية تكوين آدكونيكت
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 316d7253494c55a9bc94797d493897c2ddec516c
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/22/2019
ms.locfileid: "36541572"
---
# <a name="configure-sync-features"></a>تكوين ميزات مزامنة

يتضمن الاتصال الإعلان azure العديد من الميزات التي يتم تمكينها بشكل افتراضي، أو يمكنك تمكين لاحقاً. تتطلب بعض ميزات تكوين إضافية في بيئات محددة.

- تتم مزامنة حدود [تصفية](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) الكائنات لإعلان Azure. بشكل افتراضي، كافة المستخدمين، جهات اتصال، مجموعات، و Windows 10 حسابات كمبيوتر تتم مزامنة. يمكنك تضمين أو استبعاد الكائنات التي تستند إلى مجالات أو وحدات تنظيمية أو السمات الأخرى.

- مزامنة [المزامنة تجزئة كلمة مرور](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) كلمة مرور التجزئة من "Active Directory" الداخلي لإعلان Azure. يسمح هذا إدارة كلمة المرور في موقع واحد، لكن باستخدام نفس كلمة المرور في كل من المحلي وبيئات مجموعة النظراء. نظراً لأن "خدمة active Directory" مصدر موثوق به، يمكنك استخدام نهج كلمة المرور الخاصة بك.

- [إعادة تعيين كلمة المرور الخدمة الذاتية (صبر)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) يسمح للمستخدمين بإعادة تعيين كلمات المرور الخاصة بهم في مجموعة النظراء أثناء استمرار تطبيق نهج كلمة المرور المحلية الخاصة بك.

- يسمح [الجهاز إعادة الكتابة](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) الأجهزة المسجلة في AD Azure إعادة كتابته في خدمة "active Directory" الداخلي حيث يمكن استخدامها للوصول المشروط.

- يتم تمكين [العرضي منع الحذف](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) بشكل افتراضي لمنع حذف الكائنات المتزامنة كثيرة جداً (أكثر من 500 الكائنات كل المزامنة). يمكنك تغيير هذا الإعداد لتلبية احتياجات المؤسسة الخاصة بك.

- تمكين [الترقية التلقائية](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) افتراضياً للتثبيتات السريعة ويضمن دائماً الإصدار الخاص بك من الاتصال Azure الإعلان الحالي.
