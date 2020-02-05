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
ms.openlocfilehash: e7bfabe1555bb94e915f8544d460deecce6171be
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/04/2020
ms.locfileid: "41770338"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a>المشكلات عند إنشاء موقع متصل بمجموعة في SharePoint

1. تواجه بعض المشكلات الشائعة عند إنشاء موقع متصل بمجموعة أو إعادة إنشائه.
إذا قمت بحذف مجموعة وموقعمتصل بها وترغب في إنشاء موقع آخر بنفس عنوان URL، فستحتاج إلى إزالة الموقع السابق نهائيًا.

   - تحميل [SPO إدارة شل](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)
   - لمزيد من المعلومات حول البدء باستخدام Powershell، راجع [البدء باستخدام SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).
   - إزالة الموقع من المواقع المحذوفة باستخدام [إزالة-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell cmdlet. مطلوب Powershell لحذف مواقع المجموعة بشكل دائم.

1. إذا كنت تقوم بإنشاء موقع متصل بمجموعة وتتلقى تحذيرًا: **توجد بالفعل مجموعة أخرى تحمل نفس الاسم المستعار**، فتحقق من المجموعات الموجودة من Office [365 من مركز الإدارة](https://admin.microsoft.com/AdminPortal/Home#/groups). لحل المشكلة، احذف المجموعة الموجودة إذا لم تعد هناك حاجة إليها أو قم بإنشاء الموقع باسم مستعار مختلف معين.

1. هناك طرق مختلفة لإنشاء واستخدام المجموعات الحديثة باستخدام SharePoint.

   - يمكنك توصيل المواقع الموجودة بمجموعة Office 365. لمزيد من المعلومات، راجع [توصيل مجموعة Office 365 باستخدام واجهة مستخدم SharePoint](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).
   - لإنشاء موقع متصل بمجموعة Office 365، ستحتاج إلى إنشاء [موقع فريق](https://admin.microsoft.com/sharepoint).
