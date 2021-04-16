---
title: تقاعد أدوات eDiscovery القديمة
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001487"
- "3523"
ms.openlocfilehash: 986c78f20e7b8c303c302913d63d817a56ce2896
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51798536"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a><span data-ttu-id="324d0-102">تقاعد أدوات eDiscovery القديمة</span><span class="sxs-lookup"><span data-stu-id="324d0-102">Retirement of Legacy eDiscovery Tools</span></span>

<span data-ttu-id="324d0-103">نتيجة لوظائف eDiscovery الجديدة والمحسنة في مركز التوافق ل Microsoft 365، سيتم في الأشهر القادمة إعزال أدوات eDiscovery والأوامر القديمة التالية:</span><span class="sxs-lookup"><span data-stu-id="324d0-103">As a result of the new and improved eDiscovery functionality in Microsoft 365 Compliance center, the following legacy eDiscovery tools and commandlets will be retired in the coming months:</span></span>

- <span data-ttu-id="324d0-104">[يتم وضع eDiscovery والمواعيد](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) [في](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) مكانها في مركز إدارة Exchange.</span><span class="sxs-lookup"><span data-stu-id="324d0-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) and [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.</span></span>

- <span data-ttu-id="324d0-105">Cmdlets في Exchange Online PowerShell التي تدعم In-Place eDiscovery In-Place المواعيد.</span><span class="sxs-lookup"><span data-stu-id="324d0-105">The Exchange Online PowerShell cmdlets that support In-Place eDiscovery and In-Place Holds.</span></span> <span data-ttu-id="324d0-106">(يتم تعريف cmdlets هذه بشكل جماعي على أنها cmdlets \*-MailboxSearch.) يشمل ذلك cmdlets التالية:</span><span class="sxs-lookup"><span data-stu-id="324d0-106">(These cmdlets are collectively identified as \*-MailboxSearch cmdlets.) This includes the following cmdlets:</span></span>

    - [<span data-ttu-id="324d0-107">البحث عن علبة بريد جديدة</span><span class="sxs-lookup"><span data-stu-id="324d0-107">New-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [<span data-ttu-id="324d0-108">Start-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="324d0-108">Start-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [<span data-ttu-id="324d0-109">Stop-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="324d0-109">Stop-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [<span data-ttu-id="324d0-110">Set-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="324d0-110">Set-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- <span data-ttu-id="324d0-111">الأمر [cmdlet "البحث في علبة](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) البريد" في Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="324d0-111">The [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet in Exchange Online PowerShell.</span></span>
- <span data-ttu-id="324d0-112">العمليات التالية في API ل Exchange Web Services:</span><span class="sxs-lookup"><span data-stu-id="324d0-112">The following operations in the Exchange Web Services API:</span></span>
    - [<span data-ttu-id="324d0-113">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="324d0-113">GetSearchableMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [<span data-ttu-id="324d0-114">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="324d0-114">SetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [<span data-ttu-id="324d0-115">GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="324d0-115">GetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [<span data-ttu-id="324d0-116">eDiscovery المتقدم v1.0</span><span class="sxs-lookup"><span data-stu-id="324d0-116">Advanced eDiscovery v1.0</span></span>](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

<span data-ttu-id="324d0-117">**المخطط الزمني للتقاعد**:</span><span class="sxs-lookup"><span data-stu-id="324d0-117">**Timeline for retirement**:</span></span>
- <span data-ttu-id="324d0-118">**1 يوليو 2020** لم يعد بإمكانك إنشاء عمليات بحث وعمليات حفظ جديدة، ولكن يمكنك تشغيل عمليات البحث الموجودة وتحريرها وحذفها على حسابك الخاص.</span><span class="sxs-lookup"><span data-stu-id="324d0-118">**July 1, 2020** You can no longer create new searches and holds, but you can run, edit, and delete existing searches at your own risk.</span></span> <span data-ttu-id="324d0-119">لم يعد دعم Microsoft يدعم In-Place eDiscovery & في EAC.</span><span class="sxs-lookup"><span data-stu-id="324d0-119">Microsoft Support no longer supports In-Place eDiscovery & Holds in the EAC.</span></span>
    
- <span data-ttu-id="324d0-120">1 أكتوبر **2020** In-Place eDiscovery & سيتم وضع وظائف "المواضع الموضعية" في EAC في وضع القراءة فقط، بحيث يمكنك إزالة عمليات البحث والمواضع الموضعية الموجودة فقط.</span><span class="sxs-lookup"><span data-stu-id="324d0-120">**October 1, 2020** In-Place eDiscovery & Holds functionality in the EAC will be placed in read-only mode, so you can only remove existing searches and holds.</span></span>

<span data-ttu-id="324d0-121">**لمزيد من المعلومات، راجع:**</span><span class="sxs-lookup"><span data-stu-id="324d0-121">**For more information, see**:</span></span>

 - [<span data-ttu-id="324d0-122">ترحيل عمليات بحث eDiscovery القديمة والمحتجزة إلى مركز التوافق في Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="324d0-122">Migrate legacy eDiscovery searches and holds to the Microsoft 365 compliance center</span></span>](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [<span data-ttu-id="324d0-123">تقاعد أدوات eDiscovery القديمة</span><span class="sxs-lookup"><span data-stu-id="324d0-123">Retirement of legacy eDiscovery tools</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [<span data-ttu-id="324d0-124">الأسئلة والأسئلة In-Place eDiscovery In-Place المواعيد</span><span class="sxs-lookup"><span data-stu-id="324d0-124">FAQs about In-Place eDiscovery and In-Place Holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



