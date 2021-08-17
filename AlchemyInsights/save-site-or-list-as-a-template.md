---
title: حفظ موقع أو قائمة كقالب
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 31cb294be6b72be313cf63ed5ed2af0ef041dcf6efb7a7a2af4e1b6a9a149c43
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54109191"
---
# <a name="save-site-or-list-as-a-template"></a>حفظ موقع أو قائمة كقالب

SharePoint قوالب المواقع هي تعريفات معنيه مسبقا تم تصميمها حول حاجة عمل معينة. لمزيد من المعلومات، راجع استخدام القوالب لإنشاء أنواع مختلفة من المواقع [SharePoint.](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4)

فيما يلي بعض المشاكل/الحلول الشائعة حول حفظ موقع أو قائمة كقالب في SharePoint Online.

**الزر "حفظ قالب الموقع/القائمة" غير متوفر أو مفقود.** 

- سيحتاج المسؤولون إلى السماح بالبرنامج النصي المخصص لتمكين ميزات القالب. للحصول على خطوات مفصلة، راجع الأمثلة والاعتبارات السماح بالنص النصي [المخصص أو منعه.](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)


- الأمر حفظ الموقع كقالب غير مدعوم ويمكن أن يسبب مشاكل في المواقع التي تستخدم البنية الأساسية للنشر في SharePoint Server.


**لا يمكن إنشاء قالب الموقع أو لا يعمل بشكل صحيح**

- قد يفتقد القالب إلى [ميزة](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) ولن يتم تنشيطه. إذا لم تكن الميزة متوفرة للتنشيط في مجموعة المواقع الحالية، فلا يمكنك استخدام قالب الموقع لإنشاء موقع.


- تحقق لمعرفة ما إذا كانت هناك [](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) أي قوائم أو مكتبات تتجاوز عتبة حد طريقة عرض القائمة وهو 5000 عنصر حيث يمكن أن يمنع ذلك إنشاء قالب موقع.


- قد يستخدم الموقع موارد كثيرة جدا، وبالتالي يتجاوز قالب الموقع الحد الأقصى وهو 50 ميغابايت.


- هناك مشاكل في عرض البيانات من قائمة تستخدم عمود البحث. لمزيد من المعلومات، راجع لا تعرض القائمة التي تم إنشاؤها بواسطة القالب البيانات من قائمة البحث الصحيحة في SharePoint [Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).


لمزيد من المعلومات المفصلة حول المشاكل والحلول الشائعة، الرجاء الرجوع [إلى إنشاء قوالب الموقع واستخدامها](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).

