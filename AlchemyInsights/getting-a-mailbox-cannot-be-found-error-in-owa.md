---
title: 126 هل يتعذر العثور على خطأ في الحصول على علبة بريد في OWA؟
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "126"
- "1600020"
ms.assetid: e85bffec-e5ad-418a-8561-dab6257e1864
ms.openlocfilehash: aca0371dad9ba43fa21b0df8e50f1b8ee536528af90d6bda401995c6e5796be4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54056477"
---
# <a name="getting-a-mailbox-not-found-error-in-outlook-on-the-web"></a>هل لم يتم العثور على رسالة خطأ في علبة البريد Outlook على ويب؟

إذا كنت تستخدم Outlook على ويب ولم تتمكن من  العثور على علبة بريد للخطأ، فإن الحساب الذي استخدمته للاتصال ب Outlook على ويب ليس لديه ترخيص Exchange Online، وبالتالي لا توجد علبة بريد مقترنة بهذا الحساب. يمكن للمسؤول تعيين ترخيص لحسابك باتباع الخطوات التالية:

1. افتح [مركز مسؤولي Microsoft 365](https://portal.office.com/adminportal/home#/homepage) واذهب **إلى** المستخدمون  النشطون ضمن المقطع المستخدمون، وحدد المستخدم الذي يرى الخطأ.

2. في صفحة المستخدم التي يتم فتحها، انتقل إلى المقطع  التراخيص والتطبيقات، وحدد قيمة الموقع المناسبة، ثم عين ترخيصا يحتوي على Exchange Online (قم بتوسيع الترخيص لرؤية تفاصيله).  عند الانتهاء، انقر فوق **حفظ التغييرات**.

في بعض الحالات، إذا تم تعيين الترخيص بالفعل إلى حساب مستخدم، فإن إزالة الترخيص ثم إعادة تعيينه يساعد على حل المشكلة وتوفيره بشكل صحيح في النظام: 

- تحقق لمعرفة ما إذا كانت اشتراكات M365 Exchange Online اشتراكات M365 (وغيرها، إذا كان لديك أي اشتراك) حالية ولم تنته صلاحيتها مؤخرا.

بعد التأكد من انتهاء صلاحية اشتراكك وتعيين ترخيص صالح لحساب المستخدم، قد يستغرق توفير الترخيص فترة تصل إلى 24 ساعة، لذا قد تحتاج إلى انتظار حل المشكلة. لمزيد من المعلومات، راجع [تعيين التراخيص وإدارتها](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses).