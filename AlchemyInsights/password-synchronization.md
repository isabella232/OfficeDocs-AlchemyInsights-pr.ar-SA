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
ms.openlocfilehash: 601649f6e5212ca03df5fcc32cd1d02c133e9170
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/04/2021
ms.locfileid: "50480859"
---
# <a name="password-synchronization"></a>مزامنة كلمة المرور

**لا تعمل مزامنة كلمة المرور المتزامنة على الإطلاق**

بعض المشاكل الشائعة التي يواجهها العملاء عند عدم عمل مزامنة كلمة المرور المتزامنة هي:

- لا يتم منح حساب Active Directory الذي يستخدمه Azure AD Connect  للتواصل مع Active  Directory في الموقع "تغييرات دليل النسخ المتماثل" و"نسخ الدليل المتماثل" يغير كل الأذونات المطلوبة لمزامنة كلمة المرور - يجب إصلاح ذلك من خلال منح هذه الأذونات لحساب Active Directory.
- يتم تعطيل مزامنة كلمة المرور بعد أن يقوم المسؤول بتغيير  أسلوب المستخدم Sign-In من "مزامنة كلمة المرور" إلى خيار آخر مثل "الاتحاد مع **AD FS"** في معالج Azure AD Connect - يمكنك إصلاح ذلك من خلال إعادة تمكين ميزة مزامنة كلمة المرور في معالج Azure AD Connect. 
- مشكلة في الاتصال مع Active Directory في الموقع. على سبيل المثال، يتعذر على Azure AD Connect [](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) الوصول إلى بعض وحدات التحكم بالمجال، أو يتم حظر المنافذ المطلوبة بواسطة جدار الحماية - يجب إصلاح ذلك من خلال ضمان عمل الاتصال بين خادم Azure AD Connect و Active Directory في الموقع بشكل صحيح.
- خادم Azure AD Connect موجود حاليا في وضع الترحيل، مما يؤدي إلى عدم تمكن الخادم من الوصول إلى تقسمات كلمة المرور - لاتباع الخطوات الموضحة في مزامنة كلمة المرور في القسم وإصلاحها مع مزامنة [Azure AD Connect -](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)لا تتم مزامنة أي كلمات مرور.

**لا تعمل مزامنة كلمة المرور المتزامنة مع بعض المستخدمين**

1. إذا لاحظت عدم مزامنة كلمة المرور للمستخدم، فاستخدم  مهمة استكشاف الأخطاء وإصلاحها في Azure AD Connect للتحقق من المشكلة وحلها. تنفيذ المهام التالية:

    أ. [تشغيل مهمة استكشاف الأخطاء وإصلاحها في المعالج](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-objectsync)

    ب. [استخدام الأمر cmdlet الخاص بابتكار الأخطاء وإصلاحها للتحقق من مشكلة مزامنة كلمة المرور لاستخدام معين](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)

2. يتم تمكين كائن مستخدم Active Directory في الموقع، حيث يجب على المستخدم تغيير كلمة المرور **في خيار تسجيل** الدخول التالي. عند تمكين هذا الخيار، يتم تعيين كلمة مرور مؤقتة للمستخدم وستطالب بتغيير كلمة المرور في تسجيل الدخول التالي. لا يقوم Azure AD Connect بمزامنة كلمات المرور المؤقتة إلى Azure AD.

لحل المشكلة أعلاه، تنفيذ أي من المهام التالية:

- اطلب من المستخدم تسجيل الدخول إلى التطبيق المحلي (على سبيل المثال، سطح مكتب Windows) وتغيير كلمة المرور. سيتم مزامنة كلمة المرور الجديدة إلى Azure AD.
- يجب أن يقوم مسؤول بتحديث كلمة مرور المستخدم دون تمكين الخيار الذي يجب على المستخدم تغيير كلمة المرور عند تسجيل الدخول التالي، ومشاركة كلمة المرور الجديدة مع المستخدم.

3. لم يتم تكوين كائن مستخدم Active  Directory في الموقع بشكل صحيح لمزامنة الكائنات أو مزامنة كلمة المرور. استكشاف هذه المشكلة وإصلاحها، اتبع الخطوات الموضحة في مزامنة كلمة المرور المتزامنة مع مزامنة [Azure AD Connect وإصلاحها.](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)







