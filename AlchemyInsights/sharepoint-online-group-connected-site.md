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
ms.openlocfilehash: 352bad1b8fe219f95a37c9ac268c6c4dd8801dfc
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/04/2019
ms.locfileid: "34719469"
---
# <a name="create-group-connected-site-in-sharepoint-online"></a>إنشاء مجموعة موقع المتصلة في SharePoint عبر إنترنت

<p><strong>هناك اثنين من المشاكل الشائعة عند إنشاء أو إعادة إنشاء مجموعة الموقع متصلاً.&nbsp;</strong></p>  <p>1.إذا قمت بحذف مجموعة والمواقع المتصلة به وترغب في إنشاء موقع آخر باستخدام URL نفسه، سوف تحتاج إلى إزالة الموقع السابق.</p>  <ul>  <li>تنزيل <a title="Shell إدارة مكتب التخطيط الاستراتيجي" href="https://support.office.com/en-ie/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429">Shell إدارة مكتب التخطيط الاستراتيجي</a> - للحصول على مزيد من المعلومات حول الشروع في العمل مع powershell، راجع <a title="الشروع في SharePoint Shell إدارة الإنترنت" href="https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps">الشروع في العمل مع "إدارة SharePoint على الإنترنت شل"</a>. <br /><br /></li>  <li>إزالة الموقع من "مواقع حذف" تستخدم <a title="سبوديليتيدسيتي إزالة" href="https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps">إزالة سبوديليتيدسيتي</a> powershell cmdlet.</li>  </ul>  <p>إذا كنت تقوم بإنشاء مجموعة موقع متصلة وتلقى تحذير <strong>'مجموعة أخرى بنفس الاسم المستعار للفعل موجود'</strong>، تحقق من مجموعات موجودة من <a title="Office 365 من مركز الإدارة" href="https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups">Office 365 من مركز إدارة</a>. لحل هذه المشكلة أو حذف مجموعة موجودة إذا لم يعد مطلوباً أو إنشاء الموقع باستخدام اسم مستعار مختلف المعينة.&nbsp;</p>  <p><strong>هناك طرق مختلفة لإنشاء واستخدام مجموعات الحديثة مع SharePoint.&nbsp;</strong></p>  <ol>  <li>يمكنك توصيل مواقع موجودة لمجموعة Office 365. لمزيد من المعلومات، راجع <a title="مجموعة Office 365 إينيتيرفيس المستخدم SharePoint باستخدام الاتصال" href="https://docs.microsoft.com/en-us/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface">مجموعة Office 365 إينيتيرفيس المستخدم SharePoint باستخدام الاتصال</a>.</li>  <li>لإنشاء موقع متصلة مجموعة Office 365، ستحتاج إلى إنشاء "موقع الفريق". لمزيد من المعلومات، راجع <a title="إنشاء موقع فريق في SharePoint" href="https://support.office.com/en-us/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d">إنشاء موقع فريق في SharePoint.</a></li>  </ol>

