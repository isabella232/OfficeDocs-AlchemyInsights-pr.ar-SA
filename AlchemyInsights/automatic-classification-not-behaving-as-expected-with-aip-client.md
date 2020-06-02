---
title: التصنيف التلقائي لا يتصرف كما هو متوقع مع عميل AIP
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
- "4373"
ms.openlocfilehash: 95a994d6a49ee8737a6ebcb196314f92776d8482
ms.sourcegitcommit: 2afad0b107d03cd8c4de0b85b5bee38a13a7960d
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/26/2020
ms.locfileid: "44492891"
---
# <a name="automatic-classification-not-behaving-as-expected-with-the-aip-client"></a>التصنيف التلقائي لا يتصرف كما هو متوقع مع عميل AIP

التصنيف التلقائي لا يتصرف كما هو متوقع، استخدم الإرشادات الموصى بها التالية:

1. إذا كنت تواجه مشكلات في وضع العلامات التلقائي، فراجع [كيفية تكوين شروط التصنيف التلقائي والموصى به لحماية معلومات Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) وما تبحث عنه أنواع المعلومات [الحساسة](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).
2. تحقق مما إذا كنت تستخدم نُهج ًا ذات نطاق لم يتم تكوينها بشكل صحيح: [كيفية تكوين نهج حماية المعلومات Azure لمستخدمين محددين باستخدام نُهج ذات نطاق](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).
3. إذا لم يكن وضع العلامات التلقائي ة يعمل مع Outlook عند إرفاق مستند مسمى، فتحقق من عدم `DRMEncryptProperty` تعريفه كما هو موضح هنا: إعدادات التسجيل [IRM للأمان](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).
4. إذا كنت تستخدم [أنواع المعلومات المضمنة](https://support.office.com/article/What-the-sensitive-information-types-look-for-fd505979-76be-4d9f-b459-abef3fc9e86b) لسياسة حماية معلومات Azure، فتحقق من تطابق المحتوى مع التنسيق المتوقع.
5. تحقق من تكوين التسمية بشكل مناسب **للتلقائي** أو **الموصى به**. (تتوفر وضع العلامات**التلقائية** لجميع تطبيقات Office، في حين يتوفر **الموصى به** لجميع تطبيقات Office باستثناء Outlook.)
6. لا يمكنك استخدام التصنيف التلقائي للمستندات ورسائل البريد الإلكتروني التي تم تصنيفها يدويًا مسبقًا أو تم تصنيفها تلقائيًا مسبقًا بتصنيف أعلى.  لمزيد من المعلومات، [راجع: كيفية تطبيق التسميات التلقائية أو الموصى بها](https://docs.microsoft.com/azure/information-protection/configure-policy-classification#how-automatic-or-recommended-labels-are-applied).
7. إذا كنت لا تزال تواجه مشكلات، يرجى جمع سجلات عملاء حماية المعلومات Azure وإرفاق السجلات المصدرة بتذكرة الدعم الخاصة بك. لتصدير سجلات حماية المعلومات Azure:
    - افتح مستند Office أو أنشئ بريدًا إلكترونيًا جديدًا في Outlook.
    - انقر فوق **حماية / تعليمات الحساسية**  >  **والملاحظات.**
    - انقر فوق **سجلات التصدير**.
    - احفظ السجلات على اختيارك للموقع، وإرفاقها بطلب الخدمة الخاص بك.

لمزيد من المعلومات، راجع:

- [كيفية تكوين شروط التصنيف التلقائي والموصى به لحماية المعلومات Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-classification)
- [أدلة إرشادية للسيناريوهات الشائعة التي تستخدم حماية معلومات Azure](https://docs.microsoft.com/azure/information-protection/how-to-guides)
- [مراجعة وثائق حماية المعلومات Azure](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [مراجعة اشتراكات وميزات حماية المعلومات في Azure](https://azure.microsoft.com/pricing/details/information-protection)
- [متطلبات حماية المعلومات اللازوردية](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [بدء سريع تعليمي لحماية المعلومات أزور](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)
- [تحميل عميل حماية المعلومات Azure](https://www.microsoft.com/download/details.aspx?id=53018)
