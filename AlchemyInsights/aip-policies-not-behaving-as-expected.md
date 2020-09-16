---
title: 'AIP: لا تعمل النهج كما هو متوقع'
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
- "4780"
ms.openlocfilehash: 0dfaae776ec551fe12919e8a8e69f2e7a58d67d0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663176"
---
# <a name="aip-policies-not-behaving-as-expected"></a>AIP: لا تعمل النهج كما هو متوقع

حماية المعلومات في Azure: لا تعمل النهج كما هو متوقع ، راجع ما يلي للإرشادات المستحسنة لمشاكل النهج المختلفة:

1. إذا كنت تواجه مشاكل تتعلق بالعلامات المرئية ، فيرجى المراجعة [عند تطبيق "العلامات المرئية](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied)".
2. إذا كنت تواجه مشاكل في التسمية التلقائية ، فالرجاء مراجعه [كيفيه تكوين الشروط الخاصة بالتصنيف التلقائي والمستحسن لحماية البيانات في Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) [وما تبحث عنه أنواع المعلومات الهامه](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).
3. إذا كنت تواجه مشاكل في حماية الملفات الاصليه/pfile فالرجاء مراجعه [تكوين API للملف](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).
4. تحقق مما إذا كنت تستخدم نهجا في نطاق غير مكون بشكل صحيح: [كيفيه تكوين نهج حماية البيانات في Azure لمستخدمين محددين باستخدام نهج ذات نطاق](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).
5. إذا لم يعمل الوضع "التسمية التلقائية" في Outlook عند إرفاق مستند مسمي ، فتحقق من ان درمينكريبتبروبيرتي غير معرف كما هو موضح هنا: [إعدادات سجل IRM للامان](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).

إذا كنت لا تزال تواجه مشاكل ، يرجى جمع سجلات عميل حماية البيانات في Azure وإرفاق السجلات التي تم تصديرها بهذه البطاقة.

1. افتح مستند Office أو قم بإنشاء رسالة بريد الكتروني جديده في Outlook.
2. انقر **Protect/Sensitivity**فوق  >  **التعليمات الخاصة بالحماية/الحساسية والملاحظات**.
3. انقر فوق **تصدير السجلات**.
4. احفظ السجلات في اختيار الموقع ، وقم بإرفاقها بطلب الخدمة هذا.

موارد إضافية:

- [كيفيه تكوين تسميه لوضع العلامات المرئية لحماية البيانات في Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [مراجعه وثائق حماية البيانات في Azure](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [استخدام تسميات الحساسية في تطبيقات Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

