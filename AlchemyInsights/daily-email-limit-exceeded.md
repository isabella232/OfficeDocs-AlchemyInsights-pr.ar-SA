---
title: تم تجاوز حد البريد الكتروني اليومي. تم إيقاف سير العمل.
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: dfb42b24f1c2b4b05cb067a82505a6a8b63f277e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47731550"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>تم تجاوز حد البريد الكتروني اليومي. تم إيقاف سير العمل.

قد يتم استلام هذا الخطا في السيناريوهات التالية:

- لديك سير عمل في SharePoint Online يستخدم نوع النظام الأساسي لسير العمل SharePoint 2010 أو SharePoint 2013.
- تم تكوين سير العمل لإرسال رسالة بريد الكتروني مخصصه إلى أكثر من 200 مستخدمين في نفس الوقت ، أو أكثر من 10,000 مستلم في اليوم ، أو أكثر من 30 رسالة في الدقيقة.
- عند تشغيل سير العمل ، لا يتم إرسال رسالة البريد الكتروني ، وتلاحظ السلوك التالي:
    - بالنسبة لسير العمل باستخدام نوع النظام الأساسي ل SharePoint 2013 ، يمكنك الاستعراض وصولا إلى الصفحة " **حاله سير العمل** ". في الصفحة "حاله سير العمل" ، يتم تعيين **الحالة الداخلية** إلى " **تم البدء**" ، ويتم عرض بالون المعلومات **غير قادر علي الإرسال إلى المستلم**.

لحل هذه المشكلة ، قم بتكوين سير العمل لإرسال رسائل البريد الكتروني بدون تجاوز [حدود مرسل Exchange Online](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits). علي سبيل المثال ، يمكنك استخدام إيقاف مؤقت في سير العمل ، أو إرسال البريد الكتروني إلى مجموعه Microsoft 365 ، أو مجموعه توزيع أو مجموعه أمان ممكنة ، أو إرسال الرسالة إلى اقل من 200 مستلم في الوقت نفسه.


لمزيد من المعلومات ، راجع [المقالة](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or)التالية.

## <a name="related-topics"></a>المواضيع ذات الصلة
- [إنشاء تدفق](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint والتدفق](https://flow.microsoft.com/blog/sharepoint-and-flow/) 