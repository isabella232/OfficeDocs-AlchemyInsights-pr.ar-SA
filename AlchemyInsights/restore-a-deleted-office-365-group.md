---
title: استعادة مجموعة Microsoft 365 محذوفة
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "98"
- "1200024"
ms.assetid: bc0396ea-c426-4d1d-bb89-ced602d06fb6
ms.openlocfilehash: caa2c8987eecb89bac3469bf9471847858cab0ba
ms.sourcegitcommit: ec99a3a2e1e6a13d9a829d65ad1692a607dc3a17
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/06/2021
ms.locfileid: "51597430"
---
# <a name="restore-a-deleted-microsoft-365-group"></a><span data-ttu-id="f8865-102">استعادة مجموعة Microsoft 365 محذوفة</span><span class="sxs-lookup"><span data-stu-id="f8865-102">Restore a deleted Microsoft 365 group</span></span>

<span data-ttu-id="f8865-103">يمكنك استعادة مجموعة Microsoft 365 أو Microsoft Teams محذوفة في غضون 30 يوما من عملية الحذف.</span><span class="sxs-lookup"><span data-stu-id="f8865-103">You can restore a deleted Microsoft 365 group or Microsoft Teams within 30 days from the deletion.</span></span>

1. <span data-ttu-id="f8865-104">انتقل إلى [مركز إدارة Microsoft 365](https://aka.ms/RestoreDeletedGroup) لتسجيل الدخول وإضافة قائمة بالمجموعات والفرق المحذوفة.</span><span class="sxs-lookup"><span data-stu-id="f8865-104">Go to the [Microsoft 365 admin center](https://aka.ms/RestoreDeletedGroup) to log in and list the deleted groups and teams.</span></span>

    <span data-ttu-id="f8865-105">**ملاحظة:** سجل دخولك باستخدام الحساب المعين إلى مسؤول المستأجر أو دور مسؤول المجموعات.</span><span class="sxs-lookup"><span data-stu-id="f8865-105">**Note:** Log in using the account that is assigned to either the tenant administrator or the groups admin role.</span></span>

1. <span data-ttu-id="f8865-106">حدد مجموعة Microsoft 365/Teams المحذوفة لاستعادتها وانقر فوق **استعادة المجموعة**.</span><span class="sxs-lookup"><span data-stu-id="f8865-106">Select the deleted Microsoft 365 group/Teams to be restored and click **restore group**.</span></span>

    <span data-ttu-id="f8865-107">إذا لم تتمكن من استعادة المجموعة بسبب وجود عنوان SMTP متضارب، فاستخدم الأمر التالي للعثور على الكائن الذي يتسبب في حدوث تعارض وإزالة عنوان SMTP:</span><span class="sxs-lookup"><span data-stu-id="f8865-107">If the group can't be restored because of a conflicting SMTP address, use following command to find the object that’s causing conflict and remove the SMTP address:</span></span>

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    <span data-ttu-id="f8865-108">**ملاحظة:** في بعض الحالات، قد يستغرق الأمر 24 ساعة حتى يتم استعادة المجموعة وكل بياناتها.</span><span class="sxs-lookup"><span data-stu-id="f8865-108">**Note:** In some cases, it might take as long as 24 hours for the group and all of its data to be restored.</span></span>

    <span data-ttu-id="f8865-109">لمزيد من المعلومات، أو للتعرف على كيفية استعادة المجموعات باستخدام PowerShell، راجع [استعادة مجموعة Microsoft 365 محذوفة](https://go.microsoft.com/fwlink/?linkid=867802).</span><span class="sxs-lookup"><span data-stu-id="f8865-109">For more info, or to learn how to restore groups using PowerShell, see [Restore a deleted Microsoft 365 group](https://go.microsoft.com/fwlink/?linkid=867802).</span></span>