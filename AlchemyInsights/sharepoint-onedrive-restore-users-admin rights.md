---
title: استكشاف الأخطاء في الرسائل التي تم رفض وصولها OneDrive for Business الوصول وإصلاحها
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: fc4a2bd7dcc74f5f05e8b709e4bc3eac6ed445d6e2ea9ede698abbc8667723ce
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53957780"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>استكشاف الأخطاء في الرسائل التي تم رفض وصولها OneDrive for Business الوصول وإصلاحها

تحدث هذه المشكلة بشكل متكرر عند حذف مستخدم ثم إعادة إنشائه بنفس اسم المستخدم الأساسي (UPN). يتم إنشاء الحساب الجديد باستخدام قيمة PUID (ID فريدة من جواز السفر) مختلفة. عندما يحاول المستخدم الوصول إلى مجموعة مواقع OneDrive، يكون لدى المستخدم PUID غير صحيح. يتضمن السيناريو الثاني مزامنة الدليل مع وحدة تنظيمية ل Active Directory (OU). إذا كان المستخدمون قد SharePoint الدخول، ثم تم نقلهم إلى OU آخر ثم إعادة موازة مع SharePoint، فقد تواجه هذه المشكلة.

1. لحل هذه المشكلة، يجب استعادة UPN الأصلي باستخدام الخطوات في المقالة، استعادة مستخدم [في Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).
2. إذا لم تتمكن من استعادة المستخدم الأصلي، يجب إزالة المستخدم القديم من موقع OneDrive باستخدام هذه الخطوات، إزالة مستخدم من [قائمة معلومات المستخدم](). 
3. بعد القيام بذلك، يمكنك التحقق من أن المستخدم لديه حقوق المسؤول في [](https://docs.microsoft.com/sharepoint/manage-user-profiles) موقع OneDrive من خلال اتباع الخطوات اللازمة لإضافة مسؤول لمستخدم OneDrive

لمزيد من المعلومات حول مستويات الأذونات، راجع المقالة فهم مستويات [الأذونات في SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
