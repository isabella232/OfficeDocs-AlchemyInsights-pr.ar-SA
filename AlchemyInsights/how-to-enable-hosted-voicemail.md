---
title: كيفيه تمكين البريد الصوتي المستضاف
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/09/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002347"
- "7563"
ms.openlocfilehash: 26eb22054d246a6ca5a2491c68a5d9e4ed90d45b
ms.sourcegitcommit: 523098560e54a50184a99c974809dfbfffadacb5
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/09/2020
ms.locfileid: "49676736"
---
# <a name="how-to-enable-hosted-voicemail"></a><span data-ttu-id="05f78-102">كيفيه تمكين البريد الصوتي المستضاف</span><span class="sxs-lookup"><span data-stu-id="05f78-102">How to enable Hosted Voicemail</span></span>

<span data-ttu-id="05f78-103">لتمكين البريد الصوتي ، يجب تعيين **هوستيدفويسيميل** إلى $true.</span><span class="sxs-lookup"><span data-stu-id="05f78-103">To enable Voicemail, **HostedVoicemail** must be set to $true.</span></span>

<span data-ttu-id="05f78-104">الخاصية **هوستيدفويسيميل** علي المستخدم الذي يستخدم PowerShell البعيد (ربس).</span><span class="sxs-lookup"><span data-stu-id="05f78-104">The **HostedVoicemail** property on the user using Remote PowerShell (RPS).</span></span>

<span data-ttu-id="05f78-105">لمزيد من المعلومات حول الاتصال ب ربس ، راجع [نظره عامه حول فرق Microsoft](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) للحصول علي مزيد من المعلومات حول الاتصال ب ربس.</span><span class="sxs-lookup"><span data-stu-id="05f78-105">For more information on connecting to RPS, see [Microsoft Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) for more information on connecting to RPS.</span></span>

1. <span data-ttu-id="05f78-106">يجب ان يتم تسجيل دخول مسؤول الفرق إلى PowerShell البعيد للفرق.</span><span class="sxs-lookup"><span data-stu-id="05f78-106">The Teams Admin should be logged into Remote PowerShell for Teams.</span></span>
1. <span data-ttu-id="05f78-107">من موجه PowerShell ، يمكن لمسؤول الفرق تشغيل **move-csuser user@contoso.com-هوستيدفويسيميل $true** حيث يكون sip uri الخاص بالمستخدم.</span><span class="sxs-lookup"><span data-stu-id="05f78-107">From PowerShell prompt the Teams Admin can run **set-csuser user@contoso.com -HostedVoiceMail $true** where the sip uri is of the user in question.</span></span>

> [!NOTE]
> <span data-ttu-id="05f78-108">قد تستغرق التغييرات في النهج ما يصل إلى 24 ساعة للنسخ المتماثل.</span><span class="sxs-lookup"><span data-stu-id="05f78-108">Changes to policies can take up to 24 hours to replicate.</span></span>