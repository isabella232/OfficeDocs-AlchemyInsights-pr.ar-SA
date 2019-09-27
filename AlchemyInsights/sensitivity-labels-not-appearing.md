---
title: تسميات الحساسية لا تظهر
ms.author: stephow
author: stephow-MSFT
manager: laurawi
ms.date: ''
ms.audience: admin
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1778"
- "9000181"
ms.openlocfilehash: 4bf8e02246c966f22648467386a7862f0521fecf
ms.sourcegitcommit: 71978e2bb779b5955fd113f84512b83321b26912
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/26/2019
ms.locfileid: "37207212"
---
# <a name="sensitivity-labels-not-appearing"></a>تسميات الحساسية لا تظهر

تسمح لك تسميات الحساسية بتصنيف المحتوي الحساس والمساعدة علي حمايته. يمكن إنشاؤها في مركز التوافق Microsoft 365 أو مركز أمان Microsoft 365 أو Office 365 الأمان & مركز التوافق ضمن تصنيف > الحساسية التسميات. لمعرفه المزيد حول هذه الميزة ، راجع [نظره عامه علي تسميات الحساسية](https://docs.microsoft.com/office365/securitycompliance/sensitivity-labels).

إذا قمت بتكوين تسميات الحساسية الخاصة بك ولكنها لا تظهر في تطبيقات Office ، فتحقق مما يلي:

- تاكد من ان تسميه الحساسية قد تم [نشرها](https://docs.microsoft.com/Office365/SecurityCompliance/sensitivity-labels#what-label-policies-can-do) إلى المستخدمين والمجموعات التي تريدها.

- تاكد من ان المستخدم يستخدم تطبيقا يدعم تسميات الحساسية-راجع [تسميات الحساسية في المستند](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?ad=US&ui=en-US&rs=en-US#bkmk_whereavailable).

- إذا كنت تقوم [بترحيل تسميات حماية معلومات Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels)، يجب ان تكون علي علم بالاعتبارات المسرودة [هنا](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels).

- دعم منع فقدان البيانات (DLP): حاليا ، يمكن استخدام تسميات الاستبقاء فقط كشرط في نهج DLP.  دعم التسميات حساسية في سياسة DLP غير متوفرة حتى الآن ولكن نحن نعمل علي ذلك.

- عند تمكين التشفير علي تسميه تحسسيه ، يمكنك اختيار اما:
    - تعيين الأذونات الآن
    - السماح للمستخدمين بتعيين أذونات


لمزيد من المعلومات حول المشكلات المحتملة ، راجع [المشكلات المعروفة مع تسميات الحساسية](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).