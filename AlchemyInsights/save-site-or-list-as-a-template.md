---
title: حفظ الموقع أو القائمة كقالب
ms.author: pebaum
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 1fe0a2f5bf65ef4e8cabf3d05a701c8eff966435
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/04/2019
ms.locfileid: "36752019"
---
# <a name="save-site-or-list-as-a-template"></a>حفظ الموقع أو القائمة كقالب

قوالب موقع SharePoint هي تعريفات مصممة مسبقًا حول حاجة عمل معينة. لمزيد من المعلومات، راجع [استخدام القوالب لإنشاء أنواع مختلفة من مواقع SharePoint](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).

فيما يلي بعض المشكلات/الحلول الشائعة فيما يتعلق بحفظ موقع أو قائمة كقالب في SharePoint على الإنترنت.

**زر حفظ قالب الموقع/القائمة غير متوفر أو مفقود**. 

- سيحتاج المسؤولون إلى السماح بالبرنامج النصي المخصص لتمكين ميزات القالب. للحصول على خطوات تفصيلية وأمثلة واعتبارات راجع [السماح بالبرنامج النصي المخصص أو منعه](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).


- الأمر حفظ الموقع كقالب غير معتمد ويمكن أن يسبب مشاكل على المواقع التي تستخدم بنية نشر خادم SharePoint.


**لا يمكن إنشاء قالب الموقع أو لا يعمل بشكل صحيح**

- قد يفتقد القالب [ميزة](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) ولن يتم تنشيطه. إذا كانت الميزة غير متوفرة للتنشيط في مجموعة الموقع الحالية، لا يمكنك استخدام قالب الموقع لإنشاء موقع.


- تحقق لمعرفة ما إذا كانت أية قوائم أو مكتبات تتجاوز [عتبة حد عرض القائمة](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) للعناصر 5000 حيث أن هذا يمكن حظر إنشاء قالب موقع.


- قد يستخدم الموقع موارد كثيرة جداً وبالتالي يتجاوز قالب الموقع حد 50 ميغابايت (MB).


- توجد مشاكل في عرض البيانات من قائمة تستخدم عمود بحث. لمزيد من المعلومات، راجع [القائمة التي تم إنشاؤها بواسطة القالب لا تعرض البيانات من قائمة البحث الصحيحة في SharePoint على الإنترنت](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).


لمزيد من المعلومات التفصيلية حول المشاكل والحلول الشائعة يرجى الرجوع إليها، [إنشاء واستخدام قوالب الموقع](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).

