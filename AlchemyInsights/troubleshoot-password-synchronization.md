---
title: استكشاف أخطاء مزامنة كلمة المرور وإصلاحها
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 54b5a033b7cbb99520425b31800364ed4a99a4e6
ms.sourcegitcommit: 1d01b8b48eef2d5d10c375dcf802cd36e9d6bf61
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 07/23/2020
ms.locfileid: "45387864"
---
# <a name="troubleshoot-password-synchronization"></a>استكشاف أخطاء مزامنة كلمة المرور وإصلاحها

لاستكشاف مشكلات مزامنة كلمة المرور وإصلاحها، ابدأ باستخدام مهمة استكشاف أخطاء AAD Connect لاستكشاف الأخطاء وإصلاحها لتحديد سبب عدم مزامنة كلمات المرور. للبدء، انتقل إلى [إدارة المزامنة المباشرة](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).  

1. افتح جلسة عمل جديدة لـ Windows PowerShell على خادم Azure AD Connect، وحدد الخيار **تشغيل كمسؤول.**

2. تشغيل مجموعة التنفيذ عن بعدIgnSigned أو تعيين تنفيذPolispoli.

3. بدء تشغيل معالج الاتصال الإعلان Azure.

4. انتقل إلى صفحة المهام الإضافية > **استكشاف الأخطاء**  >  **وإصلاحها بعد ذلك**.

5. حدد **Launch** لفتح القائمة PowerShell لاستكشاف الأخطاء وإصلاحها.

6. حدد **استكشاف أخطاء مزامنة كلمة المرور وإصلاحها**.

    المشكلة عادةً لا تتم مزامنة كلمة مرور لحساب مستخدم معين.

    **ملاحظات** فشل مزامنة كلمة المرور إذا كانت آخر مزامنة ناجحة لكلمة المرور منذ بعض الوقت.

لمزيد من المساعدة في استكشاف أخطاء مزامنة كلمة المرور وإصلاحها، راجع [استكشاف أخطاء مزامنة تجزئة كلمة المرور وإصلاحها مع مزامنة Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).