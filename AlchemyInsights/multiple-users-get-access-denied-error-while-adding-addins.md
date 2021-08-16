---
title: يحصل عدة مستخدمين على خطأ رفض الوصول أثناء إضافة الوظائف الإضافية في Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5892"
- "6700008"
ms.openlocfilehash: 5e5f881ad72d2a0f76c8659d6b1044bf6a18464fa8d65c079e44eb1a2afd4431
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54065379"
---
# <a name="multiple-users-get-access-denied-error-while-adding-add-ins-in-outlook"></a>يحصل عدة مستخدمين على خطأ رفض الوصول أثناء إضافة الوظائف الإضافية في Outlook

يمكنك تحديد المسؤولين في مؤسستك الذين لديهم الأذونات لتثبيت الوظائف الإضافية وإدارتها Outlook. يمكنك أيضا تحديد المستخدمين في مؤسستك الذين لديهم الإذن لتثبيت الوظائف الإضافية وإدارتها لاستخدامها الخاص.

للحصول على التفاصيل، راجع [تحديد المسؤولين](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins)والمستخدمين الذين يمكنهم تثبيت الوظائف الإضافية وإدارتها Outlook .

للتحقق من أنك قمت بتعيين أذونات لمستخدم بنجاح، استبدل باسم الدور الذي يجب التحقق منه، ثم قم بتشغيل الأمر التالي <Role Name> في Exchange Online PowerShell:

Get-ManagementRoleAssignment -Role " <Role Name> " -GetEffectiveUsers

يوضح لك هذا المثال كيفية التحقق من الأشخاص الذين قمت بتعيين أذونات لتثبيت الوظائف الإضافية من Office Store الخاص بهذه المؤسسة.

PowerShell

-Role "Org Marketplace Apps" -GetEffectiveUsers

في النتائج، Get-ManagementRoleAssignment، راجع الإدخالات في العمود المستخدمون الفعّالون.

للحصول على معلومات مفصلة حول بناء الجملة والمعلمات، راجع [Get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).
 