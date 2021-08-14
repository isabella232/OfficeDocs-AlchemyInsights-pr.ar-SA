---
title: سجل جهاز مكرر في المدخل
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4386"
ms.openlocfilehash: 7eb642f85f437fe216c49ce6b060c9061b477629fbd45f50ca0ef315b8cd32d3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54004141"
---
# <a name="duplicate-device-record-in-the-portal"></a>سجل جهاز مكرر في المدخل

يمكنك رؤية سجلين للجهاز في المدخل، إذا لم يقم الجهاز بالإبلاغ عن حالة الإدارة المشتركة بشكل صحيح في موقع إدارة التكوين. للتحقق من حالة الإدارة المشتركة للجهاز، راجع عمود **الإدارة المشتركة** للجهاز في وحدة تحكم إدارة التكوين. إذا لم يكن العمود مرئياً، فيمكنك إضافته بالنقر بزر الماوس الأيمن فوق أي من رؤوس الأعمدة، وتحديده من القائمة.

القيمة المُدارة بشكل مشترك يجب أن تكون **نعم**. إذا كانت القيمة هي **لا**، فافتح التطبيق الصغير لعميل إدارة التكوين على جهاز العميل وتحقق من خاصية **الإدارة المشتركة** في علامة التبويب "عام".

- إذا كانت القيمة هي **ممكَّن**، فهذا يشير إلى وجود مشاكل تتعلق باتصال العميل مع نقطة الإدارة. رجاءً راجع **CcmMessaging.log** على الجهاز للتحقق من مشاكل الاتصال المحتملة.

- إذا كانت القيمة هي **معطّل** وتم تسجيل الجهاز في Intune، فرجاءً تأكد من أن الجهاز قد تلقى نهج الإدارة المشتركة من خلال مراجعة **CoManagementHandler.log** على الجهاز.
