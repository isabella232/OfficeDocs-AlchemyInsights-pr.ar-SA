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
ms.openlocfilehash: 6bab821aaa3b50c365ef5d25a61bca195c76d7ce
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/30/2021
ms.locfileid: "51426649"
---
# <a name="getting-a-mailbox-not-found-error-in-outlook-on-the-web"></a>هل لم يتم العثور على رسالة خطأ في علبة البريد في Outlook على الويب؟

إذا كنت تستخدم Outlook على الويب وعثرت على علبة بريد لخطأ، فإن الحساب الذي استخدمته للاتصال ب Outlook على الويب ليس لديه ترخيص Exchange Online، وبالتالي لا توجد علبة بريد مقترنة بهذا الحساب.  يمكن للمسؤول تعيين ترخيص لحسابك باتباع الخطوات التالية:

1. افتح  [مركز إدارة Microsoft 365](https://portal.office.com/adminportal/home#/homepage) واذهب  إلى المستخدمون النشطون ضمن القسم المستخدمون، وحدد المستخدم الذي يرى الخطأ.

2. في صفحة المستخدم التي تفتح،  انتقل إلى المقطع التراخيص  والتطبيقات، وحدد قيمة الموقع المناسبة، ثم عين ترخيصا يحتوي على Exchange Online (قم بتوسيع الترخيص لرؤية تفاصيله). عند الانتهاء، انقر فوق **حفظ التغييرات**.

في بعض الحالات، إذا تم تعيين الترخيص بالفعل إلى حساب مستخدم، فإن إزالة الترخيص ثم إعادة تعيينه يساعد على حل المشكلة وتوفيره بشكل صحيح في النظام: 

- تحقق لمعرفة ما إذا كانت اشتراكاتك في M365 Exchange Online (وغيرها، إذا كان لديك أي اشتراك) حالية ولم تنته صلاحيتها مؤخرا.

بعد التأكد من انتهاء صلاحية اشتراكك وتعيين ترخيص صالح لحساب المستخدم، قد يستغرق توفير الترخيص فترة تصل إلى 24 ساعة، لذا قد تحتاج إلى انتظار حل المشكلة. لمزيد من المعلومات، راجع [تعيين التراخيص وإدارتها](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses).