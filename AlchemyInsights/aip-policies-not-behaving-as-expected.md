---
title: 'AIP: السياسات لا تتصرف كما هو متوقع'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4780"
ms.openlocfilehash: 91308850c06485bdd11e81bd130770aefb247118
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580752"
---
# <a name="aip-policies-not-behaving-as-expected"></a>AIP: السياسات لا تتصرف كما هو متوقع

حماية المعلومات Azure: السياسات لا تتصرف كما هو متوقع، راجع ما يلي للإرشادات الموصى بها لمختلف مشكلات السياسة:

1. إذا كنت تواجه مشكلات في العلامات البصرية، يرجى مراجعة [عند تطبيق العلامات المرئية.](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied)
2. إذا كنت تواجه مشكلات في وضع العلامات التلقائية، يرجى مراجعة [كيفية تكوين شروط التصنيف التلقائي والموصى به لحماية معلومات Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) وما تبحث عنه أنواع المعلومات [الحساسة](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).
3. إذا كنت تواجه مشاكل مع حماية الأصلي / Pfile، يرجى مراجعة [تكوين واجهة برمجة التطبيقات ملف](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).
4. تحقق مما إذا كنت تستخدم نُهج ًا ذات نطاق لم يتم تكوينها بشكل صحيح: [كيفية تكوين نهج حماية المعلومات Azure لمستخدمين محددين باستخدام نُهج ذات نطاق](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).
5. إذا لم يعمل وضع العلامات التلقائي ة مع Outlook عند إرفاق مستند مسمى، فتحقق من عدم تعريف DRMEncryptProperty كما هو موضح هنا: [إعدادات التسجيل IRM للأمان](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).

إذا كنت لا تزال تواجه مشكلات، يرجى جمع سجلات عملاء حماية المعلومات Azure وإرفاق السجلات المصدرة بهذه التذكرة.

1. افتح مستند Office أو أنشئ بريدًا إلكترونيًا جديدًا في Outlook.
2. انقر فوق **حماية / تعليمات الحساسية**  >  **والملاحظات.**
3. انقر فوق **سجلات التصدير**.
4. احفظ السجلات على اختيارك للموقع، وإرفاقها بطلب الخدمة هذا.

موارد إضافية:

- [كيفية تكوين تسمية للعلامات المرئية لحماية معلومات Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [مراجعة وثائق حماية المعلومات Azure](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [استخدام تسميات الحساسية في تطبيقات Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

