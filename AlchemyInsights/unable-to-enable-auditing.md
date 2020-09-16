---
title: 2419-لا يمكن-لتمكين-التدقيق
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 2419
ms.assetid: ''
ms.openlocfilehash: 81fd8e33feb2f2b10b04cc7cdc746a8603aa366b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47767586"
---
# <a name="unable-to-enable-unified-auditing"></a>تعذر تمكين التدقيق الموحد

عند محاولة تمكين التدقيق الموحد لمؤسسك ، قد تتلقي رسالة خطا مماثله لما يلي:

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

لحل هذه المشكلة ، اتبع الخطوات التالية:

1. [الاتصال ب Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).

2. شغل أمر cmdlet التالي:

   ```
   Enable-OrganizationCustomization
   ```

3. انتظر حتى 60 دقيقه لكي يدخل الاعداد السابق حيز التنفيذ.

4. قم بتشغيل الأمر التالي في Exchange Online PowerShell:

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

للحصول علي مزيد من المعلومات ، راجع المقالات التالية:

- [الاتصال ب Exchange Online PowerShell باستخدام مصادقه متعددة العوامل](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [تشغيل ميزه البحث في سجل التدقيق أو إيقاف تشغيلها](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off)
