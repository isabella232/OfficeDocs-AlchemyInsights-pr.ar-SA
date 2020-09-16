---
title: أضافه مجموعه إلى موقع SharePoint
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
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 9bec2f71465e43e1c3cba038e0e68949672ceb8a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771186"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a>مشاكل عند إنشاء موقع متصل بمجموعه في SharePoint

1. واجهت بعض المشاكل الشائعة عند إنشاء موقع المجموعة المتصلة أو أعاده إنشائه.
إذا قمت بحذف مجموعه وموقعها المتصل وترغب في إنشاء موقع آخر باستخدام عنوان URL نفسه ، ستحتاج إلى أزاله الموقع السابق بشكل دائم.

   - تنزيل [Shell لأداره SPO](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)
   - للحصول علي مزيد من المعلومات حول بدء استخدام Powershell ، راجع [بدء استخدام SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).
   - أزاله الموقع من المواقع [المحذوفة](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) باستخدام الأمرين سبوديليتيدسيتي Powershell cmdlet. يجب ان تحذف Powershell مواقع المجموعات بشكل دائم.

1. إذا كنت تقوم بإنشاء موقع متصل بالمجموعة وتلقيت تحذيرا: **هناك مجموعه أخرى تحمل نفس الاسم المستعار موجودة بالفعل**، فتحقق من المجموعات الموجودة من [مركز أداره Microsoft 365](https://admin.microsoft.com/AdminPortal/Home#/groups). لحل هذه المشكلة ، احذف المجموعة الموجودة إذا لم تعد بحاجه اليها أو أنشئ الموقع باسم مستعار مختلف معين.

1. هناك طرق مختلفه لإنشاء المجموعات الحديثة واستخدامها مع SharePoint.

   - يمكنك توصيل مواقع موجودة بمجموعه Microsoft 365. لمزيد من المعلومات ، راجع [الاتصال بمجموعه Microsoft 365 باستخدام واجهه مستخدم SharePoint](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).
   - لإنشاء موقع Microsoft 365 المتصل بالمجموعة ، ستحتاج إلى إنشاء [موقع فريق](https://admin.microsoft.com/sharepoint).
