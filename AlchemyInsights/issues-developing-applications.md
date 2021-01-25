---
title: المشاكل المتعلقة بتطوير التطبيقات
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7754"
- "9004342"
ms.openlocfilehash: 652fd6431201380e8e96619f63ecac15a6704d4f
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974158"
---
# <a name="issues-developing-applications"></a>المشاكل المتعلقة بتطوير التطبيقات

لاستكشاف المشاكل الأكثر شيوعا عند إنشاء تطبيقات Azure Active directory (AD) ، راجع المقالات التالية:

- [اري صعوبة في تسجيل الدخول إلى التطبيق (التطبيقات) باستخدام مستعرض Chrome فقط](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications) 
- [لا اعرف كيفيه تغيير الإعدادات الافتراضية لمده بقاء الرمز المميز للتطبيق](https://docs.microsoft.com/azure/active-directory/develop/registration-config-change-token-lifetime-how-to) 
- [لا تخلط عن كيفيه عمل الموافقة علي التطبيق](https://docs.microsoft.com/azure/active-directory/application-dev-consent-framework) 
- [لا اعرف كيفيه منح الأذونات إلى التطبيق الخاص بي](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent) 
- [لا أدرك الفرق بين أذونات التطبيق والمفوض](https://docs.microsoft.com/azure/active-directory/develop/delegated-and-app-perms)

***نهاية دعم مكتبه المصادقة ل Azure active directory (ADAL) و AZURE AD GRAPH API (رسم بياني AAD)** _

- بدءا من 30 يونيو 2020 ، فلن نضيف اي ميزات جديده إلى مكتبه مصادقه Azure Active directory (ADAL) و Azure AD Graph API (رسم بياني ل AAD). سنستمر في توفير الدعم التقني وتحديثات الأمان ولكنه لن يوفر تحديثات الميزات بعد الآن.

- بدءا من 30 يونيو 2022 ، سنقوم بإنهاء الدعم ل ADAL و AAD الرسم البياني ولن يوفر الدعم التقني أو تحديثات الأمان. نتيجة لهذا الشرط ، ما يلي:

    - ستستمر التطبيقات التي تستخدم ADAL في إصدارات نظام التشغيل الموجودة في العمل بعد هذه المرة ولكن لن تحصل علي اي دعم تقني أو تحديثات أمان.

    - قد لا تتلقي التطبيقات التي تستخدم الرسم البياني AAD بعد هذه الفترة الاستجابات من نقطه نهاية الرسم البياني في AAD

_ *الترحيل ADAL**

إذا كنت تستخدم تطبيقات Microsoft ، فنوصي بالتحديث إلى مكتبه مصادقه Microsoft (مسال) ، التي تتضمن أحدث الميزات وتحديثات الأمان. هذه التوصية في سياق Microsoft لبدء عمليه ترحيل تطبيقاته إلى مسال بواسطة الموعد النهائي لنهاية الدعم. 

تضمن الترحيل بواسطة Microsoft من تطبيقاته مسال التطبيقات مزايا الأمان وتحسينات الميزات التي مسالها.

1. [قراءه الاسئله المتداولة حول ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
2. [تعرف علي كيفيه ترحيل التطبيقات علي أساس لكل نظام أساسي](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
3. إذا كنت بحاجه إلى مساعده في فهم اي من تطبيقاتك تستخدم ADAL ، فنحن ننصحك بمراجعه كل التعليمات البرمجية المصدر لتطبيقاتك ، ويمكنك الوصول إلى اي من بائعي البرامج المستقلين (إيسفس) أو موفري التطبيقات. يمكن ان يوفر لك دعم Microsoft أيضا قائمه بكل تطبيقات ADAL التابعة ل Microsoft في نطاق المستاجر الخاص بك.

**ترحيل الرسم البياني AAD**

بالنسبة إلى التطبيقات التي تستخدم الرسم البياني AAD ، اتبع الإرشادات الخاصة بنا لترحيل تطبيقات الرسم البياني AAD إلى Microsoft Graph:

1. [توفر قائمه الاختيار الخاصة بالترحيل نقطه بدء](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
2. يعرض مدخل تسجيلك في Azure app التطبيقات التي تستخدم الرسم البياني AAD. نوصي بمراجعه كل التعليمات البرمجية المصدر لتطبيقاتك ، ويمكنك الوصول إلى اي بائعين مستقلين (إيسفس) أو موفري التطبيقات ، إذا كان ذلك ممكنا. يمكن ان يوفر لك دعم Microsoft أيضا معلومات حول استخدام الرسم البياني AAD في نطاق المستاجر الخاص بك.







