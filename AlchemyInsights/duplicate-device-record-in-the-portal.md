---
title: سجل جهاز مكرر في المدخل
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4386"
ms.openlocfilehash: e32486236a318ae820538cf87c2019e05470211d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47678491"
---
# <a name="duplicate-device-record-in-the-portal"></a>سجل جهاز مكرر في المدخل

يمكنك رؤية سجلين للجهاز في المدخل، إذا لم يقم الجهاز بالإبلاغ عن حالة الإدارة المشتركة بشكل صحيح في موقع إدارة التكوين. للتحقق من حالة الإدارة المشتركة للجهاز، راجع عمود **الإدارة المشتركة** للجهاز في وحدة تحكم إدارة التكوين. إذا لم يكن العمود مرئياً، فيمكنك إضافته بالنقر بزر الماوس الأيمن فوق أي من رؤوس الأعمدة، وتحديده من القائمة.

القيمة المُدارة بشكل مشترك يجب أن تكون **نعم**. إذا كانت القيمة هي **لا**، فافتح التطبيق الصغير لعميل إدارة التكوين على جهاز العميل وتحقق من خاصية **الإدارة المشتركة** في علامة التبويب "عام".

- إذا كانت القيمة هي **ممكَّن**، فهذا يشير إلى وجود مشاكل تتعلق باتصال العميل مع نقطة الإدارة. رجاءً راجع **CcmMessaging.log** على الجهاز للتحقق من مشاكل الاتصال المحتملة.

- إذا كانت القيمة هي **معطّل** وتم تسجيل الجهاز في Intune، فرجاءً تأكد من أن الجهاز قد تلقى نهج الإدارة المشتركة من خلال مراجعة **CoManagementHandler.log** على الجهاز.
