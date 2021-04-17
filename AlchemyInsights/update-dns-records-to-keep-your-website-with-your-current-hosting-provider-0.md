---
title: تحديث سجلات DNS لإبقاء موقعك على ويب مع موفر الاستضافة الحالي
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "42"
- "43"
- "100002"
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: 89bce2aa5931c0c20706efabd42d2351be43938b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51827492"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a>تحديث سجلات DNS لإبقاء موقعك على ويب مع موفر الاستضافة الحالي

1. في مركز إدارة Microsoft 365، انتقل إلى صفحة مجالات الإعداد، وفي قائمة المجالات، حدد المجال الذي تستخدمه  >  [](https://admin.microsoft.com/Adminportal#/Domains) لموقعك على ويب.

2. حدد **+ سجل مخصص جديد** وأدخل ما يلي:

  - بالنسبة **لنوع DNS،** أدخل: **أ (عنوان)**

  - بالنسبة **إلى اسم المضيف أو الاسم المستعار**، اكتب ما يلي: **@**

  - بالنسبة **إلى عنوان IP**، اكتب عنوان IP الثابت لموقعك على ويب حيث يستضيفه حاليا (على سبيل المثال، 172.16.140.1).

    يجب أن يكون  *هذا عنوان*  IP ثابتا لموقع ويب، وليس  *عنوان*  IP ديناميكيا. تحقق من الموقع الذي يستضيف موقعك على ويب للتأكد من أنه يمكنك الحصول على عنوان IP ثابت لموقعك العام على ويب.

3. حدد **حفظ**.

بالإضافة إلى ذلك، يمكنك إنشاء سجل CNAME لمساعدة العملاء في العثور على موقعك على ويب.
  
1. حدد **+ سجل مخصص جديد** وأدخل ما يلي:

  - بالنسبة **لنوع DNS،** أدخل: **CNAME (الاسم المستعار)**

  - بالنسبة **إلى اسم المضيف أو الاسم المستعار**، اكتب ما يلي: **www**

  - لنقاط **العنوان**، اكتب اسم المجال المؤهل بالكامل (FQDN) لموقعك على ويب (على سبيل المثال، contoso.com).

2. حدد **حفظ**.
