---
title: لا تظهر التقارير مركز مسؤولي Microsoft 365 اسم المستخدم القابل للقراءة
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/02/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13809"
- "13810"
- "13812"
- "9008619"
ms.openlocfilehash: ff8eac6487ef544277c5ce2c0c0b7068c9d400ca
ms.sourcegitcommit: b47c6d5e74819b73becaf1dc5eacc72eaf7c1055
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/15/2021
ms.locfileid: "59327801"
---
# <a name="reports-in-microsoft-365-admin-center-do-not-show-readable-username"></a>لا تظهر التقارير مركز مسؤولي Microsoft 365 اسم المستخدم القابل للقراءة

لا تظهر التقارير مركز مسؤولي Microsoft 365 أسماء المستخدمين ولكنها بدلا من ذلك تظهر قيم ألفا رقمية مثل B2BC6C15BB9FCDEA71E5CD302D228CC8.

هذا سلوك متوقع وقد تم الإبلاغ به في مركز الرسائل (MC275344، الذي تم نشره في 3 أغسطس 2021). 

يمكن للمسؤولين العامين إعادة هذا التغيير لمستأجرهم وإظهار معلومات المستخدم التي يمكن التعرف عليها إذا كانت ممارسات الخصوصية الخاصة بهم تسمح بذلك. لإعادة التغيير للمستأجر:

1. في مركز الإدارة، انتقل إلى **الإعدادات** > **إعدادات المؤسسة**  >  [**الخدمات**](https://admin.microsoft.com/Adminportal/Home#/Settings/Services )، وحدد **التقارير**. 
1. ضمن **اختيار كيفية إظهار معلومات المستخدم**، حدد **إظهار معلومات المستخدم القابلة تعريفها في التقارير**، ثم قم بتشغيل التقرير من جديد.