---
title: المجموعة "إرسال Microsoft 365 باسم"
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/19/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
ms.openlocfilehash: 204b2c1777f76f11663b2735b784cbb56f1f1aba891628fb46ef37b501c9ff85
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54086115"
---
# <a name="send-as-microsoft-365-group"></a>المجموعة "إرسال Microsoft 365 باسم"

يمكنك تعيين أذونات "إرسال باسم" للسماح لمستخدمين معينين بإرسال الرسائل كمجموعة Microsoft 365:  

1. الاتصال Exchange Online PowerShell.  

2. قم بتنفيذ الأمر التالي:  

    Add-RecipientPermission `<GroupName>` -Trustee `<MailboxName>` -AccessRights SendAs

لمزيد من المعلومات، راجع [السماح للأعضاء بإرسال ك](https://docs.microsoft.com/microsoft-365/admin/create-groups/allow-members-to-send-as-or-send-on-behalf-of-group?view=o365-worldwide)أو إرسال نيابة عن مجموعة .