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
ms.openlocfilehash: 6a64e001be115c8e5553a0d8c97b8cb815922c69
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801171"
---
# <a name="sensitivity-labels-not-appearing"></a>لا تظهر تسميات الحساسية

تسمح لك تسميات الحساسية بتصنيف المحتوي الحساس والمساعدة في حمايته. يمكن إنشائها في مركز التوافق ل Microsoft 365 أو مركز الأمان ل microsoft 365 أو Microsoft 365 security & مركز التوافق ضمن تصنيف > الحساسية. لمعرفه المزيد حول هذه الميزة ، راجع [نظره عامه حول تسميات الحساسية](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels).

إذا قمت بتكوين تسميات الحساسية الخاصة بك ولكنها لا تظهر في تطبيقات Microsoft 365 ، فتحقق مما يلي:

- تاكد من انه تم [نشر](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels#what-label-policies-can-do) تسميه الحساسية إلى المستخدمين والمجموعات التي تريدها.

- تاكد من ان المستخدم يستخدم تطبيقا يعتمد تسميات الحساسية-راجع [تسميات الحساسية في المستند](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable).

- إذا كنت تقوم [بترحيل تسميات حماية البيانات في Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels)، فيجب ان تكون علي علم بالاعتبارات المذكورة [هنا](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels).

- دعم منع فقدان البيانات (DLP): يمكن استخدام تسميات الاستبقاء حاليا كشرط في نهج DLP.  لا يتوفر دعم لتسميات الحساسية في نهج DLP حتى الآن ولكننا نعمل علي ذلك.

- عند تمكين التشفير في تسميه الحساسية ، يمكنك الاختيار اما إلى:
    - تعيين الأذونات الآن
    - السماح للمستخدمين بتعيين الأذونات


لمزيد من المعلومات حول المشاكل المحتملة ، راجع [المشاكل المعروفة باستخدام تسميات الحساسية](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).