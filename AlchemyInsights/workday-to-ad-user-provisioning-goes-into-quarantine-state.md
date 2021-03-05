---
title: يوم عمل لتوفير مستخدم AD إلى حالة الفحص
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8471"
- "9004687"
ms.openlocfilehash: 0fc519c8170de498c9bcb1fc41a76116bda48b1f
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/04/2021
ms.locfileid: "50480839"
---
# <a name="workday-to-ad-user-provisioning-goes-into-quarantine-state"></a>يوم عمل لتوفير مستخدم AD إلى حالة الفحص

**يوم عمل لتوفير مستخدم AD إلى حالة الفحص ولا يتم إنشاء أي مستخدمين في AD**

لقد وصلت مهمة توفير يوم العمل لمستخدم AD إلى حالة الفحص وتظهر سجلات التدقيق أحداث فشل التصدير مع رسالة **الخطأ: OperationsError-SvcErr: حدث خطأ في العملية. لم يتم تكوين مرجع أفضل لخدمة الدليل. وبالتالي، يتعذر** على خدمة الدليل إصدار إحالات إلى كائنات خارج هذه الغابات. يظهر هذا الخطأ عادة إذا لم يتم تعيين OU حاوية Active Directory بشكل صحيح أو إذا كانت هناك مشاكل في تعيين التعبير المستخدم ل **parentDistinguishedName.**

تحقق من معلمة OU الافتراضية **للمستخدمين** الجدد للتأكد من الأخطاء الطباعية. تأكد من وجود OU المحدد بالفعل في AD. إذا كنت تستخدم **parentDistinguishedName** في تعيين السمة، فتأكد من تقييمها دائما إلى حاوية معروفة داخل مجال AD. تحقق من الحدث "تصدير" في سجلات التدقيق لرؤية القيمة التي تم إنشاؤها.

لمزيد من التفاصيل حول تكوين يوم العمل للتكوين التلقائي، راجع البرنامج [التعليمي: تكوين يوم](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)عمل للتكوين التلقائي للمستخدم.

