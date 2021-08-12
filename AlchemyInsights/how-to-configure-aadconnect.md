---
title: 646 كيفية تكوين AADConnect
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
ms.openlocfilehash: c5fa5fd7586f999698fe43554fb9a2b205be3e25740c20763254a38d41297e0c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53963630"
---
# <a name="configure-sync-features"></a>تكوين ميزات المزامنة

يتضمن الاتصال Azure AD العديد من الميزات التي يتم تمكينها بشكل افتراضي، أو التي يمكنك تمكينها لاحقا. تتطلب بعض الميزات تكوينا إضافيا في بيئات معينة.

- [تمت مزامنة](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) حدود التصفية مع Azure AD. بشكل افتراضي، يتم مزامنة جميع المستخدمين وجهات الاتصال والمجموعات Windows 10 الكمبيوتر. يمكنك تضمين كائنات استنادا إلى المجالات أو OUs أو سمات أخرى أو استبعادها.

- [تعمل مزامنة كلمة المرور على](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) مزامنة كلمة المرور من Active Directory المحلية إلى Azure AD. يسمح ذلك بإدارة كلمة المرور في موقع واحد، ولكن استخدام كلمة المرور نفسها في كل من البيئات المحلية والبيئات السحابية. نظرا لأن Active Directory هو المصدر الموثوق، يمكنك استخدام سياسات كلمات المرور الخاصة بك.

- تسمح إعادة تعيين كلمة المرور للخدمة الذاتية [(SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) للمستخدمين بإعادة تعيين كلمات المرور الخاصة بهم في السحابة مع تطبيق نهج كلمة المرور المحلي.

- [تتيح كتابة الجهاز](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) إعادة كتابة الأجهزة المسجلة في Azure AD إلى Active Directory في الموقع بحيث يمكن استخدامها للوصول الشرطي.

- [يتم تمكين منع عمليات](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) الحذف العرضية بشكل افتراضي للمساعدة على منع عدد كبير جدا من عمليات حذف العناصر في الوقت نفسه (أكثر من 500 كائن في كل مزامنة). يمكنك تغيير هذا الإعداد لتلبية احتياجات مؤسستك.

- [يتم تمكين](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) الترقية التلقائية بشكل افتراضي في عمليات التثبيت السريع وتساعد على ضمان أن إصدار Azure AD الاتصال دائما.
