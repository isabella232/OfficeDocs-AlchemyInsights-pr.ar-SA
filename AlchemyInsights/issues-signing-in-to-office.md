---
title: مشكلات تسجيل الدخول إلى تطبيقات Microsoft 365
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
ms.openlocfilehash: 4658b4df8a48072b4cc9d72bf503d7911bb5126b
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579888"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>شاشة تسجيل الدخول الفارغة في تطبيقات Microsoft 365

لإصلاح هذه المشكلة، حاول ما يلي:
- تثبيت آخر التحديثات [لـ Windows](https://support.microsoft.com/help/4027667/windows-10-update) و [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- إعادة تعيين خيارات Internet **Tools**Explorer: انتقل إلى  >  **أدوات خيارات إنترنت**  >  **Advanced**  >  **المتقدمة إعادة تعيين إعدادات إنترنت إكسبلورر** (لاحظ أنك سوف تفقد الإعدادات المخصصة)، ومن ثم حاول تسجيل الدخول إلى Office مرة أخرى.
- تعطيل حارس تطبيق Windows Defender (WDAG) أو أي جدار حماية مماثل أو برنامج مضاد للفيروسات:
    1. في لوحة التحكم، انتقل إلى **البرامج،** ثم اختر **تشغيل ميزات Windows أو إيقاف تشغيلها**.
    2. إذا تم تمكين Windows Defender Application Guard، فحاول تعطيله.<br/>
    **ملاحظة:** قد تحتاج إلى إعادة تشغيل الكمبيوتر.
- تأكد من أن Microsoft.AAD.BrokerPlugin [AAD WAM المكونات في](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) لا يتم حظرها من قبل أي تطبيق أو جدار الحماية / برنامج مكافحة الفيروسات.
- [مسح بيانات اعتماد Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) باستخدام إدارة بيانات اعتماد Windows.<br/>
    **ملاحظة:** تم تغيير مسارات التسجيل لـ Office 2016 إلى 16.0. (على سبيل: \Software\Microsoft\Office\16.0\Common\Identity\)

لمزيد من المعلومات، راجع [مشكلات "تسجيل الدخول" في "الاتصال" بعد التحديث إلى Office 2016 بناء 16.0.7967 على Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).