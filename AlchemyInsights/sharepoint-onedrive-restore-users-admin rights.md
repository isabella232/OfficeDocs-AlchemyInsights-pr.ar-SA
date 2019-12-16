---
title: استكشاف أخطاء الوصول وإصلاحها رفض الرسائل إلى اندريف لمواقع العمل
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 9d8aba4e53a1e0505a430296bb1c11713ea2ce7b
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051592"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>استكشاف أخطاء الوصول وإصلاحها رفض الرسائل إلى اندريف لمواقع العمل

تحدث هذه المشكلة بشكل متكرر عند حذف مستخدم وأعاده إنشائه بنفس الاسم الأساسي للمستخدم (UPN). يتم إنشاء الحساب الجديد باستخدام قيمه PUID (معرف فريد لPassport) مختلفه. عندما يحاول المستخدم الوصول إلى مجموعه موقع أو اندريف الخاصة بهم ، المستخدم لديه PUID غير صحيحه. يتضمن السيناريو الثاني مزامنة الدليل مع الوحدة التنظيمية "Active Directory" (OU). إذا كان المستخدمون بالفعل تسجيل الدخول إلى SharePoint ، ومن ثم يتم نقلها إلى OU مختلفه resynced مع SharePoint ، فانها قد تواجه هذه المشكلة.

1. لحل هذه المشكلة يجب استعاده UPN الأصلي مع الخطوات التالية في المقالة ، [استعاده مستخدم في Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).
2. إذا كان لا يمكنك استعاده المستخدم الأصلي يجب أزاله المستخدم القديم من موقع اندريف باستخدام هذه الخطوات [أزاله مستخدم من قائمه معلومات المستخدم](). 
3. بعد الانتهاء من ذلك ، يمكنك التحقق من ان المستخدم لديه حقوق المسؤول إلى موقع اندريف باتباع الخطوات التالية [لأضافه المسؤول لاندريف المستخدم](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)

لمزيد من المعلومات حول مستويات الأذونات ، راجع المقالة ، [فهم مستويات الأذونات في SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
