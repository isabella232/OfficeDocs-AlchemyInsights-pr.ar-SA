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
ms.openlocfilehash: 3834696ff59b7e96e90a5b660a489003dfa9729c
ms.sourcegitcommit: 581c696ec108184adae9d4bc8f47cb9247131de8
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/10/2021
ms.locfileid: "50713306"
---
# <a name="replica-set"></a>مجموعة النسخ المتماثلة

ويسمى أيضا AADDS كمجال مدار. في الواقع، يوجد اثنين من وحدات تحكم المجالات التي يتم تشغيلها وصيانتها بواسطة الواجهة الخلفية. يتضمن كل من المكاتين DC رئيسي واحد و DC متماثلا واحدا. النسخ الاحتياطية في AADDS (المجال المدار) هي عملية تلقائية مدارة بواسطة نظام Azure الأساسي. في حالة وجود مشكلة في مجالك المدار، يمكن أن يساعدك دعم Azure في الاستعادة من النسخ الاحتياطي.

يمكنك إنشاء كل نسخة مماثلة تم تعيينها في شبكة ظاهرية. يجب أن يتم أقران كل شبكة ظاهرية إلى كل شبكة ظاهرية أخرى تستضيف مجموعة النسخ المتماثلة لمجال مدار. ينشئ هذا التكوين شبكة شبكة طبولوجيا تدعم تكرار الدليل. يمكن للشبكة الظاهرية دعم مجموعات نسخ مماثلة متعددة، شرط أن تكون كل مجموعة نسخ مماثلة في شبكة فرعية ظاهرية مختلفة.

لمزيد من التفاصيل حول مجموعة النسخ المتماثلة، راجع [مجموعات النسخ المتماثلة ل "المفاهيم".](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets)
