---
title: إنشاء موقع في SharePoint Online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: b9009fdbdc2a5e7443151446daade1685d2f5d45
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/04/2020
ms.locfileid: "41770410"
---
# <a name="create-sharepoint-sites-using-templates"></a>إنشاء مواقع SharePoint باستخدام القوالب

لا يتم دعم القدرة على حفظ موقع كقالب مع مواقع الاتصال أو الفريق الحديثة. لمزيد من المعلومات حول استخدام القوالب راجع [حفظ موقع SharePoint وتنزيله وتحميله كقالب](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).

فيما يلي بعض المشكلات/الحلول الشائعة فيما يتعلق بحفظ موقع أو قائمة كقالب في Sharepoint Online. 

**حفظ زر قالب الموقع/القائمة غير متوفر أو مفقود**

سيحتاج المسؤولون إلى السماح بالبرنامج النصي المخصص لتمكين ميزات القالب. للحصول على خطوات مفصلة، أمثلة واعتبارات انظر 

- [السماح بالبرنامج النصي المخصص أو منعه](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- موقع الحفظ كأمر قالب غير معتمد ويمكن أن يسبب مشاكل على المواقع التي تستخدم البنية التحتية لنشر خادم SharePoint.

**لا يمكن إنشاء قالب الموقع أو لا يعمل بشكل صحيح**

قد يفتقد القالب [ميزة](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) ولن يتم تنشيطه. إذا لم تكن الميزة متوفرة للتنشيط في مجموعة الموقع الحالية، لا يمكنك استخدام قالب الموقع لإنشاء موقع.

- تحقق لمعرفة ما إذا كانت أي قوائم أو مكتبات تتجاوز [حد عرض القائمة الحد الأدنى](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) من 5000 عنصر حيث يمكن حظر إنشاء قالب موقع.

- قد يستخدم الموقع موارد كثيرة جداً وبالتالي يتجاوز قالب الموقع حد 50 ميغابايت.


- هناك مشاكل في عرض البيانات من قائمة تستخدم عمود بحث. لمزيد من المعلومات، راجع [القائمة التي تم إنشاؤها بواسطة القالب لا تعرض البيانات من قائمة البحث الصحيحة في SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).

لمزيد من المعلومات التفصيلية حول المشاكل والحلول الشائعة، يرجى التحقق من [إنشاء واستخدام قوالب الموقع.](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)



