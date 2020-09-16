---
title: حفظ الموقع أو القائمة كقالب
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 37ae727aa6dd6af94d0d833ce972aec413d90194
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727518"
---
# <a name="save-site-or-list-as-a-template"></a>حفظ الموقع أو القائمة كقالب

قوالب موقع SharePoint هي تعريفات منشاه مسبقا التي تم تصميمها حول احتياجات عمل معينه. لمزيد من المعلومات ، راجع [استخدام القوالب لإنشاء أنواع مختلفه من مواقع SharePoint](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).

اليك بعض المشاكل الشائعة/الحلول المتعلقة بحفظ موقع أو قائمه كقالب في SharePoint Online.

**الزر "حفظ قالب الموقع/القائمة" غير متوفر أو مفقود**. 

- سيحتاج المسؤولون إلى السماح لبرنامج نصي مخصص بتمكين ميزات القالب. للاطلاع علي الخطوات التفصيلية والامثله والاعتبارات ، راجع [السماح بالبرنامج النصي المخصص أو منعه](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).


- الأمر "حفظ الموقع كقالب" غير معتمد وقد يؤدي إلى حدوث مشاكل في المواقع التي تستخدم البنية الاساسيه لنشر SharePoint Server.


**لا يمكن إنشاء قالب الموقع أو انه لا يعمل بشكل صحيح**

- قد لا يحتوي القالب علي [ميزه](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) ولن يتم تنشيطها. إذا لم تكن الميزة متوفرة للتنشيط في مجموعه المواقع المشتركة الحالية ، فلا يمكنك استخدام قالب الموقع لإنشاء موقع.


- التحقق لمعرفه ما إذا كانت هناك اي قوائم أو مكتبات تتجاوز [عتبه حدود طريقه عرض القائمة](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) لعناصر 5000 بما انه بإمكانه حظر إنشاء قالب الموقع.


- قد يستخدم الموقع عددا كبيرا جدا من الموارد ، التالي فان قالب الموقع يتجاوز الحد الأقصى ل50 ميغابايت.


- هناك مشاكل تعرض البيانات من قائمه تستخدم عمود بحث. لمزيد من المعلومات ، راجع [القائمة التي تم إنشاؤها بالقوالب لا تعرض البيانات من قائمه البحث الصحيحة في SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).


للحصول علي مزيد من المعلومات حول المشاكل والحلول الشائعة ، يرجى الاشاره إلى [قوالب الموقع وإنشاءها واستخدامها](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).

