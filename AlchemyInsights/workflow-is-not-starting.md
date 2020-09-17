---
title: لا يتم بدء سير العمل
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: e3b8777ed74b812b31338784999eea43a95d3456
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47794754"
---
# <a name="workflow-is-not-starting"></a>لا يتم بدء سير العمل

- لا يتم بدء تشغيل مهام سير عمل SharePoint 2010 و SharePoint 2013.

    - إذا لم يتم بدء تشغيل سير العمل الخاص بك ، فقد يكون هناك مشكله خدمه مؤقته حيث يواجه المستخدمون تاخيرات متقطعه مع تقدم سير العمل. راجع [لوحه معلومات حماية الخدمة](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) لمعرفه ما إذا كانت مؤسستك متاثره بالأمر.

    - إذا تم تمرير أكثر من 24 ساعة منذ المرة الاولي التي قمت فيها بمشاهده هذه المشكلة ، يرجى تسجيل تذكره دعم. في حالات كثيره ، نحن نعمل بالفعل علي حل. يرجى تقديم 24 ساعة علي الأقل لإكمال حل.

- تم تاخير مهام سير عمل SharePoint 2010 في البداية.

    - يحدث هذا إذا تم تشغيل سير العمل في دفعات كبيره. (علي سبيل المثال ، عند أضافه عناصر متعددة في وقت واحد).

    - لا يتم تصميم مهام سير العمل ليتم تشغيلها في الوقت الحقيقي ، التالي فان التاخير هو السلوك بالتصميم.

   -  إذا كان سير العمل عبارة عن لغة تمييز معقده للعناصر (إكسمول) ، فقد يكون التحويل البرمجي بطيئا. راجع [هذه](https://support.microsoft.com//kb/3043697) المقالة.

    - ينبغي عليك تبسيط سير العمل أو أعاده تصميمه باستخدام نوع النظام الأساسي لسير العمل Microsoft SharePoint 2013.

    - إذا كانت محفوظات سير العمل كبيره جدا ، فقد ترغب في أزاله العناصر أو إنشاء قائمه محفوظات جديده.

        مزيد من المعلومات: [أزاله محفوظات سير العمل](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)


## <a name="related-topics"></a>المواضيع ذات الصلة
هل تريد تجربه Microsoft تدفق في SharePoint Online ؟
- [إنشاء تدفق](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint والتدفق](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


