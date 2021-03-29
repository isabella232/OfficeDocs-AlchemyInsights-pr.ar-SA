---
title: سير العمل لا يبدأ
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
ms.openlocfilehash: e69f3e529e4a2202f641cb62f42b1a20d774a398
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403730"
---
# <a name="workflow-is-not-starting"></a>سير العمل لا يبدأ

- لم يبدأ سير عمل SharePoint 2010 و SharePoint 2013.

    - إذا لم يبدأ سير العمل الخاص بك، فقد تكون هناك مشكلة خدمة مؤقتة حيث قد تواجه المستخدمين تأخيرات متقطعة مع تقدم سير العمل. تحقق من [لوحة معلومات حالة الخدمة](https://admin.microsoft.com/AdminPortal/Home/servicehealth) لمعرفة ما إذا كانت مؤسستك متأثّر بها.

    - إذا مرت أكثر من 24 ساعة منذ أن رأيت هذه المشكلة للمرة الأولى، فالرجاء تسجيل تذكرة دعم. في العديد من الحالات، نحن نعمل بالفعل على إيجاد حل. الرجاء منحنا 24 ساعة على الأقل لإكمال الحل.

- تم تأخير مهام سير عمل SharePoint 2010 عند البدء.

    - يحدث هذا الأمر إذا تم تشغيل سير العمل على دفعات كبيرة. (على سبيل المثال، عند إضافة عناصر متعددة في الوقت نفسه).

    - لم يتم تصميم مهام سير العمل بحيث تعمل في الوقت الحقيقي، لذا فإن التأخير هو سلوك التصميم حسب التصميم.

   -  إذا كان سير العمل عبارة عن لغة تمييز كائن (XMOL) معقدة، يمكن أن تكون عملية التحويل البرمجي بطيئة. تحقق [من هذه](https://support.microsoft.com//kb/3043697) المقالة.

    - يجب تبسيط سير العمل أو إعادة تصميمه باستخدام نوع النظام الأساسي لسير عمل Microsoft SharePoint 2013.

    - إذا ازداد حجم محفوظات سير العمل، فقد ترغب في إزالة العناصر أو إنشاء قائمة محفوظات جديدة.

        مزيد من المعلومات : [إزالة محفوظات سير العمل](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)


## <a name="related-topics"></a>المواضيع ذات الصلة
هل تريد تجربة Microsoft Flow في SharePoint Online؟
- [إنشاء تدفق](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint وتدفق](https://flow.microsoft.com/blog/sharepoint-and-flow/) 
