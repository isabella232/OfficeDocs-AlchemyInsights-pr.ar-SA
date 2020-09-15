---
title: رسائل البريد الكتروني المفقودة في الفحص
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
- "5668"
- "9002625"
ms.openlocfilehash: 55ed9a92675939c05477fbf6d12bbedd6eb931d6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47673701"
---
# <a name="missing-emails-in-quarantine"></a>رسائل البريد الكتروني المفقودة في الفحص "

يمكن للمسؤولين [عرض هذه الرسائل أو تحريرها أو حذفها.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)

لفتح مركز توافق & الأمان ، انتقل إلى [https://protection.office.com](https://protection.office.com/) . لفتح صفحه الفحص مباشره ، انتقل إلى [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .  

يمكنك البحث بحسب القيم التالية:  

- **معرف الرسالة**: المعرف الفريد العمومي للرسالة. إذا قمت بتحديد رسالة في القائمة ، ستظهر قيمه  **معرف الرسالة**  في جزء  **التفاصيل**  المنبثق الذي يظهر. يمكن للمسؤولين استخدام [تتبع الرسائل](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) للبحث عن الرسائل وقيم معرف الرسائل المقابلة لها.
- **عنوان البريد الكتروني**للمرسل: عنوان البريد الكتروني الخاص بالمرسل.
- **عنوان البريد الكتروني للمستلم**: عنوان البريد الكتروني الخاص بمستلم واحد.
- **الموضوع**: استخدم الموضوع بالبالكامل في الرسالة. لا يكون البحث متحسسا لحاله الأحرف.

بعد إدخال معايير البحث ، انقر فوق ![ الزر تحديث ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Refresh** التحديث لتصفيه النتائج.  

أوامر cmdlets التي تستخدمها لعرض الرسائل والملفات وأدارتها في الفحص هي:
- [Delete-قوارانتينيميساجي](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [تصدير-قوارانتينيميساجي](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [قوارانتينيميساجي](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [معاينه-قوارانتينيميساجي](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): لاحظ ان أمر cmdlet هذا للرسائل فقط ، وليس الملفات الضارة من ATP ل SharePoint Online أو OneDrive for business أو الفرق.
- [الإصدار-قوارانتينيميساجي](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)