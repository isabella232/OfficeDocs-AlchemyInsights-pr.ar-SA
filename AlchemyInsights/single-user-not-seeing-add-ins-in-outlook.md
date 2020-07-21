---
title: مستخدم واحد لا يرى الوظائف الإضافية في Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: 1f547c3f593b3256bd44f518aacbc36ed1c4c848
ms.sourcegitcommit: a05276bd623466ad211e1f8d9f0c616672dd3640
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 07/16/2020
ms.locfileid: "45197705"
---
# <a name="single-user-not-seeing-add-ins-in-outlook"></a>مستخدم واحد لا يرى الوظائف الإضافية في Outlook

قد يكون المستخدم جزءاً من دور لا يحتوي على المعلمة AppsForOfficeEnabled الصحيحة. تشغيل هذا cmdlet لمعرفة ما إذا كان الدور الصحيح مقترن مع المستخدم:

الحصول على إدارةRoleAssignment -RoleAssignee user@domain.com -تفويض $false | تنسيق-جدول -دور السيارات،RoleAssigneeName،RoleAssigneeType

لمزيد من المعلومات، راجع [تحديد المسؤولين والمستخدمين الذين يمكنهم تثبيت الوظائف الإضافية لـ Outlook وإدارتها](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).
