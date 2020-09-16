---
title: حول الهوية في Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6039"
- "9003111"
ms.openlocfilehash: f417117acac4c3040932fc0a35e5d0b1c3709cd5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664157"
---
# <a name="about-identity-in-yammer"></a>حول الهوية في Yammer

من المستحسن تنفيذ كل الشبكات علي الخطوات التالية لتجنب المشاكل ذات الصلة بالهوية:

1. فرض هويه Office 365 بعد توفير حسابات Microsoft 365 للمستخدمين في Azure AD للتاكد من ان كل المستخدمين يقومون بتسجيل الدخول باستخدام حساب Microsoft 365 الأساسي الخاص بهم. للحصول علي مزيد من المعلومات ، راجع [فرض هويه Office 365 لمستخدمي Yammer](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).
2. دمج عده شبكات Yammer. تسمح تكوينات Yammer القديمة بتوصيل شبكات Yammer بمستاجر واحد. للحصول علي مزيد من المعلومات ، راجع [ترحيل الشبكة-دمج شبكات Yammer متعددة](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).
3. بشكل اختياري ، قم بفرض الترخيص ل Yammer لحظر المستخدمين من Yammer إذا لم يكن لديهم ترخيص. للحصول علي مزيد من المعلومات ، راجع [أداره تراخيص مستخدمي Yammer في Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).
4. أخيرا ، قم بتدوين قائمه المستخدمين لشبكات Yammer القديمة وتوقف المستخدمون القديمون. من المستحسن ان تقوم بإيقاف (إلغاء تنشيط) المستخدمين بدلا من حذفها ، لان الحذف غير مقبول. للحصول علي مزيد من المعلومات ، راجع [تدوين مستخدمي Yammer في الشبكات المتصلة ب Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) [وأزاله المستخدمين](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).

بتكوين Yammer باستخدام هذه الخطوات ، ستكون جاهزا أيضا لتكوين شبكه Yammer للوضع الأصلي ل Microsoft 365. لمزيد من المعلومات ، راجع [تكوين شبكه Yammer للوضع الأصلي ل Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).