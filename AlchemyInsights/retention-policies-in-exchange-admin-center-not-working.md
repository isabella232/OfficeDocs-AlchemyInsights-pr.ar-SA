---
title: لا تعمل سياسات الاستبقاء في مركز إدارة Exchange
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: bb2ce7ce2405be575dfdb79d304fef690e863a4e
ms.sourcegitcommit: e9206b7bb1bf2efd2471edbf4c60c00c3607bc41
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2021
ms.locfileid: "51952215"
---
# <a name="retention-policies-in-exchange-admin-center"></a>سياسات الاستبقاء في مركز إدارة Exchange

إذا كنت تريد منا تشغيل عمليات التحقق التلقائية من الإعدادات المذكورة أدناه، فحدد زر الخلف <-- في أعلى هذه الصفحة، ثم أدخل عنوان البريد الإلكتروني للمستخدم الذي يواجه مشاكل في سياسات الاستبقاء.

إذا كنت تواجه مشاكل مع سياسات الاستبقاء في مركز إدارة Exchange التي لا تنطبق على علب البريد أو العناصر التي لا تنتقل إلى علبة بريد الأرشيف، فتحقق مما يلي:

**الأسباب الجذرية:**

- **لم يعالج "مساعد** المجلد المدار" علبة بريد المستخدم. يحاول مساعد المجلد المدار معالجة كل علبة بريد في مؤسستك المستندة إلى السحابة مرة واحدة كل سبعة أيام.

  **الحل:** تشغيل مساعد المجلد المدار.

- **تم تمكين RetentionHold** **على** علبة البريد. إذا تم وضع علبة البريد على RetentionHold، لن تتم معالجة نهج الاستبقاء على علبة البريد خلال هذه الفترة.

  **الحل:** تحقق من حالة إعداد "احتجاز الاستبقاء" والتحديث حسب الحاجة. للحصول على التفاصيل، راجع [الاستمرار في استبقاء علبة البريد](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
 
**ملاحظة:** إذا كانت علبة البريد أصغر من 10 مبايت، فإن مساعد المجلد المدار لن يقوم تلقائيا لمعالجة علبة البريد.
 
لمزيد من المعلومات حول سياسات الاستبقاء في مركز إدارة Exchange، راجع:

- [علامات الاستبقاء ونهج الاستبقاء](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)

- [تطبيق نهج استبقاء على علب](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) البريد أو [إضافة علامات استبقاء أو إزالتها](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)

- [كيفية تحديد نوع الانتظار الموضوع على علبة بريد](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
