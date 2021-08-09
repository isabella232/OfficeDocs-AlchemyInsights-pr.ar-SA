---
title: 'AIP: لا يتم تنفيذ النهج كما هو متوقع'
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
- "4780"
ms.openlocfilehash: 90448bf57297ce59ba222efd1927b5de588bfbfdb1206b6403764d7f43fed690
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53934280"
---
# <a name="aip-policies-not-behaving-as-expected"></a>AIP: لا يتم تنفيذ النهج كما هو متوقع

حماية معلومات Azure: لا يتم تنفيذ النهج كما هو متوقع، راجع الإرشادات الموصى بها لقضايا النهج المختلفة:

1. إذا كنت تواجه مشاكل في العلامات المرئية، فالرجاء مراجعة [عند تطبيق العلامات المرئية](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).
2. إذا كنت تواجه مشاكل في التسمية التلقائية، فالرجاء مراجعة كيفية تكوين الشروط للتصنيف التلقائي والموصى به ل [Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) وما هي أنواع المعلومات الحساسة التي [تبحث عن](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).
3. إذا كنت تواجه مشاكل في الحماية الأصلية/Pfile، فيرجى مراجعة [تكوين API للملفات](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).
4. تحقق مما إذا كنت تستخدم نهج النطاق التي لم يتم تكوينها بشكل صحيح: كيفية تكوين نهج [Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-scope)لمستخدمين محددين باستخدام النهج ذات النطاق .
5. إذا لم تعمل التسمية التلقائية Outlook عند إرفاق مستند باسم، فتحقق من عدم تعريف DRMEncryptProperty كما هو موضح هنا: إعدادات تسجيل [IRM](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options)الخاصة ب الأمان .

إذا كنت لا تزال تواجه مشاكل، فالرجاء تجميع سجلات عميل Azure Information Protection وإرفاق السجلات المصدرة بهذه التذكرة.

1. افتح مستندا Office أو أنشئ بريدا إلكترونيا جديدا في Outlook.
2. انقر **فوق حماية/حساسية**  >  **تعليمات وملاحظات**.
3. انقر **فوق تصدير السجلات.**
4. احفظ السجلات إلى اختيارك للموقع، وأرفقها بطلب الخدمة هذا.

موارد إضافية:

- [كيفية تكوين تسمية العلامات المرئية ل Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [مراجعة وثائق Azure Information Protection](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [استخدام تسميات الحساسية في تطبيقات Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

