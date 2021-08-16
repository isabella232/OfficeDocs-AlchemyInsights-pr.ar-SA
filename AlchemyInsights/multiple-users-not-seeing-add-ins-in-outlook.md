---
title: لا يرى عدة مستخدمين الوظائف الإضافية في Outlook
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
ms.openlocfilehash: 850df2cb349f9a751def3d59fb665670e70e493daba56a88821afcef9c48ffa8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54011791"
---
# <a name="multiple-users-not-seeing-add-ins-in-outlook"></a>لا يرى عدة مستخدمين الوظائف الإضافية في Outlook

إذا قمت Outlook الوظائف الإضافية ولم تظهر أي منها، كخطوة أولى في استكشاف الأخطاء وإصلاحها، فاستخدم **الأمر Get-OrganizationConfig** PowerShell cmdlet للاستعلام عن المعلمة _AppsForOfficeEnabled._ إذا كان الاستعلام يرجع قيمة **False**، فحدد هذه المعلمة إلى **True** باستخدام **الأمر Cmdlet Set-OrganizationConfig،** بحيث تظهر الوظائف الإضافية كما هو متوقع.

لا نوصي بتعيين المعلمة _AppsForOfficeEnabled_ إلى **False**. تتجاوز قيمة **False** كل إعدادات الدور الإداري ودور المستخدم أعلاه وتمنع أي تطبيقات جديدة من التنشيط من قبل أي مستخدم في المؤسسة.

لمزيد من المعلومات، راجع تحديد المسؤولين والمستخدمين الذين يمكنهم تثبيت الوظائف الإضافية وإدارتها [Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles).