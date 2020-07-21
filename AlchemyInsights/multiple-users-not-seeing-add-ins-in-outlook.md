---
title: مستخدمين متعددين لا يرون الوظائف الإضافية في Outlook
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
ms.openlocfilehash: 18d3fa535a88af18d8c4b02a5371d0a81c8d28c0
ms.sourcegitcommit: a05276bd623466ad211e1f8d9f0c616672dd3640
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 07/16/2020
ms.locfileid: "45197707"
---
# <a name="multiple-users-not-seeing-add-ins-in-outlook"></a>مستخدمين متعددين لا يرون الوظائف الإضافية في Outlook

إذا قمت باختبار Outlook الوظائف الإضافية و لا تظهر أي خطوة استكشاف الأخطاء وإصلاحها الأولى استخدم cmdlet **Get-OrganizationConfig** PowerShell الاستعلام _المعلمة AppsForOfficeEnabled._ إذا كان الاستعلام بإرجاع قيمة **خطأ**، تعيين هذه المعلمة إلى **True** باستخدام cmdlet **Set-OrganizationConfig** ، لذلك تظهر الوظائف الإضافية كما هو متوقع.

لا ننصح تعيين _معلمة AppsForOfficeEnabled_ إلى **False**. تتجاوز قيمة **False** كافة إعدادات دور "الإداري" و"المستخدم" أعلاه وتمنع أي تطبيقات جديدة من أن يتم تنشيطها من قبل أي مستخدم في المؤسسة.

لمزيد من المعلومات، راجع [تحديد المسؤولين والمستخدمين الذين يمكنهم تثبيت الوظائف الإضافية لـ Outlook وإدارتها](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles).