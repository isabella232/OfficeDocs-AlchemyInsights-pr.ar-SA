---
title: استكشاف الأخطاء في الرسائل التي تم رفض الوصول إليها وإصلاحها
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 9acde72f82a27c9f2faa2cf4d0417374aa5a294234da96080dc0498d07639248
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54085215"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>استكشاف الأخطاء في الرسائل التي تم رفض الوصول إليها في مركز إدارة Sharepoint/OneDrive وإصلاحها

إذا كنت تتلقى رسالة رفض الوصول عند محاولة الاستعراض إلى مركز إدارة Sharepoint/OneDrive، فالرجاء التأكد من تعيين ترخيص [للمستخدم](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users). إذا كان لدى المستخدم ترخيص، يجب أيضا [](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) التأكد من تعيين دور مسؤول له يمكنه الوصول إلى مراكز الإدارة.

يمكن أن تحدث هذه المشكلة أيضا عند حذف مستخدم ثم إعادة إنشائه بنفس اسم المستخدم الأساسي (UPN). يتم إنشاء الحساب الجديد باستخدام قيمة PUID (ID فريدة من جواز السفر) مختلفة. عندما يحاول المستخدم الوصول إلى مجموعة مواقع OneDrive، يكون لدى المستخدم PUID غير صحيح. يتضمن السيناريو الثاني مزامنة الدليل مع وحدة تنظيمية ل Active Directory (OU). إذا كان المستخدمون قد SharePoint الدخول، ثم تم نقلهم إلى OU آخر ثم إعادة موازة مع SharePoint، فقد تواجه هذه المشكلة.

لحل هذه المشكلة، يجب استعادة UPN الأصلي باستخدام الخطوات في المقالة، استعادة مستخدم [في Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).

ملاحظة: إذا لم OneDrive أو SharePoint مركز الإدارة لعدة مستخدمين سبق لهم الوصول إليه، فقد تكون هناك مشكلة مؤقتة في الخدمة.  [تحقق من لوحة معلومات "صحة الخدمة".](https://portal.office.com/adminportal/home#/servicehealth)


