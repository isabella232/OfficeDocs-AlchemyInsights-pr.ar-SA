---
title: مشاكل في تسجيل الدخول إلى تطبيقات Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2556"
ms.openlocfilehash: e6cbab7401fd6168041e7fc31ac97e3be036536d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833011"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>شاشة تسجيل الدخول الفارغة في تطبيقات Microsoft 365

لإصلاح هذه المشكلة، جرب ما يلي:
- تثبيت التحديثات الأخيرة [لنظامي التشغيل Windows و](https://support.microsoft.com/help/4027667/windows-10-update) [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- إعادة تعيين خيارات Internet Explorer: انتقل إلى أدوات خيارات الإنترنت المتقدمة إعادة تعيين إعدادات Internet Explorer (لاحظ أنك ستفقد الإعدادات المخصصة)، ثم حاول تسجيل الدخول  >    >    >   إلى Office مرة أخرى.
- قم بتعطيل Windows Defender Application Guard (WDAG) أو أي برنامج مماثل لجدار الحماية أو برنامج مكافحة الفيروسات:
    1. في لوحة التحكم، انتقل إلى **البرامج**، ثم اختر **تشغيل ميزات Windows أو إيقاف تشغيلها**.
    2. إذا تم تمكين Windows Defender Application Guard، فحاول تعطيله.<br/>
    **ملاحظة:** قد تحتاج إلى إعادة تشغيل الكمبيوتر.
- تأكد من عدم حظر المكون الإضافية Microsoft.AAD.BrokerPlugin [AAD WAM](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) بواسطة أي تطبيق أو برنامج جدار حماية/مكافحة الفيروسات.
- [مسح بيانات اعتماد Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) باستخدام إدارة بيانات اعتماد Windows.<br/>
    **ملاحظة:** تم تغيير مسارات التسجيل ل Office 2016 إلى 16.0. (على ما يلي: \Software\Microsoft\Office\16.0\Common\Identity\)

لمزيد من المعلومات، راجع مشاكل الاتصال في تسجيل الدخول بعد التحديث إلى [إصدار Office 2016 16.0.7967 على Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).