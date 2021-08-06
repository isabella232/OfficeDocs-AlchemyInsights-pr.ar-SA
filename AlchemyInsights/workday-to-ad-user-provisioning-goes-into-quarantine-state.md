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
ms.openlocfilehash: 32a5d010b95b9587e121ca1526def743fd8f371b13d1d73d3578c692839edf19
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54036479"
---
# <a name="workday-to-ad-user-provisioning-goes-into-quarantine-state"></a>يوم عمل لتوفير مستخدم AD إلى حالة الفحص

**يوم عمل لتوفير مستخدم AD إلى حالة الفحص ولا يتم إنشاء أي مستخدمين في AD**

لقد وصلت مهمة توفير يوم العمل إلى مستخدم AD إلى حالة الفحص وتظهر سجلات التدقيق أحداث فشل التصدير مع رسالة **الخطأ: OperationsError-SvcErr: حدث خطأ في العملية. لم يتم تكوين مرجع أفضل لخدمة الدليل. وبالتالي، يتعذر** على خدمة الدليل إصدار إحالات إلى كائنات خارج هذه الغابات. يظهر هذا الخطأ عادة إذا لم يتم تعيين OU حاوية Active Directory بشكل صحيح أو إذا كانت هناك مشاكل في تعيين التعبير المستخدم ل **parentDistinguishedName**.

تحقق من معلمة OU الافتراضية **للمستخدمين** الجدد للتحقق من الأخطاء المطبعية. تأكد من وجود OU المحدد بالفعل في AD. إذا كنت تستخدم **parentDistinguishedName** في تعيين السمات، فتأكد من تقييمها دائما إلى حاوية معروفة ضمن مجال AD. تحقق من الحدث تصدير في سجلات التدقيق لرؤية القيمة التي تم إنشاؤها.

لمزيد من التفاصيل حول تكوين يوم العمل للتكوين التلقائي، راجع البرنامج [التعليمي: تكوين يوم](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)عمل لتوفير تلقائي للمستخدم .

