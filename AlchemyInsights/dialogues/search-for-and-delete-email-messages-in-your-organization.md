---
title: البحث عن رسائل البريد الإلكتروني وحذفها في مؤسستك
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000260"
- "7257"
ms.openlocfilehash: e935b10083459b81fc58e12bb59c9511defefa6d
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/05/2021
ms.locfileid: "50523128"
---
# <a name="search-for-and-delete-email-messages-in-your-organization"></a><span data-ttu-id="bb174-102">البحث عن رسائل البريد الإلكتروني وحذفها في مؤسستك</span><span class="sxs-lookup"><span data-stu-id="bb174-102">Search for and delete email messages in your organization</span></span>

<span data-ttu-id="bb174-103">اتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="bb174-103">Follow these steps:</span></span>

1. <span data-ttu-id="bb174-104">إذا لم تكن المسؤول العام، للبحث عن الرسائل، يجب إضافة حسابك إلى مجموعة دور **مدير eDiscovery** أو دور إدارة بحث **التوافق.**</span><span class="sxs-lookup"><span data-stu-id="bb174-104">If you're not a global admin, to search for messages your account must be added to the **eDiscovery Manager role group** or **Compliance Search management role**.</span></span> <span data-ttu-id="bb174-105">لحذف الرسائل، ستحتاج إلى الانضمام إلى مجموعة دور **"إدارة** المؤسسة" أو دور إدارة البحث **واحذف.**</span><span class="sxs-lookup"><span data-stu-id="bb174-105">To delete messages, you'll need to join the **Organization Management role group** or the **Search and Purge management role**.</span></span> <span data-ttu-id="bb174-106">يتم تعيين الأذونات لهذه الأدوار في مركز التوافق & [الأمان.](https://protection.office.com)</span><span class="sxs-lookup"><span data-stu-id="bb174-106">Permissions to these roles are assigned in the [Security & compliance center.](https://protection.office.com)</span></span>
2. <span data-ttu-id="bb174-107">[أنشئ عملية بحث في المحتوى](https://docs.microsoft.com/office365/securitycompliance/content-search) للعثور على الرسالة التي تريد حذفها.</span><span class="sxs-lookup"><span data-stu-id="bb174-107">[Create a content search](https://docs.microsoft.com/office365/securitycompliance/content-search) to find the message to delete.</span></span>
3. <span data-ttu-id="bb174-108">[الاتصال بمركز & التوافق في PowerShell.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell)</span><span class="sxs-lookup"><span data-stu-id="bb174-108">[Connect to Security & Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).</span></span> <span data-ttu-id="bb174-109">إذا كنت تستخدم المصادقة متعددة العوامل، فشاهد هذه الإرشادات: الاتصال بمركز التوافق & [PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell) باستخدام المصادقة متعددة العوامل</span><span class="sxs-lookup"><span data-stu-id="bb174-109">If you're using MFA, see these instructions: [Connect to Security & Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)</span></span>
4. <span data-ttu-id="bb174-110">احذف الرسالة: قم `New-ComplianceSearchAction` بتشغيل الأمر cmdlet لحذف الرسالة.</span><span class="sxs-lookup"><span data-stu-id="bb174-110">Delete the message: run the `New-ComplianceSearchAction` cmdlet to delete the message.</span></span> <span data-ttu-id="bb174-111">يتم نقل الرسائل المحذوفة إلى مجلد "العناصر القابلة لاسترداد" الخاص بالمستخدم.</span><span class="sxs-lookup"><span data-stu-id="bb174-111">Deleted messages are moved to a user's Recoverable Items folder.</span></span> <span data-ttu-id="bb174-112">للحصول على مثال على الأمر، راجع [الخطوة 3: حذف الرسالة.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)</span><span class="sxs-lookup"><span data-stu-id="bb174-112">For an example command, see [Step 3: Delete the message.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)</span></span>
