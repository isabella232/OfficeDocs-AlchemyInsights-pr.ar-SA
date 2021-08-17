---
title: إنشاء موقع في SharePoint Online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: eaf09aebad5568aab3a716ce28c8ce3357c9f43175e1b1458bfcd43fd95a71fa
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54057953"
---
# <a name="create-sharepoint-sites-using-templates"></a>إنشاء SharePoint جديدة باستخدام القوالب

القدرة على حفظ موقع كقالب غير مدعومة في وسائل الاتصال الحديثة أو مواقع الفريق. لمزيد من المعلومات حول استخدام القوالب، راجع [حفظ موقع SharePoint وتنزيله وتحميله كقالب](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).

فيما يلي بعض المشاكل/الحلول الشائعة المتعلقة حفظ موقع أو قائمة كقالب في Sharepoint Online. 

**الزر "حفظ قالب الموقع/القائمة" غير متوفر أو مفقود**

سيحتاج المسؤولون إلى السماح بالبرنامج النصي المخصص لتمكين ميزات القالب. للحصول على خطوات مفصلة، راجع الأمثلة والاعتبارات 

- [السماح بالبرنامج النصي المخصص أو منعه](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- الأمر حفظ الموقع كقالب غير مدعوم ويمكن أن يسبب مشاكل في المواقع التي تستخدم البنية الأساسية للنشر في SharePoint Server.

**لا يمكن إنشاء قالب الموقع أو لا يعمل بشكل صحيح**

قد يفتقد القالب إلى [ميزة](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) ولن يتم تنشيطه. إذا لم تكن الميزة متوفرة للتنشيط في مجموعة المواقع الحالية، فلا يمكنك استخدام قالب الموقع لإنشاء موقع.

- تحقق لمعرفة ما إذا كانت هناك [](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) أي قوائم أو مكتبات تتجاوز عتبة حد طريقة عرض القائمة وهو 5000 عنصر حيث يمكن أن يمنع ذلك إنشاء قالب موقع.

- قد يستخدم الموقع موارد كثيرة جدا، وبالتالي يتجاوز قالب الموقع الحد الأقصى وهو 50 مبايت.


- هناك مشاكل في عرض البيانات من قائمة تستخدم عمود البحث. لمزيد من المعلومات، راجع لا تعرض القائمة التي تم إنشاؤها بواسطة القالب البيانات من قائمة البحث الصحيحة في SharePoint [Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).

للحصول على مزيد من المعلومات المفصلة حول المشاكل والحلول الشائعة، يرجى التحقق [من إنشاء قوالب الموقع واستخدامها](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).



