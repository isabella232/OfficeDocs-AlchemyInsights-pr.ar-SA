---
title: أخطاء التطبيق
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004342"
- "7841"
ms.openlocfilehash: 2ef90b54ce222a06740e05891fabe87b6565cb14
ms.sourcegitcommit: ba3118b7ad5e02756d0e5c2113245090f54370af
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/25/2021
ms.locfileid: "49984500"
---
# <a name="application-errors"></a>أخطاء التطبيق

هل تبحث عن معلومات حول **رموز أخطاء آدستس** التي يتم إرجاعها من خدمه الرمز المميز للامان ل Azure Active Directory (azure AD) ؟ أقرا [رموز أخطاء التخويل والمصادقة في AZURE AD](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) للعثور علي وصف الخطا آدستس والتصحيحات وبعض الحلول البديلة المقترحة.

يمكن ان تكون أخطاء التخويل نتيجة لعده مشاكل مختلفه ، معظمها تنشئ خطا 401 أو 403. علي سبيل المثال ، يمكن لكل العملاء المتوقعين الوصول إلى أخطاء التخويل:

- [تدفقات الاستحواذ علي رمز الوصول](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) غير صحيحه 
- [نطاقات الأذونات](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes) المكونة بشكل سيئ 
- نقص [الموافقة](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)

لحل أخطاء التخويل الشائعة ، جرب الخطوات المذكورة أدناه الأكثر تطابقا مع الخطا الذي تتلقاه. قد ينطبق أكثر من واحد.

**401 خطا غير مصرح به: هل الرمز المميز صحيح ؟**

تاكد من ان التطبيق الخاص بك يقوم بتقديم رمز مميز صحيح للوصول إلى Microsoft Graph كجزء من الطلب. يعني هذا الخطا غالبا ان الرمز المميز للوصول قد يكون مفقودا في راس طلب مصادقه HTTP أو ان الرمز المميز غير صالح أو منتهي الصلاحية. نوصي بشده باستخدام [مكتبه المصادقة من Microsoft (مسال)](https://docs.microsoft.com/azure/active-directory/develop/msal-overview) للحصول علي الحصول علي رمز الوصول. بالاضافه إلى ذلك ، قد يحدث هذا الخطا إذا حاولت استخدام رمز مميز للوصول مفوض ممنوح لحساب Microsoft شخصي للوصول إلى واجهه برمجه التطبيقات التي تدعم حسابات العمل أو المؤسسة التعليمية فقط (حسابات المؤسسات).

**403 خطا حظر: هل اخترت مجموعه الأذونات المناسبة ؟**

تاكد من انك قمت بطلب مجموعه الأذونات الصحيحة استنادا إلى واجات برمجه تطبيقات Microsoft Graph الخاصة بك. يتم توفير الأذونات الأقل تميزا في كل مواضيع أسلوب مرجع API ل Microsoft Graph. بالاضافه إلى ذلك ، يجب ان يتم منح هذه الأذونات إلى التطبيق من قبل مستخدم أو مسؤول. تحدث الأذونات بشكل طبيعي من خلال صفحه موافقه أو من خلال منح الأذونات باستخدام ريش تسجيل تطبيق Azure Portal. من النصليه **الإعدادات** الخاصة بالتطبيق ، انقر فوق **الأذونات المطلوبة**، ثم انقر فوق **منح الأذونات**.

- [أذونات Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) 
- [فهم أذونات Azure AD والموافقة عليه](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) 

**403 خطا حظر: هل حصل تطبيقك علي رمز مميز لمطابقه الأذونات المختارة ؟**

تاكد من ان نوع الأذونات المطلوبة أو الممنوحة يتطابق مع نوع الرمز المميز للوصول الذي تكتسبه التطبيق. قد تحتاج إلى الطلب ومنح أذونات التطبيق ولكن باستخدام رموز مميزه لتدفق التعليمات البرمجية التفاعلية بدلا من الرموز المميزة لتدفق بيانات اعتماد العميل ، أو طلب الأذونات المفوضة ومنحها ولكن باستخدام الرموز المميزة لتدفق البيانات المفوضة.

- [الحصول علي حق الوصول بالنيابة عن المستخدمين والأذونات المفوضة](https://docs.microsoft.com/graph/auth_v2_user) 
- [التدفق اللغوي لتخويل Azure AD v 2.0-OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [الحصول علي access بدون مستخدم (خدمه البرنامج الخفي) وأذونات التطبيق](https://docs.microsoft.com/graph/auth_v2_service) 
- [تدفق بيانات اعتماد عميل Azure AD v 2.0-OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) 

**403 خطا حظر: أعاده تعيين كلمه المرور**

حاليا ، لا توجد أذونات لخدمه البرنامج الخفي لاذن التطبيق والتي تسمح باعاده تعيين كلمات مرور المستخدمين. يتم دعم واجات برمجه التطبيقات هذه فقط باستخدام تدفقات التعليمات البرمجية التي تم تفويضها بواسطة مسؤول مسجل للدخول.

- [أذونات Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference)

**403 محظور: هل يملك المستخدم حق الوصول وهم مرخصون ؟**

بالنسبة إلى تدفقات التعليمات البرمجية المفوضة ، يقوم Microsoft Graph بتقييم ما إذا كان مسموحا بالطلب استنادا إلى الأذونات الممنوحة للتطبيق والأذونات التي يملكها المستخدم الذي تم تسجيل دخوله. بشكل عام ، يشير هذا الخطا إلى ان المستخدم ليس مميزا بما يكفي لتنفيذ الطلب أو ان المستخدم غير مرخص للبيانات التي يتم الوصول اليها. يمكن فقط للمستخدمين الذين لديهم الأذونات المطلوبة أو التراخيص اجراء الطلب بنجاح.

**403 محظور: هل حددت API للمورد الصحيح ؟**

تقوم خدمات API مثل Microsoft Graph بالتحقق من تطابق المطالبة الaudه (الجماعة المستهدفة) في الرمز المميز للوصول الذي تم تلقيه بالقيمة التي يتوقعها لنفسها ، وإذا لم يكن الأمر كذلك ، سيؤدي ذلك إلى حدوث خطا في 403. الخطا الشائع الذي يتسبب في هذا الخطا هو محاولة استخدام رمز مميز تم الحصول عليه من أجل واجات برمجه تطبيقات Azure AD Graph أو Outlook APIs أو SharePoint/OneDrive للاتصال ب Microsoft Graph (أو العكس). تاكد من ان المورد (أو النطاق) الذي يقوم بالحصول علي رمز مميز يتطابق مع واجهه برمجه التطبيقات (API) التي يقوم التطبيق بالاتصال بها.

**400 طلب غير صالح أو 403 محظور: هل يتوافق المستخدم مع نهج الوصول الشرطي (CA) الخاصة بالمؤسسة الخاصة به ؟**

بالاستناد إلى نهج المراجع المصدقة للمؤسسة ، قد يكون المستخدم الذي يقوم بالوصول إلى موارد Microsoft Graph عبر تطبيقك تشالينجيد للحصول علي معلومات اضافيه غير موجودة في الرمز المميز للوصول الذي حصلت عليه الآن. في هذه الحالة ، يتلقى التطبيق 400 بالخطا *interaction_required* اثناء الحصول علي رمز الوصول المميز أو 403 مع ظهور الخطا *insufficient_claims* عند الاتصال ب Microsoft Graph. في كلتا الحالتين ، تحتوي استجابه الخطا علي معلومات اضافيه يمكن تقديمها إلى نقطه النهاية التخويل لارتياب المستخدم للحصول علي معلومات اضافيه (مثل المصادقة متعددة العوامل أو تسجيل الاجهزه).

- [معالجه تحديات الوصول الشرطي باستخدام مسال ](https://docs.microsoft.com/azure/active-directory/develop/msal-handling-exceptions#conditional-access-and-claims-challenges)
- [إرشادات المطور ل Azure Active directory access الشرطي](https://docs.microsoft.com/azure/active-directory/develop/conditional-access-dev-guide)
