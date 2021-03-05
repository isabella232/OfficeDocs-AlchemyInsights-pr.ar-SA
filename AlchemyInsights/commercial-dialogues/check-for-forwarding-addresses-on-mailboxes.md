---
title: التحقق من إعادة توجيه العناوين في علب البريد
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 17/02/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002486"
- "7524"
ms.openlocfilehash: 1b0a6c8fe368196f2d1f9811aea895c2c024b2e6
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/05/2021
ms.locfileid: "50480949"
---
# <a name="check-for-forwarding-addresses-on-mailboxes"></a><span data-ttu-id="edf5a-102">التحقق من إعادة توجيه العناوين في علب البريد</span><span class="sxs-lookup"><span data-stu-id="edf5a-102">Check for forwarding addresses on mailboxes</span></span>

<span data-ttu-id="edf5a-103">في بعض الأحيان، يقوم المتسللون إعادة توجيه رسائل البريد الإلكتروني الخاصة بالمستخدمين لأنفسهم، لذا أولا سنتحقق من إعادة توجيه العناوين والقواعد في علبة البريد.</span><span class="sxs-lookup"><span data-stu-id="edf5a-103">Sometimes hackers forward users' email messages to themselves, so first we'll check for forwarding addresses and rules on the mailbox.</span></span> <span data-ttu-id="edf5a-104">ثم سنتحقق من سجلات التدقيق.</span><span class="sxs-lookup"><span data-stu-id="edf5a-104">Then we'll check the audit logs.</span></span> <span data-ttu-id="edf5a-105">فيما يلي كيفية التحقق من إعادة توجيه العناوين:</span><span class="sxs-lookup"><span data-stu-id="edf5a-105">Here's how to check for forwarding addresses:</span></span>

1. <span data-ttu-id="edf5a-106">حدد   >  **المستخدمين النشطين.**</span><span class="sxs-lookup"><span data-stu-id="edf5a-106">Select **Users** > **Active users**.</span></span>
1. <span data-ttu-id="edf5a-107">حدد المستخدم الذي تم اختراق حسابه.</span><span class="sxs-lookup"><span data-stu-id="edf5a-107">Select the user whose account has been compromised.</span></span>
1. <span data-ttu-id="edf5a-108">في القائمة flyout التي تظهر، قم بتوسيع **"إعدادات** البريد"، ثم انقر فوق **"تحرير"** إعادة **توجيه البريد الإلكتروني.**</span><span class="sxs-lookup"><span data-stu-id="edf5a-108">In the flyout that appears, expand **Mail Settings**, and then click **Edit** for **Email forwarding**.</span></span>
1. <span data-ttu-id="edf5a-109">قم بإزالة أي عناوين إعادة توجيه لا تتعرف عليها.</span><span class="sxs-lookup"><span data-stu-id="edf5a-109">Remove any forwarding addresses you don't recognize.</span></span>