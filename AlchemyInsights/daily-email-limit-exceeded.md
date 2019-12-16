---
title: تم تجاوز حد البريد الكتروني اليومي. تم تعليق سير العمل.
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: 3cad5d8305da0a5db9a85888793350a062e6aed6
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/15/2019
ms.locfileid: "40053104"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>تجاوز حد البريد الكتروني اليومي. تم تعليق سير العمل.

قد يتم تلقي هذا الخطا في السيناريوهات التالية:

- لديك سير عمل في SharePoint علي الإنترنت التي تستخدم SharePoint 2010 أو SharePoint 2013 نوع النظام الأساسي سير العمل.
- يتم تكوين سير العمل لإرسال رسالة بريد الكتروني مخصصه إلى أكثر من 200 المستخدمين في كل مره ، أكثر من 10,000 المستلمين في اليوم الواحد ، أو أكثر من 30 رسالة في الدقيقة الواحدة.
- عند تشغيل سير العمل ، لا يتم إرسال رسالة البريد الكتروني ، ولاحظت السلوك التالي:
    - بالنسبة لسير العمل باستخدام نوع النظام الأساسي ل SharePoint 2013 ، يمكنك الاستعراض إلى صفحه **حاله سير العمل** . في الصفحة "حاله سير العمل" ، يتم تعيين **الحالة الداخلية** إلى **البدء**، ويعرض بالون المعلومات **غير قادر علي إرسال إلى مستلم**.

كمحاولة للتغلب علي هذه المشكلة قم بتكوين سير العمل الخاص بك لإرسال رسائل البريد الكتروني دون تجاوز [حدود المرسل Exchange عبر إنترنت](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits). علي سبيل المثال ، استخدم وقفه في سير العمل ، إرسال البريد الكتروني إلى مجموعه 365 Office أو مجموعه توزيع أو البريد تمكين مجموعه الأمان أو إرسال الرسالة إلى اقل من 200 المستلمين في كل مره.


لمزيد من المعلومات ، راجع [المقالة](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or)التالية.

## <a name="related-topics"></a>المواضيع ذات الصلة
- [إنشاء تدفق](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint والتدفق](https://flow.microsoft.com/blog/sharepoint-and-flow/) 