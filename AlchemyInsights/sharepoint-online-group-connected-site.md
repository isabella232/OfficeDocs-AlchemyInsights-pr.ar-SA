---
title: إضافة مجموعة إلى موقع SharePoint
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 8ef33cbd44b01deaf0e45813d019f7696ef5def0
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/27/2020
ms.locfileid: "43912953"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a>مشكلات عند إنشاء موقع متصل بمجموعة في SharePoint

1. بعض المشكلات الشائعة التي تمت مواجهتها عند إنشاء موقع متصل بمجموعة أو إعادة إنشائه.
إذا حذفت مجموعة وموقعها المتصل وترغب في إنشاء موقع آخر بنفس عنوان URL، فستحتاج إلى إزالة الموقع السابق نهائيًا.

   - تحميل [SPO إدارة شل](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)
   - لمزيد من المعلومات حول البدء باستخدام Powershell، راجع [البدء باستخدام SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).
   - قم بإزالة الموقع من المواقع المحذوفة باستخدام [cmdlet إزالة SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell. Powershell مطلوب لحذف مواقع المجموعة بشكل دائم.

1. إذا كنت تقوم بإنشاء موقع متصل بمجموعة وتلقي تحذير: **توجد بالفعل مجموعة أخرى بنفس الاسم المستعار،** فتحقق من المجموعات الموجودة من مركز إدارة Microsoft [365](https://admin.microsoft.com/AdminPortal/Home#/groups). لحل المشكلة، احذف المجموعة الموجودة إذا لم تعد هناك حاجة إليها أو قم بإنشاء الموقع باسم مستعار مختلف معين.

1. هناك طرق مختلفة لإنشاء واستخدام المجموعات الحديثة مع SharePoint.

   - يمكنك توصيل المواقع الموجودة بمجموعة Microsoft 365. لمزيد من المعلومات، راجع [توصيل مجموعة Microsoft 365 باستخدام واجهة مستخدم SharePoint](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).
   - لإنشاء موقع متصل بمجموعة Microsoft 365، ستحتاج إلى إنشاء [موقع فريق](https://admin.microsoft.com/sharepoint).
