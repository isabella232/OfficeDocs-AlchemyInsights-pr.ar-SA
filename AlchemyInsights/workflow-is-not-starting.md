---
title: لم يبدأ سير العمل
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: 941e6349c98278a1a8cdac77457ec1cc72cdef8b
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766084"
---
# <a name="workflow-is-not-starting"></a>لم يبدأ سير العمل

- لم يتم بدء سير عمل SharePoint 2010 و SharePoint 2013.

    - إذا لم يبدأ سير العمل، فقد تكون هناك مشكلة خدمة مؤقتة حيث قد يواجه المستخدمون تأخيرات متقطعة مع تقدم سير العمل. تحقق من [لوحة معلومات صحة الخدمة](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) لمعرفة ما إذا كانت مؤسستك متأثرة.

    - إذا مرت أكثر من 24 ساعة منذ أن رأيت هذه المشكلة لأول مرة، يرجى تسجيل تذكرة دعم. في كثير من الحالات، نحن نعمل بالفعل على حل. يرجى من خلالنا أن تعطينا 24 ساعة على الأقل لإكمال الحل.

- تأخر سير عمل SharePoint 2010 في البداية.

    - يحدث هذا إذا تم تشغيل سير العمل على دفعات كبيرة. (على سبيل المثال، عند إضافة عدة عناصر في وقت واحد).

    - لم يتم تصميم مهام سير العمل لتشغيلها في الوقت الفعلي، لذلك فإن التأخير هو سلوك حسب التصميم.

   -  إذا كان سير العمل هو لغة ترميز كائن قابلة للتوسعة المعقدة (XMOL)، يمكن أن يكون التحويل البرمجي بطيئاً. تحقق من [هذه](https://support.microsoft.com//kb/3043697) المقالة.

    - يجب تبسيط سير العمل أو إعادة تصميمه باستخدام نوع نظام Microsoft SharePoint 2013 الأساسي لسير العمل.

    - إذا كان سجل سير العمل الخاص بك قد نما بشكل كبير، فقد تحتاج إلى تطهير العناصر أو إنشاء قائمة محفوظات جديدة.

        مزيد من المعلومات : [تطهير محفوظات سير العمل](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)


## <a name="related-topics"></a>المواضيع ذات الصلة
هل تريد تجربة Microsoft Flow في SharePoint Online؟
- [إنشاء تدفق](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint والتدفق](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


