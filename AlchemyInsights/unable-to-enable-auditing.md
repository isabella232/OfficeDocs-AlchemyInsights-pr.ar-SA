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
# <a name="unable-to-enable-unified-auditing"></a><span data-ttu-id="475f8-102">غير قادر على تمكين التدقيق الموحد</span><span class="sxs-lookup"><span data-stu-id="475f8-102">Unable to enable unified auditing</span></span>

<span data-ttu-id="475f8-103">عند محاولة تمكين التدقيق الموحد لمؤسستك، قد تتلقى خطأ مشابه لما يلي:</span><span class="sxs-lookup"><span data-stu-id="475f8-103">When you try to enable unified auditing for your organization, you may receive an error similar the following:</span></span>

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

<span data-ttu-id="475f8-104">لحل هذه المشكلة، اتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="475f8-104">To resolve this issue, follow these steps:</span></span>

1. <span data-ttu-id="475f8-105">[الاتصال تبادل Powershell عبر الإنترنت](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).</span><span class="sxs-lookup"><span data-stu-id="475f8-105">[Connect to Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).</span></span>

2. <span data-ttu-id="475f8-106">تشغيل cmdlet التالية:</span><span class="sxs-lookup"><span data-stu-id="475f8-106">Run the following cmdlet:</span></span>

   ```
   Enable-OrganizationCustomization
   ```

3. <span data-ttu-id="475f8-107">انتظر لمدة 60 دقيقة حتى يدخل الإعداد السابق حيز التنفيذ.</span><span class="sxs-lookup"><span data-stu-id="475f8-107">Wait for 60 minutes for the previous setting to take effect.</span></span>

4. <span data-ttu-id="475f8-108">تشغيل الأمر التالي في Exchange Online PowerShell:</span><span class="sxs-lookup"><span data-stu-id="475f8-108">Run the following command in Exchange Online PowerShell:</span></span>

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

<span data-ttu-id="475f8-109">لمزيد من المعلومات، راجع المقالات التالية:</span><span class="sxs-lookup"><span data-stu-id="475f8-109">For additional information, see the following articles:</span></span>

- [<span data-ttu-id="475f8-110">الاتصال بـ Exchange Online PowerShell باستخدام المصادقة متعددة العوامل</span><span class="sxs-lookup"><span data-stu-id="475f8-110">Connect to Exchange Online PowerShell using multi-factor authentication</span></span>](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [<span data-ttu-id="475f8-111">تشغيل البحث في سجل التدقيق أو إيقاف تشغيله</span><span class="sxs-lookup"><span data-stu-id="475f8-111">Turn audit log search on or off</span></span>](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off)
