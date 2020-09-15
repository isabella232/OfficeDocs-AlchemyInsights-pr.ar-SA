---
title: استكشاف أخطاء مزامنة كلمه المرور وإصلاحها
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
ms.openlocfilehash: 96f63f2ae8e5de246bce7fc15a9b2c3d604f2eb8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664913"
---
# <a name="troubleshoot-password-synchronization"></a>استكشاف أخطاء مزامنة كلمه المرور وإصلاحها

لاستكشاف أخطاء مزامنة كلمات المرور وإصلاحها ، أبدا باستخدام المهمة التالية لاستكشاف الأخطاء وإصلاحها في AAD للبدء ، انتقل إلى [أداره المزامنة المباشرة](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).  

1. افتح جلسة Windows PowerShell جديده علي خادم Azure AD Connect ، وحدد الخيار **تشغيل كمسؤول** .

2. شغل Set اكسيكوتيونبوليسي ريموتيسيجنيد أو Set-اكسيكوتيونبوليسي غير مقيد.

3. أبدا تشغيل معالج Azure AD Connect.

4. انتقل إلى صفحه المهام الاضافيه > **استكشاف الأخطاء وإصلاحها**  >  **Next**.

5. حدد **تشغيل** لفتح قائمه استكشاف الأخطاء وإصلاحها في PowerShell.

6. حدد **استكشاف أخطاء مزامنة كلمه المرور وإصلاحها**.

    تحدث هذه المشكلة عاده بعدم مزامنة كلمه المرور لحساب مستخدم معين.

    **ملاحظات** تفشل مزامنة كلمه المرور إذا كانت آخر مزامنة ناجحه لكلمه المرور قد تم منذ بعض الوقت.

للحصول علي المزيد من المساعدة في استكشاف أخطاء مزامنة كلمه المرور [وإصلاحها ، راجع استكشاف أخطاء مزامنة تجزئه كلمه المرور باستخدام مزامنة AZURE AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).