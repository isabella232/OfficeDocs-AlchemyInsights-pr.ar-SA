---
title: لا يرى مستخدم واحد الوظائف الإضافية في Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: 647a17bb5220d3591934c4f53cf417d42810b2c1a681bafd3e2d703abbfcbc64
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54050645"
---
# <a name="single-user-not-seeing-add-ins-in-outlook"></a>لا يرى مستخدم واحد الوظائف الإضافية في Outlook

قد يكون المستخدم جزءا من دور لا تملك المعلمة الصحيحة AppsForOfficeEnabled. تشغيل أمر cmdlet هذا لمعرفة ما إذا كان الدور الصحيح مقترن بالمستخدم:

Get-ManagementRoleAssignment -RoleAssignee user@domain.com -تفويض $false | Format-Table -Auto Role,RoleAssigneeName,RoleAssigneeType

لمزيد من المعلومات، راجع [تحديد المسؤولين](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins)والمستخدمين الذين يمكنهم تثبيت الوظائف الإضافية وإدارتها Outlook .
