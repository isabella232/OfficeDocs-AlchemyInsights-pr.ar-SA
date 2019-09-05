---
title: إضافة مجموعة إلى موقع SharePoint
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 423db4e5bbb85e75aee3548d5b6b46a64ebc6fa0
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/04/2019
ms.locfileid: "36750507"
---
# <a name="issues-when-creating-or-group-connected-sites-in-sharepoint-online"></a>المشكلات عند إنشاء أو تجميع المواقع المتصلة في SharePoint على الإنترنت

هناك عدد من المشكلات الشائعة التي تمت مواجهتها عند إنشاء موقع متصل بالمجموعة أو إعادة إنشائه.

 إذا حذفت مجموعة وموقعها المتصل وترغب في إنشاء موقع آخر بنفس عنوان URL، فستحتاج إلى إزالة الموقع السابق نهائيًا.

تحميل [SPO إدارة شل](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)

 لمزيد من المعلومات حول الشروع في العمل باستخدام powershell، راجع [الشروع في العمل باستخدام SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)

إزالة الموقع من المواقع المحذوفة باستخدام cmdlet powershell [إزالة SPODeletedSite.](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)

إذا كنت تقوم بإنشاء موقع متصل بمجموعة وتتلقى تحذيرًا، توجد بالفعل مجموعة أخرى بنفس الاسم المستعار، فتحقق من المجموعات الموجودة من [Office 365 من مركز المسؤول](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups). لحل هذه المشكلة، احذف المجموعة الموجودة إذا لم تعد هناك حاجة إليها أو قم بإنشاء الموقع باسم مستعار مختلف تم تعيينه.

هناك طرق مختلفة لإنشاء واستخدام المجموعات الحديثة مع SharePoint.

يمكنك توصيل المواقع الموجودة بمجموعة Office 365. لمزيد من المعلومات، راجع [توصيل مجموعة Office 365 باستخدام مستخدم SharePoint ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).

لإنشاء موقع متصل بمجموعة Office 365، ستحتاج إلى إنشاء موقع فريق. لمزيد من المعلومات، راجع [إنشاء موقع فريق في SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).

