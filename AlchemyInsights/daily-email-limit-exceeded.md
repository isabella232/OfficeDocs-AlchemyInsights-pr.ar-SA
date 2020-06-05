---
title: تجاوز حد البريد الإلكتروني اليومي. تم تعليق سير العمل.
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
ms.openlocfilehash: 701c4aef6bfc0c4a2c4570f6dd16dbe4f99efc44
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580320"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>تجاوز حد البريد الإلكتروني اليومي. تم تعليق سير العمل.

قد يتم تلقي هذا الخطأ في السيناريوهات التالية:

- لديك سير عمل في SharePoint Online يستخدم نوع منصة سير عمل SharePoint 2010 أو SharePoint 2013.
- تم تكوين سير العمل لإرسال رسالة بريد إلكتروني مخصصة إلى أكثر من 200 مستخدم في وقت واحد، أو أكثر من 10,000 مستلم يوميًا، أو أكثر من 30 رسالة في الدقيقة.
- عند تشغيل سير العمل، لا يتم إرسال رسالة البريد الإلكتروني، وتلاحظ السلوك التالي:
    - بالنسبة لسير العمل باستخدام نوع النظام الأساسي SharePoint 2013، يمكنك الاستعراض إلى صفحة **حالة سير العمل.** في صفحة حالة سير العمل، يتم تعيين **الحالة الداخلية** إلى **"تم البدء"،** ويعرض بالون المعلومات **غير قادر على الإرسال إلى مستلم**.

لحل هذه المشكلة، قم بتكوين سير العمل لإرسال رسائل البريد الإلكتروني دون تجاوز [حدود المرسل Exchange Online](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits). على سبيل المثال، استخدم إيقافمؤقت في سير العمل، أو إرسال البريد الإلكتروني إلى مجموعة Microsoft 365 أو مجموعة توزيع أو مجموعة أمان ممكّنة للبريد، أو إرسال الرسالة إلى أقل من 200 مستلم في كل مرة.


لمزيد من المعلومات، راجع [المقالة](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or)التالية .

## <a name="related-topics"></a>المواضيع ذات الصلة
- [إنشاء تدفق](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint والتدفق](https://flow.microsoft.com/blog/sharepoint-and-flow/) 