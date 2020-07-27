---
title: يحصل العديد من المستخدمين على خطأ تم رفض الوصول أثناء إضافة الوظائف الإضافية في Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5892"
- "6700008"
ms.openlocfilehash: 624d880c535b7d8888b676ff23c774c6d138a75a
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 07/24/2020
ms.locfileid: "45423304"
---
# <a name="multiple-users-get-access-denied-error-while-adding-add-ins-in-outlook"></a>يحصل العديد من المستخدمين على خطأ تم رفض الوصول أثناء إضافة الوظائف الإضافية في Outlook

يمكنك تحديد المسؤولين في المؤسسة التي لديك أذونات لتثبيت الوظائف الإضافية لـ Outlook وإدارتها. يمكنك أيضاً تحديد المستخدمين الذين لديهم إذن في مؤسستك لتثبيت الوظائف الإضافية وإدارتها لاستخدامهم الخاص.

للحصول على التفاصيل، راجع [تحديد المسؤولين والمستخدمين الذين يمكنهم تثبيت الوظائف الإضافية لـ Outlook وإدارتها](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).

للتحقق من أنك قمت بتعيين الأذونات لمستخدم بنجاح، استبدل <Role Name> باسم الدور للتحقق من صحة، ثم قم بتشغيل الأمر التالي في Exchange Online PowerShell:

الحصول على إدارةRoleAssignment -دور " <Role Name> - GetEffectiveUsers

يوضح لك هذا المثال كيفية التحقق من الأشخاص الذين قمت بتعيينهم للأذونات لتثبيت الوظائف الإضافية من متجر Office للمؤسسة.

Powershell

-Role "Org Marketplace Apps" - GetEffectiveUsers

في النتائج، Get-ManagementRoleAssignment، راجع الإدخالات في العمود "المستخدمين الفعالين".

للحصول على معلومات تفصيلية عن بناء الجملة والمعلمة، راجع [Get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).
 