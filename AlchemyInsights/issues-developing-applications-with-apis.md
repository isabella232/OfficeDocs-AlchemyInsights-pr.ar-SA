---
title: مشاكل تطوير التطبيقات باستخدام واجات برمجه التطبيقات
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
- "9004343"
- "7755"
ms.openlocfilehash: 26d732819b64efa4fb84da44cc2a279368aa28b0
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974205"
---
# <a name="issues-developing-applications-with-apis"></a>مشاكل تطوير التطبيقات باستخدام واجات برمجه التطبيقات

للبدء باستخدام واجهه برمجه التطبيق الخاصة ب Azure Active Directory ، راجع [دليل AZURE Ad GRAPH api تشغيل](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) ، أو اعرض [الوثائق التبادلية التفاعلية ل azure ad graph](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog).

**نهاية دعم مكتبه المصادقة ل Azure Active directory (ADAL) و Azure AD Graph API (رسم البياني AAD)**

**يبدا يوم 30 يونيو ، 2020**، لن نضيف اي ميزات جديده إلى الرسم البياني ADAL و Azure AD. سنستمر في توفير الدعم التقني وتحديثات الأمان ولكنه لن يوفر تحديثات الميزات بعد الآن.

**بدءا من 30 يونيو 2022**، سنقوم بإنهاء الدعم ل ADAL والرسم البياني ل Azure AD ولن يعود بحاجه إلى توفير الدعم التقني أو تحديثات الأمان.

ستستمر التطبيقات التي تستخدم ADAL في إصدارات نظام التشغيل الموجودة في العمل بعد هذه المرة ولكن لن تحصل علي اي دعم تقني أو تحديثات أمان.

قد لا تتلقي التطبيقات التي تستخدم الرسم البياني Azure AD بعد هذه الفترة الاستجابات من نقطه نهاية الرسم البيانية في Azure AD.

**الترحيل ADAL**

نوصي بالتحديث إلى [مكتبه مصادقه Microsoft (مسال)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview)، التي تحتوي علي أحدث الميزات وتحديثات الأمان.

إذا كنت تستخدم تطبيقات Microsoft ، فتعرف ان Microsoft يجري عمليه ترحيل تطبيقاته إلى مسال بواسطة الموعد النهائي لنهاية الدعم ، مما يضمن توفرها من الأمان وتحسينات الميزات المسالة.

1. [أقرا الاسئله المتداولة حول ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).
1. [تعرف علي كيفيه ترحيل التطبيقات علي أساس كل نظام أساسي](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).
1. إذا كنت بحاجه إلى مساعده في التعرف علي التعليمات البرمجية الخاصة بالتطبيقات التي تستخدمها ADAL ، فمن المستحسن مراجعه جميع برامج المصدر الخاصة بكل تطبيق ، والوصول إلى اي إيسفس أو موفري تطبيقات. يمكن ان يوفر لك دعم Microsoft أيضا قائمه بكل تطبيقات ADAL التابعة ل Microsoft في نطاق المستاجر الخاص بك.

**ترحيل الرسم البياني AAD**

بالنسبة إلى التطبيقات التي تستخدم الرسم البياني Azure AD ، اتبع الإرشادات الخاصة بنا لترحيل [تطبيقات الرسومات البيانية في AZURE ad إلى Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true).

1. [توفر قائمه الاختيار الخاصة بالترحيل نقطه بدء](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
1. يعرض مدخل تسجيلك في Azure app التطبيقات التي تستخدم الرسم البياني AAD. نوصي بمراجعه كل التعليمات البرمجية المصدر لتطبيقاتك ، وإذا كان ذلك ممكنا ، فيمكنك الوصول إلى اي إيسفس أو موفري التطبيق. يمكن ان يوفر لك دعم Microsoft أيضا قائمه بكل استخدامات الرسم البياني ل AAD في المستاجر.
1. بالنسبة إلى التطبيق للوصول إلى البيانات في Microsoft Graph ، يجب ان يمنح المستخدم أو المسؤول الأذونات الصحيحة عبر عمليه الموافقة. يسرد [مرجع أذونات Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) الأذونات المقترنة بكل مجموعه رئيسيه من واجات برمجه تطبيقات microsoft graph. يوفر أيضا إرشادات حول كيفيه استخدام الأذونات.
