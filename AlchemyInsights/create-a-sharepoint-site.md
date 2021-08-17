---
title: إنشاء موقع SharePoint ويب
ms.author: pebaum
author: pebaum
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.collection: Adm_O365
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "5200004"
- "3911416"
- "1386"
- "2303"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: bf9380727fff415357884a5122e633f2254337d3db50e2b8656d94938f76d394
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54080877"
---
# <a name="create-a-sharepoint-site"></a>إنشاء موقع SharePoint ويب

يمكنك إنشاء مواقع أو إدارتها من [المواقع النشطة](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) في SharePoint الإدارة. لمزيد من المعلومات، راجع إدارة المواقع في مركز إدارة SharePoint [الجديد.](https://docs.microsoft.com/sharepoint/manage-site-creation) 

## <a name="tips"></a>تلميحات:

- لا **يمكنك** إنشاء موقع باستخدام عنوان URL نفسه لموقع موجود. إذا قمت بحذف موقع ورغبت في إعادة استخدام عنوان URL، فمن المحتمل أن يكون الموقع المحذوف لا يزال موجودا ضمن [المواقع المحذوفة](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true). يجب حذف الموقع بشكل دائم لإعادة استخدام عنوان URL. لإزالة موقع بالكامل باستخدام Powershell، راجع مثال [cmdlet Remove-SPSite.](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site)
- قد لا يتمكن بعض المستخدمين من إنشاء موقع. [راجع إدارة إنشاء الموقع في SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).
- من المحتمل أن يظهر الموقع عالقا عند **إنشاء** مدة أطول من المتوقع. إذا مرت أكثر من 24 ساعة منذ أن رأيت هذه المشكلة للمرة الأولى، فالرجاء تسجيل تذكرة دعم. في العديد من الحالات، نحن نعمل بالفعل على إيجاد حل. الرجاء منحنا 24 ساعة على الأقل لإكمال الحل.
