---
title: AADSTS50011 خطا تسجيل الدخول إلى OneDrive
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003820"
- "6840"
ms.openlocfilehash: 1f906f82e99c322ed953800d54fba5a073eacd10
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 11/09/2020
ms.locfileid: "48982416"
---
# <a name="onedrive-login-error-aadsts50011"></a>AADSTS50011 خطا تسجيل الدخول إلى OneDrive

إذا تلقيت رسالة الخطا "AADSTS50011: لا يتطابق عنوان URL المحدد في الطلب مع الرد" عند تسجيل الدخول إلى تطبيق OneDrive ، تحقق مما يلي:

يجب ان يكون إصدار OneDrive الخاص بك مساويا للإصدار 20.052 أو أكبر منه. XXXX. للتحقق من الإصدار الذي قمت به ، انقر فوق أيقونه OneDrive الزرقاء في منطقه الاعلام ، حدد **تعليمات & إعدادات > الإعدادات > حول**.

قد تحظر الشبكة نقل البيانات إلى **g.live.com** و **oneclient.sfx.ms**. إذا تم حظر نقل البيانات ، فلن يتمكن OneDrive من تحديث نفسه. استخدام مسؤول الشبكة لضمان امكانيه الوصول إلى عناوين Url هذه. يجب ان تكون [نقاط النهاية هذه](https://docs.microsoft.com/microsoft-365/enterprise/urls-and-ip-address-ranges?view=o365-worldwide) يمكن الوصول اليها للعملاء الذين يستخدمون خطط Microsoft 365.

إذا كنت بحاجه إلى الحصول علي إصدار حالي من OneDrive يدويا ، فقم بزيارة [https://aka.ms/getonedrive](https://aka.ms/getonedrive) .
