---
title: تم تجاوز حد البريد الإلكتروني اليومي. تم إيقاف سير العمل مؤقتا.
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
ms.openlocfilehash: 60ddbe68298e998a4e0b271a15209efc135c80638702c98dbcb3e0b2f1554860
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53914638"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>تم تجاوز حد البريد الإلكتروني اليومي. تم إيقاف سير العمل مؤقتا.

قد يتم تلقي هذا الخطأ في السيناريوهات التالية:

- لديك سير عمل في SharePoint Online يستخدم نوع النظام الأساسي SharePoint 2010 أو SharePoint 2013.
- تم تكوين سير العمل لإرسال رسالة بريد إلكتروني مخصصة إلى أكثر من 200 مستخدم في كل مرة، أو أكثر من 10000 مستلم في اليوم، أو أكثر من 30 رسالة في الدقيقة.
- عند تشغيل سير العمل، لا يتم إرسال رسالة البريد الإلكتروني، وتلاحظ السلوك التالي:
    - بالنسبة إلى سير عمل يستخدم نوع النظام الأساسي SharePoint 2013، يمكنك الاستعراض إلى صفحة **حالة سير** العمل. في الصفحة حالة سير العمل، **يتم** تعيين الحالة الداخلية إلى تم البدء **،** ويعرض بالون المعلومات تعذر إرساله **إلى المستلم.**

لل حل هذه المشكلة، قم بتكوين سير العمل لإرسال رسائل البريد الإلكتروني دون تجاوز Exchange Online [المرسلين.](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits) على سبيل المثال، استخدم إيقافا مؤقتا في سير العمل، أو أرسل البريد الإلكتروني إلى مجموعة Microsoft 365 أو مجموعة توزيع أو مجموعة أمان تم تمكين البريد لها، أو أرسل الرسالة إلى أقل من 200 مستلم في كل مرة.


لمزيد من المعلومات، راجع المقالة [التالية](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).

## <a name="related-topics"></a>المواضيع ذات الصلة
- [إنشاء Flow](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 