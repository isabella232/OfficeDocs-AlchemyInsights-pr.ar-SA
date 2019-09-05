---
title: إنشاء موقع في SharePoint على الإنترنت
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: 42430c8dadc17b87dc7741f3fa045ba7c25fab84
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/04/2019
ms.locfileid: "36755295"
---
# <a name="create-sharepoint-sites-using-templates"></a>إنشاء مواقع SharePoint باستخدام القوالب

قوالب موقع SharePoint هي تعريفات مصممة مسبقًا حول حاجة عمل معينة. لمزيد من المعلومات، راجع [استخدام القوالب لإنشاء أنواع مختلفة من مواقع SharePoint](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).

فيما يلي بعض المشكلات/الحلول الشائعة فيما يتعلق بحفظ موقع أو قائمة كقالب في Sharepoint عبر الإنترنت. 

**زر حفظ قالب الموقع/القائمة غير متوفر أو مفقود**

سيحتاج المسؤولون إلى السماح بالبرنامج النصي المخصص لتمكين ميزات القالب. للاطلاع على الخطوات التفصيلية والأمثلة والاعتبارات، انظر 

- [السماح بالبرنامج النصي المخصص أو منعه](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- الأمر حفظ الموقع كقالب غير معتمد ويمكن أن يسبب مشاكل على المواقع التي تستخدم بنية نشر خادم SharePoint.

**لا يمكن إنشاء قالب الموقع أو لا يعمل بشكل صحيح**

قد يفتقد القالب [ميزة](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) ولن يتم تنشيطه. إذا كانت الميزة غير متوفرة للتنشيط في مجموعة الموقع الحالية، لا يمكنك استخدام قالب الموقع لإنشاء موقع.

- تحقق لمعرفة ما إذا كانت أية قوائم أو مكتبات تتجاوز [عتبة حد عرض القائمة](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) للعناصر 5000 حيث أن هذا يمكن حظر إنشاء قالب موقع.

- قد يستخدم الموقع موارد كثيرة جداً وبالتالي يتجاوز قالب الموقع حد 50 ميغا بايت.


- توجد مشاكل في عرض البيانات من قائمة تستخدم عمود بحث. لمزيد من المعلومات، راجع [القائمة التي تم إنشاؤها بواسطة القالب لا تعرض البيانات من قائمة البحث الصحيحة في SharePoint على الإنترنت](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).

لمزيد من المعلومات التفصيلية حول المشاكل والحلول الشائعة، الرجاء مراجعة [إنشاء قوالب المواقع واستخدامها](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).



