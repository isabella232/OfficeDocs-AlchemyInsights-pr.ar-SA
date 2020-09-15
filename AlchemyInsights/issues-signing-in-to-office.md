---
title: المشاكل المتعلقة بتسجيل الدخول إلى تطبيقات Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2556"
ms.openlocfilehash: 3c016b198ad43f35c8149dde71c28a2f7fc3bd38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695274"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>شاشه تسجيل الدخول الفارغة في تطبيقات Microsoft 365

لإصلاح هذه المشكلة ، جرب ما يلي:
- تثبيت آخر التحديثات ل [Windows](https://support.microsoft.com/help/4027667/windows-10-update) و [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- أعاده تعيين خيارات internet explorer: **Tools**انتقل إلى  >  **أدوات الإنترنت خيارات**  >  أعاده تعيين**متقدمة**  >  **لإعدادات internet Explorer** (لاحظ انك ستفقد الإعدادات المخصصة) ، ثم حاول تسجيل الدخول إلى Office مره أخرى.
- تعطيل ' حماية التطبيقات ل Windows Defender ' (فداج) أو اي برنامج جدار حماية مشابه أو برامج مكافحه الفيروسات:
    1. في لوحه التحكم ، انتقل إلى **البرامج**، ثم اختر **تشغيل ميزات Windows أو إيقاف تشغيلها**.
    2. إذا تم تمكين حماية التطبيقات ل Windows Defender ، فجرب تعطيلها.<br/>
    **ملاحظه:** قد تحتاج إلى أعاده تشغيل الكمبيوتر.
- تاكد من انه لم يتم حظر [المكون الإضافي بروكيربلوجين aad](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) الخاص ب aad ، بواسطة اي تطبيق أو جدار حماية/برنامج مكافحه الفيروسات.
- [مسح بيانات اعتماد Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) باستخدام "أداره بيانات اعتماد Windows".<br/>
    **ملاحظه:** لقد تغيرت مسارات التسجيل ل Office 2016 إلى 16.0. (علي سبيل المثال: \Software\Microsoft\Office\16.0\Common\Identity\)

لمزيد من المعلومات ، راجع [مشاكل الاتصال في تسجيل الدخول بعد التحديث إلى Office 2016 16.0.7967 علي Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).