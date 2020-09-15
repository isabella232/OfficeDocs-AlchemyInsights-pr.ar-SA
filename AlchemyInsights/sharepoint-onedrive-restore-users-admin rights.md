---
title: استكشاف أخطاء الوصول عبر البريد إلى مواقع OneDrive for Business وإصلاحها
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
ms.openlocfilehash: 9001cf0b7d9f1f05a2ecedca2c3137dd1b8a1c38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670603"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>استكشاف أخطاء الوصول عبر البريد إلى مواقع OneDrive for Business وإصلاحها

تحدث هذه المشكلة بشكل متكرر عند حذف مستخدم وأعاده إنشائه باستخدام الاسم الأساسي للمستخدم (UPN). يتم إنشاء الحساب الجديد باستخدام قيمه مختلفه لبويد (المعرف الفريد ل Passport). عندما يحاول المستخدم الوصول إلى مجموعه مواقع مشتركه أو من OneDrive ، فهذا يعني ان المستخدم لديه بويد غير صحيح. يتضمن السيناريو الثاني مزامنة الدليل مع الوحدة التنظيمية لخدمه Active Directory (OU). إذا قام المستخدمون بتسجيل الدخول إلى SharePoint بالفعل ، سيتم نقله إلى الوحدة التنظيمية والريسينسيد المختلفة مع SharePoint ، وقد يواجهوا هذه المشكلة.

1. لحل هذه المشكلة ، يجب استعاده النسخة الاصليه ل UPN باستخدام الخطوات الواردة في المقالة ، [استعاده مستخدم في Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).
2. إذا لم تتمكن من استعاده المستخدم الأصلي ، فيجب أزاله المستخدم القديم من موقع OneDrive باستخدام هذه الخطوات ، [وأزاله مستخدم من قائمه معلومات المستخدم](). 
3. بعد الانتهاء من ذلك ، يمكنك التحقق من ان المستخدم يملك حقوق المسؤول لموقع OneDrive عن طريق اتباع الخطوات [المتعلقة باضافه المسؤول لOneDrive الخاص بالمستخدم](https://docs.microsoft.com/sharepoint/manage-user-profiles)

للحصول علي مزيد من المعلومات حول مستويات الأذونات ، راجع المقالة [التعرف علي مستويات الأذونات في SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
