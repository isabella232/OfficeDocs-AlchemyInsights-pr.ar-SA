---
title: التصنيف التلقائي لا يعمل كما هو متوقع مع عميل AIP
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
- "9002266"
- "4373"
ms.openlocfilehash: d7a2246d78cbd6c4ab40c2a4e5a21807933b619a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47715188"
---
# <a name="automatic-classification-not-behaving-as-expected-with-the-aip-client"></a>التصنيف التلقائي لا يعمل كما هو متوقع مع عميل AIP

التصنيف التلقائي لا يعمل كما هو متوقع ، استخدم الإرشادات المستحسنة التالية:

1. إذا كنت تواجه مشاكل في التسمية التلقائية ، فراجع [كيفيه تكوين الشروط الخاصة بالتصنيف التلقائي والموصي به لحماية البيانات في Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) [وما تبحث عنه أنواع المعلومات الهامه](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).
2. تحقق مما إذا كنت تستخدم نهجا في نطاق غير مكون بشكل صحيح: [كيفيه تكوين نهج حماية البيانات في Azure لمستخدمين محددين باستخدام نهج ذات نطاق](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).
3. إذا لم يعمل الوضع "التسمية التلقائية" في Outlook عند إرفاق مستند مسمي ، فتحقق من `DRMEncryptProperty` عدم تعريفها كما هو موضح هنا: [إعدادات التسجيل في IRM للامان](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).
4. إذا استخدمت [أنواع المعلومات المضمنة](https://support.office.com/article/What-the-sensitive-information-types-look-for-fd505979-76be-4d9f-b459-abef3fc9e86b) لنهج حماية البيانات في Azure ، فتحقق من ان المحتوي يطابق التنسيق المتوقع.
5. تاكد من تكوين التسمية بشكل صحيح **لتلقائية** أو **مستحسنه**. (تتوفر التسمية**التلقائية** لكل تطبيقات microsoft 365 ، وهو الخيار **الموصي به** لكل تطبيقات Microsoft 365 باستثناء Outlook.)
6. لا يمكنك استخدام التصنيف التلقائي للمستندات ورسائل البريد الكتروني التي تم تسميتها مسبقا بشكل يدوي أو تم تسميتها مسبقا باستخدام تصنيف اعلي.  لمزيد من المعلومات ، راجع: [كيفيه تطبيق التسميات التلقائية أو المستحسنة](https://docs.microsoft.com/azure/information-protection/configure-policy-classification#how-automatic-or-recommended-labels-are-applied).
7. إذا كنت لا تزال تواجه مشاكل ، يرجى جمع سجلات عميل حماية البيانات في Azure وإرفاق السجلات التي تم تصديرها بتذكره الدعم. لتصدير سجلات حماية البيانات في Azure:
    - افتح مستند Office أو قم بإنشاء رسالة بريد الكتروني جديده في Outlook.
    - انقر **Protect/Sensitivity**فوق  >  **التعليمات الخاصة بالحماية/الحساسية والملاحظات**.
    - انقر فوق **تصدير السجلات**.
    - احفظ السجلات في اختيار الموقع ، وقم بإرفاقها بطلب الخدمة.

للحصول علي مزيد من المعلومات ، راجع:

- [كيفيه تكوين شروط التصنيف التلقائي والمستحسن لحماية البيانات في Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-classification)
- [إرشادات ارشاديه للسيناريوهات الشائعة التي تستخدم حماية البيانات في Azure](https://docs.microsoft.com/azure/information-protection/how-to-guides)
- [مراجعه وثائق حماية البيانات في Azure](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [مراجعه اشتراكات وميزات حماية البيانات في Azure](https://azure.microsoft.com/pricing/details/information-protection)
- [متطلبات حماية البيانات في Azure](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [البرنامج التعليمي لبدء التشغيل السريع لحماية البيانات في Azure](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)
- [تنزيل عميل حماية المعلومات في Azure](https://www.microsoft.com/download/details.aspx?id=53018)
