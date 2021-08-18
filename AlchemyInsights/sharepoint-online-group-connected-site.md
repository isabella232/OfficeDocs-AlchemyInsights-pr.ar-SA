---
title: إضافة مجموعة إلى موقع SharePoint ويب
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200004"
- "5766"
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 5dd159b8b9e141c2fb448bae5fb624efe1014d7d
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/13/2021
ms.locfileid: "58318111"
---
# <a name="common-issues-when-creating-a-group-connected-site-in-sharepoint"></a>المشاكل الشائعة عند إنشاء موقع متصل بالمجموعة في SharePoint

1. إذا قمت بحذف مجموعة لموقعها المتصل وترغب في إنشاء موقع آخر بنفس عنوان URL، ستحتاج إلى إزالة الموقع السابق بشكل دائم.

   - تنزيل [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)
   - لمزيد من المعلومات حول بدء باستخدام Powershell، راجع بدء SharePoint [Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).
   - قم بإزالة الموقع من المواقع المحذوفة باستخدام [الأمر cmdlet Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell. Powershell مطلوب لحذف مواقع المجموعات بشكل دائم.

1. إذا كنت تقوم بإنشاء موقع متصل بالمجموعة وتلقيت **تحذيرا:** توجد مجموعة أخرى بنفس الاسم المستعار بالفعل ، فتحقق من المجموعات الموجودة من [مركز مسؤولي Microsoft 365](https://admin.microsoft.com/AdminPortal/Home#/groups). لحل هذه المشكلة، احذف المجموعة الموجودة إذا لم تعد هناك حاجة إليها أو قم بإنشاء الموقع باستخدام اسم مستعار مختلف تم تعيينه.

1. هناك طرق مختلفة لإنشاء المجموعات الحديثة واستخدامها مع SharePoint.

   - يمكنك توصيل المواقع الموجودة إلى مجموعة Microsoft 365 أخرى. لمزيد من المعلومات، راجع الاتصال [مجموعة Microsoft 365 باستخدام SharePoint المستخدم.](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface)
   - لإنشاء موقع Microsoft 365 متصل بالمجموعة، ستحتاج إلى إنشاء [موقع فريق](https://admin.microsoft.com/sharepoint).
