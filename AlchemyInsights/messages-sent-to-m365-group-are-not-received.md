---
title: الرسائل المرسلة إلى مجموعة Microsoft 365 لا يستلمها جميع الأعضاء
ms.author: pebaum
author: pebaum
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
- "5995"
ms.openlocfilehash: 73c0fd3eb2f022b1c5917849bae676b748025fb69a3a15ba1389b42a6854db9c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53976492"
---
# <a name="messages-sent-to-a-microsoft-365-group-are-not-received-by-all-members"></a>الرسائل المرسلة إلى مجموعة Microsoft 365 لا يستلمها جميع الأعضاء

تأكد من أن جميع أعضاء المجموعة مشتركين في استلام رسائل البريد الإلكتروني. اطلع على [متابعة مجموعة في Outlook](https://support.microsoft.com/office/e147fc19-f548-4cd2-834f-80c6235b7c36).  

للتحقق من حالة الرسائل لدى الأعضاء المشتركين في رسائل البريد الإلكتروني للمجموعة، قم بتشغيل الأمر التالي على [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true):

`Get-UnifiedGroup <GroupName> | Get-UnifiedGroupLinks -LinkType Subscribers`

استخدم أمر EXO PowerShell التالي لتكوين كل أعضاء المجموعة على استلام رسائل البريد الإلكتروني المرسلة إلى مجموعة Microsoft 365 في علبة الوارد لديهم:

`$Group = "Address of [Microsoft 365 Groups]"Get-UnifiedGroupLinks $Group -LinkType Member | % {Add-UnifiedGroupLinks -Identity $Group -LinkType subscriber -Links $_.Guid.toString() -Confirm:$false}`

على سبيل المثال:

`$Group = "testg@contoso.onmicrosoft.com"Get-UnifiedGroupLinks $Group -LinkType Member | % {Add-UnifiedGroupLinks -Identity $Group -LinkType subscriber -Links $_.Guid.toString() -Confirm:$false}`