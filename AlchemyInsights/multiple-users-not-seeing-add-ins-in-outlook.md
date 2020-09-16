---
title: مستخدمون متعددون لا يريون الوظائف الاضافيه في Outlook
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
ms.openlocfilehash: a0c272f40044795754ed8630e88e00ed14ea6ad7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47729858"
---
# <a name="multiple-users-not-seeing-add-ins-in-outlook"></a>مستخدمون متعددون لا يريون الوظائف الاضافيه في Outlook

إذا قمت باختبار وظائف Outlook الاضافيه ولم يظهر اي من الخطوات الاولي ، فاستخدم الأمر **get-organizationconfig** cmdlet للاستعلام عن المعلمة _أبسفوروفيسينابليد_ . إذا ارجع الاستعلام قيمه **False**، فقم بتعيين هذه المعلمة إلى **True** باستخدام الأمر **get-organizationconfig** cmdlet ، بحيث تظهر الوظائف الاضافيه كما هو متوقع.

لا نوصي بتعيين المعلمة _أبسفوروفيسينابليد_ إلى **False**. تتجاوز قيمه **False** كل إعدادات ادوار المستخدمين والمسؤولين السابقة وتمنع تنشيط اي تطبيقات جديده من قبل اي مستخدم في المؤسسة.

لمزيد من المعلومات ، راجع [تحديد المسؤولين والمستخدمين الذين يمكنهم تثبيت الوظائف الاضافيه وأدارتها ل Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles).