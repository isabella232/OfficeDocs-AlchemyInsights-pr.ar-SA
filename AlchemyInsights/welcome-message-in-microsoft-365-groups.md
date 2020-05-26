---
title: رسالة ترحيب في مجموعات Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "5685"
ms.openlocfilehash: d82931ae6978a09e674b00640d1dd413bcce7cfd
ms.sourcegitcommit: b196100759b29aecd62b693a2bfedbbd25a697c6
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/19/2020
ms.locfileid: "44357255"
---
# <a name="welcome-message-in-microsoft-365-groups"></a>رسالة ترحيب في مجموعات Microsoft 365

سيتلقى المستخدمون الجدد الذين ينضمون إلى مجموعة Microsoft 365 بريدًا إلكترونيًا مرحبًا به إذا كانت خاصية "UnifiedGroupWelcomeMessageEnabled" صحيحة.

في حال كنت ترغب في تعطيل رسالة الترحيب، استخدم الأمر [التالي EXO PowerShell:](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps)

`
Set-UnifiedGroup <groupname> -UnifiedGroupWelcomeMessageEnabled:$False
`
