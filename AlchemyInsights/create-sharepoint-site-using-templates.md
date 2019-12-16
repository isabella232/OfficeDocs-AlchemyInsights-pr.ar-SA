---
title: إنشاء موقع في SharePoint علي الإنترنت
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
ms.openlocfilehash: 458990889d3c074820527982cbfa6e2d198d3e66
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/15/2019
ms.locfileid: "40052456"
---
# <a name="create-sharepoint-sites-using-templates"></a>إنشاء مواقع SharePoint باستخدام القوالب

قوالب موقع SharePoint هي تعريفات تم بناؤها مسبقا مصممه حول حاجه عمل معينه. لمزيد من المعلومات ، راجع [استخدام قوالب لإنشاء أنواع مختلفه من مواقع SharePoint](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).

فيما يلي بعض المشكلات/الحلول الشائعة المتعلقة بحفظ موقع أو قائمه كقالب في Sharepoint Online. 

**زر حفظ قالب الموقع/القائمة غير متوفر أو مفقود**

سيحتاج المسؤولون إلى السماح بالبرنامج النصي المخصص لتمكين ميزات القالب. وللاطلاع علي الخطوات التفصيلية ، انظر الامثله والاعتبارات 

- [السماح بالبرنامج النصي المخصص أو منعه](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- الأمر حفظ الموقع كقالب غير معتمد ويمكن ان يسبب مشاكل علي المواقع التي تستخدم البنية الاساسيه للنشر خادم SharePoint.

**لا يمكن إنشاء قالب الموقع أو لا يعمل بشكل صحيح**

قد يفتقد القالب [ميزه](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) ولن يتم تنشيطه. إذا كانت الميزة غير متوفرة للتنشيط في مجموعه الموقع الحالية ، لا يمكنك استخدام قالب الموقع لإنشاء موقع.

- تحقق لمعرفه ما إذا كانت إيه قوائم أو مكتبات تتجاوز [عتبه حد عرض القائمة](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) للعناصر 5000 لان هذا يمكن ان يمنع إنشاء قالب موقع.

- قد يستخدم الموقع موارد كثيره جدا التالي يتجاوز قالب الموقع حد 50 ميغابايت.


- هناك مشاكل في عرض البيانات من قائمه تستخدم عمود بحث. لمزيد من المعلومات ، راجع [القائمة التي تم إنشاؤها بالقالب لا تعرض البيانات من قائمه البحث الصحيحة في SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).

للحصول علي معلومات أكثر تفصيلا حول المشاكل والحلول الشائعة ، الرجاء التحقق من [إنشاء قوالب الموقع واستخدامها](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).



