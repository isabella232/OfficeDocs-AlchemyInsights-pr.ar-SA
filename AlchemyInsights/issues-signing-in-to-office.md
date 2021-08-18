---
title: مشاكل في تسجيل الدخول إلى Microsoft 365 التطبيقات
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
ms.openlocfilehash: 7a8a0b68fc211e99b22e857d51d1de54e53a69357f75a0c60b1e83078cd5b27f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54088023"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>شاشة تسجيل الدخول الفارغة Microsoft 365 التطبيقات

لإصلاح هذه المشكلة، جرب ما يلي:
- قم بتثبيت التحديثات الأخيرة [Windows](https://support.microsoft.com/help/4027667/windows-10-update) [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- إعادة تعيين خيارات Internet Explorer: انتقل إلى أدوات خيارات الإنترنت المتقدمة إعادة تعيين Internet Explorer الإعدادات (لاحظ أنك ستفقد الإعدادات المخصصة)، ثم حاول تسجيل الدخول Office  >    >    >   مرة أخرى.
- قم بتعطيل حماية التطبيقات لـ Windows Defender (WDAG) أو أي برنامج مماثل لجدار الحماية أو برنامج مكافحة الفيروسات:
    1. في لوحة التحكم، انتقل إلى **البرامج**، ثم اختر تشغيل Windows **أو إيقاف تشغيلها**.
    2. إذا حماية التطبيقات لـ Windows Defender، فحاول تعطيله.<br/>
    **ملاحظة:** قد تحتاج إلى إعادة تشغيل الكمبيوتر.
- تأكد من عدم حظر المكون الإضافية Microsoft.AAD.BrokerPlugin [AAD WAM](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) بواسطة أي تطبيق أو برنامج جدار حماية/مكافحة الفيروسات.
- [مسح Office بيانات الاعتماد](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) باستخدام Windows بيانات الاعتماد.<br/>
    **ملاحظة:** تم تغيير مسارات التسجيل Office 2016 إلى 16.0. (على ما يلي: \Software\Microsoft\Office\16.0\Common\Identity\)

لمزيد من المعلومات، راجع مشاكل الاتصال في تسجيل الدخول بعد التحديث إلى Office [2016 16.0.7967 على Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).