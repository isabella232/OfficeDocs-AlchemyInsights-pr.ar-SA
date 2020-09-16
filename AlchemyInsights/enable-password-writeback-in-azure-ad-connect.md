---
title: تمكين الكتابة الخلفية لكلمه المرور في Azure AD Connect
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002933"
- "5615"
ms.openlocfilehash: 9dbb88492a3906f6780a345cf880327d411dcc66
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709714"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a>تمكين الكتابة الخلفية لكلمه المرور في Azure AD Connect

لتمكين أعاده تعيين كلمه مرور الخدمة الذاتية ، قم أولا بتمكين خيار الكتابة الخلفية في Azure AD Connect. من خادم Azure AD Connect ، أكمل الخطوات التالية:

1. سجل دخولك إلى خادم Azure AD Connect وأبدا بتشغيل معالج تكوين **AZURE Ad connect** .
2. علي صفحه **الترحيب** ، انقر فوق **تكوين**.
3. في الصفحة **المهام الاضافيه** ، حدد **تخصيص خيارات المزامنة**، ثم انقر فوق **التالي**.
4. في صفحه **الاتصال ب AZURE AD** ، ادخل بيانات اعتماد المسؤول العمومي لمستاجر azure الخاص بك ، ثم انقر فوق التالي.
5. في الصفحتين **الاتصال بالدلائل** وتصفيه **المجال/الوحدة التنظيمية** ، انقر فوق **التالي**.
6. في صفحه **الميزات الاختيارية** ، حدد المربع إلى جانب **كتابه كلمه المرور** ، ثم انقر فوق **التالي**.
7. في الصفحة **جاهز للتكوين** ، انقر فوق **تكوين** وانتظر حتى تنتهي العملية.
8. عندما تري تاريخ انتهاء التكوين ، انقر فوق **إنهاء**.

باستخدام الكتابة الخلفية لكلمه المرور الممكنة في Azure AD Connect ، قم الآن بتكوين Azure AD صبر لاجراء الكتابة الخلفية.  لتمكين الكتابة الخلفية لكلمه المرور في صبر ، أكمل الخطوات التالية:

1. سجل دخولك إلى مدخل Azure باستخدام حساب مسؤول عام.
2. ابحث عن **Azure Active directory**وحدده ، وانقر فوق **أعاده تعيين كلمه المرور**، ثم اختر **التكامل المحلي**.
3. تعيين خيار **كتابه كلمات المرور إلى الدليل المحلي ؟** إلى **نعم**.
4. تعيين الخيار الخاص **بتمكين المستخدمين من إلغاء تامين الحسابات من دون أعاده تعيين كلمه المرور الخاصة بهم ؟** إلى **نعم**.
5. عندما تكون جاهزا ، انقر فوق **حفظ**.

لمزيد من المعلومات ، راجع [تمكين أعاده تعيين كلمه مرور الخدمة الذاتية ل Azure active directory إلى بيئة محليه](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).
