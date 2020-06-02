---
title: 2419-غير قادر على تمكين التدقيق
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 2419
ms.assetid: ''
ms.openlocfilehash: 23ad07a6dd943d61d1bd45453089a771cfd51b58
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510415"
---
# <a name="unable-to-enable-unified-auditing"></a>غير قادر على تمكين التدقيق الموحد

عند محاولة تمكين التدقيق الموحد لمؤسستك، قد تتلقى خطأ مشابه لما يلي:

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

لحل هذه المشكلة، اتبع الخطوات التالية:

1. [الاتصال تبادل Powershell عبر الإنترنت](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).

2. تشغيل cmdlet التالية:

   ```
   Enable-OrganizationCustomization
   ```

3. انتظر لمدة 60 دقيقة حتى يدخل الإعداد السابق حيز التنفيذ.

4. تشغيل الأمر التالي في Exchange Online PowerShell:

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

لمزيد من المعلومات، راجع المقالات التالية:

- [الاتصال بـ Exchange Online PowerShell باستخدام المصادقة متعددة العوامل](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [تشغيل البحث في سجل التدقيق أو إيقاف تشغيله](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off)
