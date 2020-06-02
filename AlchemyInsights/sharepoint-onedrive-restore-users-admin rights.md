---
title: استكشاف الأخطاء وإصلاحها الوصول رفض الرسائل إلى مواقع OneDrive للأعمال
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 95bd46e8b7a6006f3735612d9a5602fb2b2a283b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511171"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>استكشاف الأخطاء وإصلاحها الوصول رفض الرسائل إلى مواقع OneDrive للأعمال

تحدث هذه المشكلة بشكل متكرر عند حذف مستخدم وإعادة إنشائه بنفس اسم المستخدم الرئيسي (UPN). يتم إنشاء الحساب الجديد باستخدام قيمة PUID مختلفة (معرف فريد من جواز السفر). عندما يحاول المستخدم الوصول إلى مجموعة موقع أو OneDrive الخاص بهم، يكون لدى المستخدم PUID غير صحيح. يتضمن سيناريو الثاني مزامنة الدليل مع وحدة تنظيمية "الدليل النشط" (OU). إذا قام المستخدمون بتسجيل الدخول بالفعل إلى SharePoint، ثم تم نقلهم إلى OU مختلف وإعادة مزامنتهم مع SharePoint، فقد يواجهون هذه المشكلة.

1. لحل هذه المشكلة يجب استعادة UPN الأصلي مع الخطوات في المقالة استعادة [مستخدم في Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).
2. إذا لم تتمكن من استعادة المستخدم الأصلي يجب إزالة المستخدم القديم من موقع OneDrive باستخدام هذه الخطوات، [قم بإزالة مستخدم من قائمة معلومات المستخدم](). 
3. بعد الانتهاء من ذلك، يمكنك التحقق من أن المستخدم لديه حقوق المسؤول إلى موقع OneDrive باتباع الخطوات لإضافة [المسؤول لـ OneDrive للمستخدم](https://docs.microsoft.com/sharepoint/manage-user-profiles)

لمزيد من المعلومات حول مستويات الأذونات، راجع المقالة، [فهم مستويات الأذونات في SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
