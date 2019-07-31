---
title: مشكلات تسجيل الدخول إلى تطبيقات Office
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2556"
ms.openlocfilehash: 08bb0a94066f071f2ba0e9c54378f0d479191496
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938119"
---
# <a name="blank-sign-in-screen-in-office-apps"></a>شاشة تسجيل الدخول فارغة في تطبيقات Office

لحل هذه المشكلة، جرب ما يلي:
- تثبيت التحديثات ل [Windows](https://support.microsoft.com/help/4027667/windows-10-update) و [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- إعادة تعيين خيارات Internet Explorer: انتقل إلى **أدوات** > **خيارات إنترنت** > **خيارات متقدمة** > **إعادة تعيين إعدادات Internet Explorer** (لاحظ أنك ستفقد إعدادات مخصصة)، وثم حاول تسجيل الدخول إلى Office مرة أخرى.
- تعطيل حماية التطبيق Windows Defender (وداج) أو أي برنامج جدار حماية أو برنامج مكافحة الفيروسات مشابهة:
    1. في "لوحة التحكم"، انتقل إلى **البرامج**، وثم اختر **تشغيل ميزات Windows أو إيقاف تشغيله**.
    2. إذا تم تمكين حماية التطبيق Windows Defender، حاول تعطيله.<br/>
    **ملاحظة:** قد تحتاج إلى إعادة تشغيل الكمبيوتر.
- تأكد من أن Microsoft.AAD.BrokerPlugin [أم عاد المكون الإضافي](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) لا يتم حظر من قبل أي تطبيق أو برنامج جدار حماية/المضادة للفيروسات.
- ["مكتب مسح" بيانات الاعتماد](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) باستخدام إدارة بيانات اعتماد Windows.<br/>
    **ملاحظة:** لقد تغيرت المسارات لعام 2016 Office إلى 16.0. (مثلاً: \Software\Microsoft\Office\16.0\Common\Identity\)

لمزيد من المعلومات، راجع [اتصال مشكلات في تسجيل الدخول بعد التحديث إلى عام 2016 Office بناء 16.0.7967 على Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).