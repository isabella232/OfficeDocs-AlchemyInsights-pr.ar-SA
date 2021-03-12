---
title: استكشاف رسائل رفض الوصول وإصلاحها
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 3189fa61d28253569278024d4191ee63b917509f
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707941"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>استكشاف الأخطاء في الرسائل التي تم رفض الوصول إليها وإصلاحها في مركز إدارة Sharepoint/OneDrive

إذا كنت تتلقى رسالة رفض الوصول عند محاولة الاستعراض إلى مركز إدارة Sharepoint/OneDrive، فالرجاء التأكد من تعيين ترخيص [للمستخدم.](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users) إذا كان لدى المستخدم ترخيص، يجب أيضا [](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) التأكد من تعيين دور مسؤول له يمكنه الوصول إلى مراكز الإدارة.

يمكن أن تحدث هذه المشكلة أيضا عند حذف مستخدم ثم إعادة إنشائه بنفس اسم المستخدم الأساسي (UPN). يتم إنشاء الحساب الجديد باستخدام قيمة PUID مختلفة (الم ID الخاص ب جواز السفر). عندما يحاول المستخدم الوصول إلى مجموعة مواقع ويب أو OneDrive الخاص به، يكون لدى المستخدم PUID غير صحيح. يتضمن السيناريو الثاني مزامنة الدليل مع وحدة تنظيمية ل Active Directory (OU). إذا كان المستخدمون قد سبقوا الدخول إلى SharePoint، ثم تم نقلهم إلى OU آخر ثم إعادة مواصة مع SharePoint، فقد تواجههم هذه المشكلة.

لحل هذه المشكلة، يجب استعادة UPN الأصلي باستخدام الخطوات في المقالة، استعادة مستخدم [في Microsoft 365.](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user)

ملاحظة: إذا لم يتوفر مركز إدارة OneDrive أو SharePoint لمستخدمين متعددين سبق لهم الوصول إليه، فقد تكون هناك مشكلة مؤقتة في الخدمة.  [تحقق من لوحة معلومات "صحة الخدمة".](https://portal.office.com/adminportal/home#/servicehealth)


