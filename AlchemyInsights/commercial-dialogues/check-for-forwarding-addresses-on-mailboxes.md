---
title: التحقق من عناوين إعادة توجيه علب البريد
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002486"
- "7524"
ms.openlocfilehash: 3abd45230360c61ecb62e4b7a39d1b0b547271fc
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403298"
---
# <a name="check-for-forwarding-addresses-on-mailboxes"></a><span data-ttu-id="57969-102">التحقق من عناوين إعادة توجيه علب البريد</span><span class="sxs-lookup"><span data-stu-id="57969-102">Check for forwarding addresses on mailboxes</span></span>

<span data-ttu-id="57969-103">في بعض الأحيان، يقوم المتسللون ب إعادة توجيه رسائل البريد الإلكتروني الخاصة بالمستخدمين إلى أنفسهم، لذا سنتحقق أولا من إعادة توجيه العناوين والقواعد في علبة البريد.</span><span class="sxs-lookup"><span data-stu-id="57969-103">Sometimes hackers forward users' email messages to themselves, so first we'll check for forwarding addresses and rules on the mailbox.</span></span> <span data-ttu-id="57969-104">ثم سنتحقق من سجلات التدقيق.</span><span class="sxs-lookup"><span data-stu-id="57969-104">Then we'll check the audit logs.</span></span> <span data-ttu-id="57969-105">فيما يلي كيفية التحقق من عناوين إعادة توجيه:</span><span class="sxs-lookup"><span data-stu-id="57969-105">Here's how to check for forwarding addresses:</span></span>

1. <span data-ttu-id="57969-106">حدد   >  **المستخدمون المستخدمون النشطون**.</span><span class="sxs-lookup"><span data-stu-id="57969-106">Select **Users** > **Active users**.</span></span>
1. <span data-ttu-id="57969-107">حدد المستخدم الذي تم اختراق حسابه.</span><span class="sxs-lookup"><span data-stu-id="57969-107">Select the user whose account has been compromised.</span></span>
1. <span data-ttu-id="57969-108">في القائمة flyout التي تظهر، قم بتوسيع **إعدادات البريد**، ثم انقر فوق **تحرير** إعادة توجيه **البريد الإلكتروني**.</span><span class="sxs-lookup"><span data-stu-id="57969-108">In the flyout that appears, expand **Mail Settings**, and then click **Edit** for **Email forwarding**.</span></span>
1. <span data-ttu-id="57969-109">قم بإزالة أي عناوين إعادة توجيه لا تتعرف عليها.</span><span class="sxs-lookup"><span data-stu-id="57969-109">Remove any forwarding addresses you don't recognize.</span></span>