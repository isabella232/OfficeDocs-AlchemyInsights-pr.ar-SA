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
# <a name="unable-to-enable-unified-auditing"></a><span data-ttu-id="fa7dd-102">تعذر تمكين التدقيق الموحد</span><span class="sxs-lookup"><span data-stu-id="fa7dd-102">Unable to enable unified auditing</span></span>

<span data-ttu-id="fa7dd-103">عند محاولة تمكين التدقيق الموحد لمؤسسك ، قد تتلقي رسالة خطا مماثله لما يلي:</span><span class="sxs-lookup"><span data-stu-id="fa7dd-103">When you try to enable unified auditing for your organization, you may receive an error similar the following:</span></span>

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

<span data-ttu-id="fa7dd-104">لحل هذه المشكلة ، اتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="fa7dd-104">To resolve this issue, follow these steps:</span></span>

1. <span data-ttu-id="fa7dd-105">[الاتصال ب Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).</span><span class="sxs-lookup"><span data-stu-id="fa7dd-105">[Connect to Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).</span></span>

2. <span data-ttu-id="fa7dd-106">شغل أمر cmdlet التالي:</span><span class="sxs-lookup"><span data-stu-id="fa7dd-106">Run the following cmdlet:</span></span>

   ```
   Enable-OrganizationCustomization
   ```

3. <span data-ttu-id="fa7dd-107">انتظر حتى 60 دقيقه لكي يدخل الاعداد السابق حيز التنفيذ.</span><span class="sxs-lookup"><span data-stu-id="fa7dd-107">Wait for 60 minutes for the previous setting to take effect.</span></span>

4. <span data-ttu-id="fa7dd-108">قم بتشغيل الأمر التالي في Exchange Online PowerShell:</span><span class="sxs-lookup"><span data-stu-id="fa7dd-108">Run the following command in Exchange Online PowerShell:</span></span>

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

<span data-ttu-id="fa7dd-109">للحصول علي مزيد من المعلومات ، راجع المقالات التالية:</span><span class="sxs-lookup"><span data-stu-id="fa7dd-109">For additional information, see the following articles:</span></span>

- [<span data-ttu-id="fa7dd-110">الاتصال ب Exchange Online PowerShell باستخدام مصادقه متعددة العوامل</span><span class="sxs-lookup"><span data-stu-id="fa7dd-110">Connect to Exchange Online PowerShell using multi-factor authentication</span></span>](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [<span data-ttu-id="fa7dd-111">تشغيل ميزه البحث في سجل التدقيق أو إيقاف تشغيلها</span><span class="sxs-lookup"><span data-stu-id="fa7dd-111">Turn audit log search on or off</span></span>](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off)
