---
title: عدم التعامل مع التصنيف التلقائي كما هو متوقع مع عميل AIP
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4373"
ms.openlocfilehash: 93d15b8b65fd52a567ecbb6e1f84363bf2b38946c105896b0b5ef41e49d16ea9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53979696"
---
# <a name="automatic-classification-not-behaving-as-expected-with-the-aip-client"></a>عدم التعامل مع التصنيف التلقائي كما هو متوقع مع عميل AIP

لا يتم تنفيذ التصنيف التلقائي كما هو متوقع، استخدم الإرشادات الموصى بها التالية:

1. إذا كنت تواجه مشاكل في التسمية التلقائية، فاطلع على كيفية تكوين الشروط للتصنيف التلقائي والموصى به ل [Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) وما هي أنواع المعلومات الحساسة التي [تبحث عن](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).
2. تحقق مما إذا كنت تستخدم نهج النطاق التي لم يتم تكوينها بشكل صحيح: كيفية تكوين نهج [Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-scope)لمستخدمين محددين باستخدام النهج ذات النطاق .
3. إذا لم تعمل التسمية التلقائية Outlook عند إرفاق مستند باسم، فتحقق من عدم تعريفه كما هو موضح هنا: إعدادات تسجيل `DRMEncryptProperty` [IRM](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options)الخاصة ب الأمان .
4. إذا استخدمت أنواع [المعلومات المضمنة](https://support.office.com/article/What-the-sensitive-information-types-look-for-fd505979-76be-4d9f-b459-abef3fc9e86b) لن نهج حماية معلومات Azure، فتحقق من أن المحتوى يتطابق مع التنسيق المتوقع.
5. تحقق من تكوين التسمية بشكل مناسب ل **Automatic** أو **Recommended**. (**تتوفر** التسمية التلقائية لجميع تطبيقات Microsoft 365، في حين تتوفر الموصى بها لجميع تطبيقات Microsoft 365 باستثناء تطبيقات Outlook.) 
6. لا يمكنك استخدام التصنيف التلقائي للمستندات ورسائل البريد الإلكتروني التي تم تسميتها يدويا مسبقا أو التي تم تسميتها مسبقا ب تصنيف أعلى.  لمزيد من المعلومات، راجع: كيفية تطبيق التسميات التلقائية [أو الموصى بها](https://docs.microsoft.com/azure/information-protection/configure-policy-classification#how-automatic-or-recommended-labels-are-applied).
7. إذا كنت لا تزال تواجه مشاكل، فيرجى تجميع سجلات عميل Azure Information Protection وإرفاق السجلات التي تم تصديرها بتذكرة الدعم. لتصدير سجلات Azure Information Protection:
    - افتح مستندا Office أو أنشئ بريدا إلكترونيا جديدا في Outlook.
    - انقر **فوق حماية/حساسية**  >  **تعليمات وملاحظات**.
    - انقر **فوق تصدير السجلات.**
    - احفظ السجلات إلى اختيارك للموقع، وأرفقها بطلب الخدمة.

لمزيد من المعلومات، راجع:

- [كيفية تكوين الشروط للتصنيف التلقائي والموصى به لحماية معلومات Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-classification)
- [أدلة إرشادية للسيناريوهات الشائعة التي تستخدم Azure Information Protection](https://docs.microsoft.com/azure/information-protection/how-to-guides)
- [مراجعة وثائق Azure Information Protection](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [مراجعة ميزات واشتراكات Azure Information Protection](https://azure.microsoft.com/pricing/details/information-protection)
- [متطلبات حماية معلومات Azure](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [برنامج تعليمي للبدء السريع لحماية معلومات Azure](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)
- [تنزيل عميل Azure Information Protection](https://www.microsoft.com/download/details.aspx?id=53018)
