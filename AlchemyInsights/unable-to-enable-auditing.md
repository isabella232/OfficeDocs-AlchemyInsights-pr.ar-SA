---
title: 2419--إلى-تمكين-مراجعة الحسابات
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 2419
ms.assetid: ''
ms.openlocfilehash: 3af01c03711eed646f0009afb5bea685bc358196
ms.sourcegitcommit: 87153fec6f6468b57893abf4aac073ba4068e67b
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/19/2019
ms.locfileid: "35065593"
---
# <a name="unable-to-enable-unified-auditing"></a>غير قادر على تمكين تدقيق موحدة

عند محاولة تمكين تدقيق موحدة للمؤسسة الخاصة بك Office 365، قد تتلقى خطأ مشابهة ما يلي:

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

لحل هذه المشكلة، اتبع الخطوات التالية:

1. [الاتصال بتبادل Powershell عبر الإنترنت](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).

2. قم بتشغيل cmdlet التالية:

   ```
   Enable-OrganizationCustomization
   ```

3. الانتظار لمدة 60 دقيقة للإعداد السابق ساري المفعول.

4. تشغيل الأمر التالي في PowerShell Exchange عبر إنترنت:

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

لمزيد من المعلومات، راجع المقالات التالية:

- [الاتصال باستخدام مصادقة متعددة العوامل PowerShell Exchange عبر إنترنت](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [تشغيل أو إيقاف تشغيل البحث سجل التدقيق Office 365](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off)
