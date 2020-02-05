---
title: إنشاء موقع SharePoint
ms.author: pebaum
author: todmccoy
ms.audience: Admin
ms.topic: article
ms.collection: Adm_O365
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "5200004"
- "3911416"
- "1386"
- "2303"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: e1e71ae9401448ed18058f6307302dcbaf773649
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/04/2020
ms.locfileid: "41770842"
---
# <a name="create-a-sharepoint-site"></a>إنشاء موقع SharePoint

إنشاء مواقع من [المواقع النشطة](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) في مركز إدارة SharePoint أو إدارتها. لمزيد من المعلومات، راجع [إدارة المواقع في مركز مشرف SharePoint الجديد](https://docs.microsoft.com/sharepoint/manage-site-creation). 

## <a name="tips"></a>نصائح:

- **لا** يمكنك إنشاء موقع بنفس عنوان URL لموقع موجود. إذا قمت بحذف موقع وترغب في إعادة استخدام عنوان URL، فمن المحتمل أن يكون الموقع المحذوف لا يزال موجودًا ضمن [المواقع المحذوفة](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true). يجب حذف الموقع نهائيًا لإعادة استخدام عنوان URL. لإزالة موقع بالكامل باستخدام Powershell، راجع مثال [إزالة SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet.
- قد لا يتمكن بعض المستخدمين من إنشاء موقع. [راجع إدارة إنشاء الموقع في SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).
- من المحتمل أن يظهر الموقع **عالقًا** في إنشاء لفترة أطول من المتوقع. إذا مر أكثر من 24 ساعة منذ أن رأيت هذه المشكلة لأول مرة، يرجى تسجيل تذكرة دعم. في كثير من الحالات، نحن نعمل بالفعل على حل. يرجى تعطينا ما لا يقل عن 24 ساعة لإكمال الحل.
