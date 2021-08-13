---
title: مزامنة كلمة المرور
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "8619"
ms.openlocfilehash: 3cdde086e535d2397b4d1a8a66903121a5217015ca055fb9f8d025b0842f044b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53960822"
---
# <a name="password-synchronization"></a>مزامنة كلمة المرور

**لا تعمل مزامنة كلمة المرور على الإطلاق**

بعض المشاكل الشائعة التي يواجهها العملاء عندما لا تعمل مزامنة كلمة المرور هي:

- لا يتم منح حساب Active Directory الذي يستخدمه Azure AD الاتصال للتواصل  مع Active Directory في الموقع نسخ متماثل لتغييرات الدليل ونسخه نسخا متماثلاتغيير كل الأذونات المطلوبة لمزامنة كلمة المرور - يجب إصلاح ذلك من خلال منح هذه الأذونات لحساب Active **Directory.**
- يتم تعطيل مزامنة كلمة المرور بعد أن قام المسؤول بتغيير  أسلوب المستخدم Sign-In من مزامنة كلمة المرور إلى خيار آخر مثل "الاتحاد مع **AD FS"** في معالج Azure AD الاتصال - يمكنك إصلاح ذلك من خلال إعادة تمكين ميزة مزامنة كلمة المرور في معالج Azure AD الاتصال. 
- مشكلة في الاتصال مع Active Directory في الموقع. على سبيل المثال، لا يمكن الوصول إلى بعض وحدات التحكم بالمجال بواسطة Azure AD الاتصال، أو يتم حظر المنافذ المطلوبة بواسطة جدار الحماية - يجب إصلاح ذلك من خلال التأكد من أن الاتصال بين خادم Azure AD الاتصال و Active Directory في الموقع يعمل بشكل صحيح. [](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports)
- خادم Azure AD الاتصال موجود حاليا في وضع الترحيل، مما يؤدي إلى عدم تمكن الخادم من الوصول إلى هاشتات كلمة المرور - لا استكشاف المشكلة وإصلاحها، اتبع الخطوات الموضحة في القسم استكشاف الأخطاء في مزامنة كلمة المرور وإصلاحها مع مزامنة [Azure AD الاتصال -](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)لا تتم مزامنة كلمات المرور .

**لا تعمل مزامنة كلمة المرور مع بعض المستخدمين**

1. إذا لاحظت عدم مزامنة كلمة المرور لمستخدم، فاستخدم مهمة استكشاف الأخطاء وإصلاحها في Azure AD الاتصال للتحقق من المشكلة وحلها.  تنفيذ المهام التالية:

    a. [تشغيل مهمة استكشاف الأخطاء وإصلاحها في المعالج](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-objectsync)

    b. [استخدام الأمر cmdlet الخاص بابتكار الأخطاء وإصلاحها للتحقق من مشكلة مزامنة كلمة المرور لاستخدام معين](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)

2. يتم تمكين كائن مستخدم Active Directory في الموقع حيث يجب على المستخدم تغيير كلمة المرور **في خيار تسجيل** الدخول التالي. عند تمكين هذا الخيار، يتم تعيين كلمة مرور مؤقتة للمستخدم وستطلب منه تغيير كلمة المرور في تسجيل الدخول التالي. لا يقوم Azure AD الاتصال مزامنة كلمات المرور المؤقتة إلى Azure AD.

لحل المشكلة أعلاه، تنفيذ أي من المهام التالية:

- اطلب من المستخدم تسجيل الدخول إلى التطبيق المحلي (على سبيل المثال، Windows سطح المكتب) وتغيير كلمة المرور. سيتم مزامنة كلمة المرور الجديدة إلى Azure AD.
- يجب أن يقوم مسؤول بتحديث كلمة مرور المستخدم دون تمكين الخيار يجب على المستخدم تغيير كلمة المرور عند تسجيل الدخول التالي ، ومشاركة كلمة المرور الجديدة مع المستخدم.

3. لم يتم تكوين كائن مستخدم Active  Directory في الموقع بشكل صحيح لمزامنة الكائن أو مزامنة كلمة المرور. لا استكشاف هذه المشكلة وإصلاحها، اتبع الخطوات الموضحة في مزامنة مزامنة كلمة المرور مع [مزامنة Azure AD الاتصال وإصلاحها.](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)







