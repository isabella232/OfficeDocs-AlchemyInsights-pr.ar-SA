---
title: التغيير من خدمات أسماء Microsoft إلى إدارة سجلات DNS الخاصة بك
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13988"
- "14"
ms.openlocfilehash: a228bcda1220011ab994de7aa70f19ea092e2142
ms.sourcegitcommit: e9e282be4997b0ee95f1ff4491e0943f8fc52444
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/22/2021
ms.locfileid: "59506200"
---
# <a name="changing-from-microsoft-nameservers-back-to-managing-your-own-dns-records"></a>التغيير من خدمات أسماء Microsoft إلى إدارة سجلات DNS الخاصة بك

لقد قمت مسبقا بتغيير سجلات NS لتشير إلى Microsoft (ns1.bdm.microsoftonline.com) ولكنك قررت الآن إدارة سجلات DNS الخاصة بك:

في موقع جهة تسجيل المجالات على الويب، يمكنك تغيير اسم الخدمة مرة أخرى إلى جهة التسجيل أو الإعداد السابق. إذا لم تكن ملما باستخدام DNS، فاتصل بالدعم لدى جهة تسجيل المجالات. تجدر الإشارة إلى أن عملية نشر تغييرات خدمات الاسم قد تستغرق ما يصل إلى 48 ساعة. 

1. في مدخل Microsoft 365، انتقل إلى الإعدادات المجالات ، وحدد خانة الاختيار بجانب المجال،  >  [](https://admin.microsoft.com/Adminportal/Home#/Domains)وحدد **إدارة DNS**. 

2. في المعالج، حدد **إضافة سجلات DNS** الخاصة بك وإكمال المعالج. هذا الأمر يغير طريقة إدارة DNS، ثم يسمح لك بإضافة سجلات DNS المخصصة المطلوبة لدعم خدماتك المحددة.

بدلا من ذلك، إذا قمت بتغيير سجلات أسماءserver إلى Microsoft وكان لديك موقع ويب، يمكنك إضافة سجلات DNS لموقع ويب بدلا من تغيير أسماءservers مرة أخرى. لمزيد من المعلومات، راجع [تحديث سجلات DNS لإبقاء](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider)موقعك على ويب مع موفر الاستضافة الحالي.


