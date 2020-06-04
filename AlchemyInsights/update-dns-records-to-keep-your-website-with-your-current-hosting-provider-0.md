---
title: تحديث سجلات DNS للحفاظ على موقعك على الويب مع مزود الاستضافة الحالي
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "42"
- "43"
- "100002"
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: 7bd36c3954d12d3ee4ac624a2f827d8e5cd88082
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/02/2020
ms.locfileid: "36665747"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a>تحديث سجلات DNS للحفاظ على موقعك على الويب مع مزود الاستضافة الحالي

1. في مركز إدارة Microsoft 365، **Setup**انتقل إلى صفحة  >  [نطاقات](https://portal.office.com/adminportal/home#/Domains) الإعداد، وفي قائمة المجالات، حدد المجال الذي تستخدمه لموقعك على الويب.

2. حدد **+ سجل مخصص جديد** وأدخل ما يلي:

  - لإدخال **نوع DNS:** **أ (عنوان)**

  - لاسم **المضيف أو الاسم المستعار**، اكتب ما يلي:**@**

  - بالنسبة **إلى عنوان IP**، اكتب عنوان IP الثابت لموقع الويب الخاص بك حيث يتم استضافته حاليًا (على سبيل المثال ، 172.16.140.1).

    يجب أن يكون هذا عنوان IP *ثابت* لموقع الويب، وليس عنوان IP *ديناميكي.* تحقق مع الموقع الذي يتم فيه استضافة موقع الويب الخاص بك للتأكد من أنه يمكنك الحصول على عنوان IP ثابت لموقعك العام.

3. حدد **حفظ**.

بالإضافة إلى ذلك، يمكنك إنشاء سجل CNAME لمساعدة العملاء في العثور على موقعك على الويب.
  
1. حدد **+ سجل مخصص جديد** وأدخل ما يلي:

  - لإدخال **نوع DNS:** **CNAME (الاسم المستعار)**

  - لاسم **المضيف أو الاسم المستعار،** اكتب ما يلي: **www**

  - للحصول **على نقاط للعنوان**، اكتب اسم النطاق المؤهل بالكامل (FQDN) لموقعك على الويب (على سبيل المثال ، contoso.com).

2. حدد **حفظ**.
