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
# <a name="how-to-enable-hosted-voicemail"></a>كيفيه تمكين البريد الصوتي المستضاف

لتمكين البريد الصوتي ، يجب تعيين **هوستيدفويسيميل** إلى $true.

الخاصية **هوستيدفويسيميل** علي المستخدم الذي يستخدم PowerShell البعيد (ربس).

لمزيد من المعلومات حول الاتصال ب ربس ، راجع [نظره عامه حول فرق Microsoft](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) للحصول علي مزيد من المعلومات حول الاتصال ب ربس.

1. يجب ان يتم تسجيل دخول مسؤول الفرق إلى PowerShell البعيد للفرق.
1. من موجه PowerShell ، يمكن لمسؤول الفرق تشغيل **move-csuser user@contoso.com-هوستيدفويسيميل $true** حيث يكون sip uri الخاص بالمستخدم.

> [!NOTE]
> قد تستغرق التغييرات في النهج ما يصل إلى 24 ساعة للنسخ المتماثل.