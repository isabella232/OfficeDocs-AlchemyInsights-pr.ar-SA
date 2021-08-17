---
title: مجموعة النسخ المتماثلة
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
- "9004400"
- "9004395"
- "8265"
- "9276"
ms.openlocfilehash: 45cf530c3258fa3c7008c3e8251fdb7b74be6911d0487f58c5ce2530e25ca282
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54110667"
---
# <a name="replica-set"></a>مجموعة النسخ المتماثلة

يسمى AADDS أيضا المجال المدار. إنه في الواقع جهازي تحكم للمجال يتم تشغيلها وصيانتها بواسطة الواجهة الخلفية. تتضمن اثنتان من DCs DC رئيسي واحد ونسخة متماثلة واحدة DC. النسخ الاحتياطية في AADDS (المجال المدار) هي عملية تلقائية مدارة بواسطة نظام Azure الأساسي. في حالة وجود مشكلة في مجالك المدار، يمكن أن يساعدك دعم Azure في الاستعادة من النسخ الاحتياطي.

يمكنك إنشاء كل مجموعة نسخ متماثلة في شبكة ظاهرية. يجب أن تكون كل شبكة ظاهرية نظيرة لكل شبكة ظاهرية أخرى تستضيف مجموعة النسخ المتماثلة لمجال مدار. ينشئ هذا التكوين طبولوجيا شبكة شبكة تدعم تكرار الدليل. يمكن للشبكة الظاهرية دعم مجموعات نسخ متماثلة متعددة، شرط أن تكون كل مجموعة نسخ متماثلة في شبكة فرعية ظاهرية مختلفة.

لمزيد من التفاصيل حول مجموعة النسخ المتماثلة، راجع [مجموعات المفاهيم المتماثلة](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets).
