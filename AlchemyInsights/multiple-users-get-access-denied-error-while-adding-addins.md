---
title: ظهور رسالة الخطا "رفض الوصول" لعده مستخدمين اثناء أضافه وظائف اضافيه في Outlook
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
ms.openlocfilehash: 611a4df473458abc0ab0c65442f2141763f7b868
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47724350"
---
# <a name="multiple-users-get-access-denied-error-while-adding-add-ins-in-outlook"></a>ظهور رسالة الخطا "رفض الوصول" لعده مستخدمين اثناء أضافه وظائف اضافيه في Outlook

يمكنك تحديد المسؤولين الذين لديهم الأذونات لتثبيت الوظائف الاضافيه وأدارتها ل Outlook. يمكنك أيضا تحديد المستخدمين الذين لديهم الاذن لتثبيت الوظائف الاضافيه وأدارتها لاستخدامها.

للحصول علي التفاصيل ، راجع [تحديد المسؤولين والمستخدمين الذين يمكنهم تثبيت الوظائف الاضافيه وأدارتها ل Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).

للتحقق من انك قمت بتعيين الأذونات لمستخدم بنجاح ، استبدل <Role Name> باسم الدور الذي تريد التحقق منه ، ثم قم بتشغيل الأمر التالي في Exchange Online PowerShell:

ماناجيمينتروليسيجنمينت-Role " <Role Name> "-جيتيفيكتيفيوسيرس

يوضح هذا المثال كيفيه التحقق من الأشخاص الذين قمت بتعيين أذونات لهم لتثبيت الوظائف الاضافيه من متجر Office للمؤسسة.

PowerShell

-الدور "التطبيقات الخاصة بسوق المؤسسة"-جيتيفيكتيفيوسيرس

في النتائج ، ماناجيمينتروليسيجنمينت ، راجع الإدخالات في العمود المستخدمون الفعالون.

للحصول علي معلومات تفصيليه حول المعلمات وبناءها ، راجع [ماناجيمينتروليسيجنمينت](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).
 