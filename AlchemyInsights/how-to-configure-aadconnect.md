---
title: 646 كيفيه تكوين AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 6327e42b74283d732247c9a847c68db72082c56a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47704476"
---
# <a name="configure-sync-features"></a>تكوين ميزات المزامنة

يتضمن Azure AD Connect العديد من الميزات التي يتم تمكينها بشكل افتراضي ، أو يمكنك تمكينها لاحقا. تتطلب بعض الميزات تكوين إضافي في بيئات معينه.

- حدود [التصفية](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) يتم مزامنة العناصر إلى Azure AD. بشكل افتراضي ، تتم مزامنة كل المستخدمين وجات الاتصال والمجموعات وحسابات الكمبيوتر في Windows 10. يمكنك تضمين كائنات أو استبعادها استنادا إلى المجالات أو الأووس أو السمات الأخرى.

- يقوم " [مزامنة" تجزئه كلمه المرور](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) بمزامنة تجزئه كلمه المرور من active directory المحلي إلى Azure AD. يسمح هذا باداره كلمه المرور في موقع واحد ، ولكن استخدام نفس كلمه المرور في كل من البيئات المحلية والسحابية. لان Active Directory هو المصدر الموثوق ، يمكنك استخدام نهج كلمه المرور الخاصة بك.

- تسمح [أعاده تعيين كلمه مرور الخدمة الذاتية (سبر)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) للمستخدمين باعاده تعيين كلمات المرور الخاصة بهم في السحابة مع استمرار تطبيق نهج كلمه المرور المحلية.

- يسمح [الكتابة الخلفية للجهاز](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) باعاده كتابه الاجهزه المسجلة في Azure AD إلى active directory المحلي بحيث يمكن استخدامها للوصول الشرطي.

- [منع الحذف العرضي](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) يتم تمكينه بشكل افتراضي للمساعدة علي منع العديد من عمليات حذف الكائنات المتزامنة (أكثر من 500 كائن لكل مزامنة). يمكنك تغيير هذا الاعداد لتلبيه احتياجات مؤسستك.

- يتم تمكين [الترقية التلقائية](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) بشكل افتراضي لتثبيتات express والمساعدة علي التاكد من ان إصدار Azure AD Connect حاليا دائما.
