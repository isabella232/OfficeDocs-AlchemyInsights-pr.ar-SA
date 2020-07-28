---
title: غير قادر على تغيير اسم المستخدم
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1729"
- "9000183"
ms.openlocfilehash: 34aecdf503699ee500179f0958158fc964d77fcb
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 07/28/2020
ms.locfileid: "45438723"
---
# <a name="unable-to-change-username"></a>غير قادر على تغيير اسم المستخدم

في بعض الحالات، لا يتم نشر تغييرات UPN (UserPrincipalName) إلى مجموعة النظراء. قد تتلقى أخطاء التحقق من الصحة في مدخل Office 365 أو قد لا تتمكن من تغيير اسم المستخدم أو عنوان البريد الإلكتروني. لحل هذه المشكلة، يدوياً تعيين UserPrincipalName باستخدام هذا الأمر PowerShell.

**مثال: إعادة تسمية مستخدم**

PowerShellCopy

PS C: \> تعيين MsolUserPrincipalName -UserPrincipalName "davidc@contoso.com"-NewUserPrincipalName "davidchew@contoso.com"

يعيد هذا الأمر تسمية davidc@contoso.com إلى davidchew@contoso.com.

لمزيد من المعلومات، راجع [تعيين MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0).