---
title: أضافه مجموعه إلى موقع SharePoint
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
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/18/2019
ms.locfileid: "36750507"
---
# <a name="issues-when-creating-or-group-connected-sites-in-sharepoint-online"></a>المشكلات عند إنشاء أو تجميع المواقع المتصلة في SharePoint علي الإنترنت

هناك بعض المشكلات الشائعة التي تمت مواجهتها عند إنشاء أو أعاده إنشاء موقع متصل بالمجموعة.

 إذا قمت بحذف مجموعه وموقعها المتصل وترغب في إنشاء موقع آخر بنفس عنوان URL ، ستحتاج إلى أزاله الموقع السابق بشكل دائم.

تحميل [أداره البرامج الاستراتيجي شل](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)

 لمزيد من المعلومات حول الشروع في التشغيل مع powershell ، راجع الشروع [في التشغيل باستخدام Shell أداره SharePoint علي الإنترنت](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)

أزاله الموقع من المواقع المحذوفة باستخدام cmdlet powershell [أزاله سبوديليدموقع](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) .

إذا كنت تقوم بإنشاء موقع متصل بمجموعه وتتلقي تحذيرا توجد مجموعه أخرى بنفس الاسم المستعار بالفعل ، تحقق من المجموعات الموجودة من [Office 365 من مركز الاداره](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups). لحل هذه المشكلة ، احذف المجموعة الموجودة إذا لم تعد هناك حاجه اليها أو قم بإنشاء الموقع باسم مستعار مختلف معين.

هناك طرق مختلفه لإنشاء واستخدام المجموعات الحديثة مع SharePoint.

يمكنك توصيل المواقع الموجودة إلى مجموعه 365 Office. لمزيد من المعلومات ، راجع [توصيل مجموعه 365 Office باستخدام الواجهة المستخدمة ل SharePoint](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).

لإنشاء موقع متصل بمجموعه Office 365 ، ستحتاج إلى إنشاء موقع فريق. لمزيد من المعلومات ، راجع [إنشاء موقع فريق في SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).

