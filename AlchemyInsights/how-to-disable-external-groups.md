---
title: كيفية تعطيل المجموعات الخارجية
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: 2159feb4aa3999072de57d76790a2959c7355976
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43720755"
---
# <a name="how-to-disable-external-groups"></a>كيفية تعطيل المجموعات الخارجية

تطبق الرسائل الخارجية Yammer قواعد نقل Exchange (ETRs)، وهي مجموعة من عناصر التحكم الاستباقية لمنع مشاركة معلومات الشركة. لتقييد المستخدمين من إنشاء مجموعات خارجية، تحتاج إلى تكوين قاعدة نقل Exchange (ETR)، ثم تكوين Yammer لاستخدام قاعدة Exchange Transport لمنع المراسلة الخارجية.
  
بمجرد إنشاء قاعدة في مركز إدارة Exchange Online، اتبع هذه الخطوات لتعيين ETR للتطبيق في Yammer:
  
- قم بتسجيل الدخول إلى Yammer كمسؤول تم التحقق منه، وفي **مركز مسؤول Yammer**، انتقل إلى إعدادات أمان المحتوى والأمان ** \> C.**

- ضمن **المراسلة الخارجية،** حدد **فرض قواعد نقل التبادل عبر الإنترنت (ETRs) في Yammer.**

- اختر **حفظ**.

لمزيد من المعلومات، راجع [تعطيل المراسلة الخارجية في شبكة Yammer](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).
  