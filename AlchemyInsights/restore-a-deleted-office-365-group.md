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
ms.openlocfilehash: b72b7c93ce9fe1b90d1608811b0eeabc8aec1363
ms.sourcegitcommit: a5edaaefdc56f8d5c8220a335f4e8228e2de4ee0
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/08/2021
ms.locfileid: "51645118"
---
# <a name="restore-a-deleted-microsoft-365-group"></a>استعادة مجموعة Microsoft 365 محذوفة

يمكنك استعادة مجموعة Microsoft 365 أو Microsoft Teams محذوفة في غضون 30 يوما من عملية الحذف.

1. انتقل إلى [مركز إدارة Microsoft 365](https://aka.ms/RestoreDeletedGroup) لتسجيل الدخول إلى قائمة المجموعات والفرق المحذوفة.

    **ملاحظة:** سجل دخولك باستخدام الحساب المعين إلى مسؤول المستأجر أو دور مسؤول المجموعات.

1. حدد مجموعة Microsoft 365/Teams المحذوفة لاستعادتها وانقر فوق **استعادة المجموعة**.

    إذا لم تتمكن من استعادة المجموعة بسبب وجود عنوان SMTP متضارب، فاستخدم الأمر التالي للعثور على الكائن الذي يتسبب في حدوث تعارض وإزالة عنوان SMTP:

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    **ملاحظة:** في بعض الحالات، قد يستغرق الأمر 24 ساعة حتى يتم استعادة المجموعة وكل بياناتها.

    لمزيد من المعلومات، أو للتعرف على كيفية استعادة المجموعات باستخدام PowerShell، راجع [استعادة مجموعة Microsoft 365 محذوفة](https://go.microsoft.com/fwlink/?linkid=867802).