---
title: استكشاف الأخطاء في مزامنة كلمة المرور وإصلاحها
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: cb782c0d1dc396ee7a9f016afb9629a2cdee93d52f5408b7a73e576e783ebc0a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105735"
---
# <a name="troubleshoot-password-synchronization"></a>استكشاف الأخطاء في مزامنة كلمة المرور وإصلاحها

لاستعلام مشاكل مزامنة كلمة المرور وإصلاحها، ابدأ باستخدام مهمة استكشاف الأخطاء وإصلاحها الاتصال AAD هذه لتحديد سبب عدم مزامنة كلمات المرور. للبدء، انتقل إلى [إدارة المزامنة المباشرة](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).  

1. افتح جلسة عمل Windows PowerShell على خادم Azure AD الاتصال، وحدد **الخيار تشغيل كمسؤول.**

2. تشغيل Set-ExecutionPolicy RemoteSigned أو Set-ExecutionPolicy غير مقيد.

3. ابدأ تشغيل معالج Azure AD الاتصال AD.

4. انتقل إلى صفحة المهام الإضافية > **استكشاف الأخطاء التالية وإصلاحها.**  >  

5. حدد **تشغيل** لفتح قائمة استكشاف الأخطاء وإصلاحها في PowerShell.

6. حدد **استكشاف الأخطاء في مزامنة كلمة المرور وإصلاحها**.

    عادة ما تكون المشكلة عدم مزامنة كلمة مرور لحساب مستخدم معين.

    **الملاحظات** تفشل مزامنة كلمة المرور إذا كانت آخر مزامنة ناجحة لكلمة المرور قد تم منذ بعض الوقت.

للحصول على مزيد من المساعدة حول استكشاف الأخطاء وإصلاحها في مزامنة كلمة المرور، راجع استكشاف الأخطاء وإصلاحها في مزامنة كلمة المرور مع [Azure AD الاتصال مزامنة](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).