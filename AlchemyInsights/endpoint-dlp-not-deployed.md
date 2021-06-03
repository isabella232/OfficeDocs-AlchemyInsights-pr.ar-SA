---
title: نقطة النهاية DLP غير منشرة على جهاز المستخدم
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/27/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11470"
- "9000292"
ms.openlocfilehash: 948835f5468b480536c176bfdf3b4eefb76b3bdb
ms.sourcegitcommit: c32233a1b7e6f1b07913d25f90189a58a8de2560
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/27/2021
ms.locfileid: "52731246"
---
# <a name="endpoint-dlp-not-deployed-to-users-device"></a>نقطة النهاية DLP غير منشرة على جهاز المستخدم

إذا لم يتم تطبيق إعداد منع فقدان بيانات نقطة النهاية (DLP) على جهاز مستخدم، فتأكد من أنك تلبي هذه المتطلبات:

- Windows 10 x64 1809 أو أي وقت لاحق مثبتا على الجهاز.
- تم تثبيت إصدار عميل مكافحة البرامج الضارة 4.18.2009.7 أو إصدار أحدث.
- الجهاز هو **أحد** هذه:
    
    - Azure Active Directory (Azure AD) المنضم
    - Azure AD المختلط المنضم
    - AAD مسجل

- لفرض إجراءات النهج، تأكد من تثبيت microsoft Chromium Edge على جهاز نقطة النهاية.

للحصول على متطلبات إضافية لنشر نقطة النهاية DLP، راجع بدء استخدام منع [فقدان بيانات نقطة النهاية](/microsoft-365/compliance/endpoint-dlp-getting-started#prepare-your-endpoints).