---
title: لا تظهر تسميات الحساسية
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1778"
- "9000181"
ms.openlocfilehash: 824824257fee4aaaab1f2dd32597b4cdc858d035fabd357af90cf054dd35c9c4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54061419"
---
# <a name="sensitivity-labels-not-appearing"></a>لا تظهر تسميات الحساسية

تسمح لك تسميات الحساسية بتصنيف المحتوى الحساس ومساعدته على حمايته. يمكن إنشاؤها في مركز التوافق في Microsoft 365 أو Microsoft 365 الأمان أو Microsoft 365 مركز التوافق & ضمن تصنيف > الحساسية. لمعرفة المزيد حول هذه الميزة، راجع [نظرة عامة حول تسميات الحساسية](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels).

إذا قمت بتكوين تسميات الحساسية ولكنك لا تظهر في تطبيقات Microsoft 365، فتحقق مما يلي:

- تأكد من نشر تسمية [](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels#what-label-policies-can-do) الحساسية للمستخدمين والمجموعات التي تريدها.

- تأكد من أن المستخدم يستخدم تطبيقا يدعم تسميات الحساسية - راجع [تسميات](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable)الحساسية في المستند .

- إذا كنت تقوم [بتهجر تسميات Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels)، فتنبه إلى الاعتبارات المذكورة [هنا](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels).

- دعم منع فقدان البيانات (DLP): حاليا، يمكن استخدام تسميات الاستبقاء فقط كشرط في سياسات DLP.  لا يتوفر الدعم لتسميات الحساسية في نهج DLP بعد ولكننا نعمل على ذلك.

- عند تمكين التشفير على تسمية حساسية، يمكنك اختيار ما يلي:
    - تعيين الأذونات الآن
    - السماح للمستخدمين بتعيين الأذونات


لمزيد من المعلومات حول المشاكل المحتملة، راجع [المشاكل المعروفة مع تسميات الحساسية](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).