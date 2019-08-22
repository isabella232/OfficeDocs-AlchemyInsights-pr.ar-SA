---
title: تم تجاوز حد البريد الإلكتروني يوميا. يتم تعطيل سير العمل.
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 7/25/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: e3fbcd5bfc279847cfb39140c3689f5433b61509
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/22/2019
ms.locfileid: "36514427"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>تجاوز حد البريد الإلكتروني يوميا. يتم تعطيل سير العمل.

وقد تلقي هذا الخطأ في السيناريوهات التالية:

- يكون سير عمل في SharePoint على الإنترنت الذي يستخدم SharePoint 2010 أو نوع النظام الأساسي لسير العمل SharePoint 2013.
- تم تكوين سير العمل لإرسال رسالة بريد إلكتروني مخصصة للمستخدمين أكثر من 200 في مرة الواحدة أو المستلمين أكثر من 10 آلاف يوميا أكثر من 30 رسالة في الدقيقة.
- عندما تقوم بتشغيل سير العمل، لم يتم إرسال رسالة البريد الإلكتروني، ولاحظت السلوك التالي:
    - لسير عمل باستخدام نوع النظام الأساسي SharePoint 2013، يمكنك استعراض الصفحة " **حالة سير العمل** ". في الصفحة "حالة سير العمل"، يتم تعيين **الحالة الداخلية** **الشروع في العمل**، ويعرض بالون معلومات **قادر على إرسال إلى مستلم**.

للتغلب على هذه المشكلة، قم بتكوين سير العمل الخاص بك لإرسال رسائل البريد الإلكتروني دون تجاوز [حدود المرسل Exchange عبر إنترنت](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits). على سبيل المثال، استخدم مؤقتاً في سير العمل إرسال البريد الإلكتروني إلى مجموعة Office 365، مجموعة توزيع أو مجموعة أمان تمكين البريد أو إرسال الرسالة إلى المستلمين أقل من 200 في نفس وقت.


لمزيد من المعلومات، راجع [المقالة](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or)التالية.

## <a name="related-topics"></a>المواضيع ذات الصلة
- [إنشاء تدفق](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint والتدفق](https://flow.microsoft.com/blog/sharepoint-and-flow/) 