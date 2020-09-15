---
title: نهج مشاركه تقويم 618
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: d2511183d068330cdcfb4e08b08df4f18625c822
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684217"
---
# <a name="policy-error-when-sharing-a-calendar"></a><span data-ttu-id="3513e-102">خطا في النهج عند مشاركه تقويم</span><span class="sxs-lookup"><span data-stu-id="3513e-102">Policy error when sharing a calendar</span></span>

1. <span data-ttu-id="3513e-103">قم بواحد مما يلي ، بما يتناسب مع حالتك:</span><span class="sxs-lookup"><span data-stu-id="3513e-103">Do one of the following, as appropriate for your situation:</span></span>
    - <span data-ttu-id="3513e-104">الاتصال ب Exchange Online باستخدام PowerShell البعيد.</span><span class="sxs-lookup"><span data-stu-id="3513e-104">Connect to Exchange Online by using Remote PowerShell.</span></span> <span data-ttu-id="3513e-105">لمزيد من المعلومات ، راجع [الاتصال ب Exchange Online باستخدام PowerShell البعيد](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="3513e-105">For more information, see [Connect to Exchange Online using Remote PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).</span></span>
    - <span data-ttu-id="3513e-106">علي الخادم المحلي ، افتح Exchange Management Shell.</span><span class="sxs-lookup"><span data-stu-id="3513e-106">On the on-premises server, open the Exchange Management Shell.</span></span>
2. <span data-ttu-id="3513e-107">تحديد نهج المشاركة الذي تم تعيينه إلى المستخدم.</span><span class="sxs-lookup"><span data-stu-id="3513e-107">Determine the sharing policy that's assigned to the user.</span></span> <span data-ttu-id="3513e-108">للقيام بذلك ، قم بتشغيل الأمر التالي ولاحظ ان النهج ارجع:</span><span class="sxs-lookup"><span data-stu-id="3513e-108">To do this, run the following command and note the policy returned:</span></span>

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. <span data-ttu-id="3513e-109">تحديث نهج المشاركة للمستخدم.</span><span class="sxs-lookup"><span data-stu-id="3513e-109">Update the sharing policy for the user.</span></span> <span data-ttu-id="3513e-110">لعمل ذلك، اتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="3513e-110">To do this, follow these steps:</span></span>
    - <span data-ttu-id="3513e-111">افتح مركز أداره Exchange.</span><span class="sxs-lookup"><span data-stu-id="3513e-111">Open the Exchange admin center.</span></span>
    - <span data-ttu-id="3513e-112">انقر فوق **المؤسسة**، ثم انقر نقرا مزدوجا فوق النهج الذي تم تعيينه إلى المستخدم ضمن **المشاركة الفردية**.</span><span class="sxs-lookup"><span data-stu-id="3513e-112">Click **Organization**, and then double-click the policy that's assigned to the user under **Individual Sharing**.</span></span> <span data-ttu-id="3513e-113">هذا هو النهج الذي تم إرجاعه في الخطوة 2.</span><span class="sxs-lookup"><span data-stu-id="3513e-113">This is the policy that was returned in step 2.</span></span>
    - <span data-ttu-id="3513e-114">في صفحه قاعده المشاركة ، حدد مستوي مشاركه التقويم الذي تريد السماح به ضمن **تحديد المعلومات التي تريد مشاركتها**؛ انقر فوق **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="3513e-114">On the Sharing Rule page, select the calendar sharing level that you want to allow under **Specify what information you want to share**; click **Save**.</span></span>

<span data-ttu-id="3513e-115">لمزيد من المعلومات ، راجع: ["لا يسمح النهج بمنح الأذونات الموجودة في هذا المستوي إلى رسالة واحده أو أكثر من المستلمين" عند محاولة المستخدم مشاركه التقويم](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).</span><span class="sxs-lookup"><span data-stu-id="3513e-115">For more information see: ["Policy does not allow granting permissions at this level to one or more of the recipient(s)" error when user tries to share calendar](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).</span></span>
