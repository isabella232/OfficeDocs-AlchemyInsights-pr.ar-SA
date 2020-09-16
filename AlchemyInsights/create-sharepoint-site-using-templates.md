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
ms.openlocfilehash: b554bfa4ccccbd68d0c3df27cf17397f860735c2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47732198"
---
# <a name="create-sharepoint-sites-using-templates"></a>إنشاء مواقع SharePoint باستخدام القوالب

القدرة علي حفظ موقع كقالب غير معتمده مع الاتصال الحديث أو مواقع الفريق. للحصول علي مزيد من المعلومات حول استخدام القوالب [، راجع حفظ موقع SharePoint وتنزيله وتحميله كقالب](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).

اليك بعض المشاكل الشائعة/الحلول المتعلقة بحفظ موقع أو قائمه كقالب في Sharepoint Online. 

**الزر "حفظ قالب الموقع/القائمة" غير متوفر أو مفقود**

سيحتاج المسؤولون إلى السماح لبرنامج نصي مخصص بتمكين ميزات القالب. للاطلاع علي الخطوات التفصيلية والامثله والاعتبارات 

- [السماح بالبرامج النصية المخصصة أو منعها](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- الأمر "حفظ الموقع كقالب" غير معتمد وقد يؤدي إلى حدوث مشاكل في المواقع التي تستخدم البنية الاساسيه لنشر SharePoint Server.

**لا يمكن إنشاء قالب الموقع أو انه لا يعمل بشكل صحيح**

قد لا يحتوي القالب علي [ميزه](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) ولن يتم تنشيطها. إذا لم تكن الميزة متوفرة للتنشيط في مجموعه المواقع المشتركة الحالية ، فلا يمكنك استخدام قالب الموقع لإنشاء موقع.

- التحقق لمعرفه ما إذا كانت هناك اي قوائم أو مكتبات تتجاوز [عتبه حدود طريقه عرض القائمة](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) لعناصر 5000 بما انه بإمكانه حظر إنشاء قالب الموقع.

- قد يستخدم الموقع عددا كبيرا جدا من الموارد ، التالي فان قالب الموقع يتجاوز الحد الأقصى ل50.


- هناك مشاكل تعرض البيانات من قائمه تستخدم عمود بحث. لمزيد من المعلومات ، راجع [القائمة التي تم إنشاؤها بالقوالب لا تعرض البيانات من قائمه البحث الصحيحة في SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).

للحصول علي مزيد من المعلومات حول المشاكل والحلول الشائعة ، يرجى التحقق من [إنشاء قوالب الموقع واستخدامها](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).



