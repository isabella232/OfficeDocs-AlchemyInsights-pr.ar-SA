---
title: إضافة مجموعة إلى موقع SharePoint
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: f0126f7f753275e9bbf8c3a09a6af5faf9a27862
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/07/2019
ms.locfileid: "34758718"
---
# <a name="create-group-connected-site-in-sharepoint-online"></a>إنشاء مجموعة موقع المتصلة في SharePoint عبر إنترنت

هناك اثنين من المشاكل الشائعة عند إنشاء أو إعادة إنشاء مجموعة الموقع متصلاً.

 إذا قمت بحذف مجموعة والمواقع المتصلة به وترغب في إنشاء موقع آخر باستخدام URL نفسه، سوف تحتاج إلى إزالة الموقع السابق.

تحميل [Shell إدارة مكتب التخطيط الاستراتيجي](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)

 لمزيد من المعلومات حول الشروع في العمل مع powershell، راجع [الشروع في استخدام SharePoint Shell إدارة الإنترنت](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)

إزالة الموقع من "المواقع المحذوفة" استخدام cmdlet powershell [إزالة سبوديليتيدسيتي](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) .

إذا كنت تقوم بإنشاء مجموعة موقع متصلة وتلقى تحذير مجموعة أخرى بنفس الاسم المستعار بالفعل، تحقق من مجموعات موجودة من [Office 365 من مركز الإدارة](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups). لحل هذه المشكلة أو حذف مجموعة موجودة إذا لم يعد مطلوباً أو إنشاء الموقع باستخدام اسم مستعار مختلف المعينة.

هناك طرق مختلفة لإنشاء واستخدام مجموعات الحديثة مع SharePoint.

يمكنك توصيل مواقع موجودة لمجموعة Office 365. لمزيد من المعلومات، راجع [الاتصال مجموعة Office 365 استخدام إينيتيرفيس المستخدم SharePoint](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).

لإنشاء موقع متصلة مجموعة Office 365، ستحتاج إلى إنشاء "موقع الفريق". لمزيد من المعلومات، راجع [إنشاء موقع فريق في SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).

