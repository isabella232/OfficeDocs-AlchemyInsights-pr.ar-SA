---
title: استكشاف أخطاء الوصول إلى الرسائل التي تم رفضها
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 22f5966fdae563c44affb7d0447787a4ee0aca93
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47767631"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>استكشاف أخطاء الوصول إلى الرسائل التي تم رفضها في مركز أداره Sharepoint/OneDrive وإصلاحها

إذا تلقيت رسالة تفيد بأنه تم رفض الوصول عند محاولة الاستعراض إلى مركز أداره Sharepoint/OneDrive ، فالرجاء التاكد من [تعيين ترخيص للمستخدم](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users). إذا كان لدي المستخدم ترخيص ، فعليك أيضا التاكد من انه قد [تم تعيين دور مسؤول](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) له بحيث يمكنه الوصول إلى مراكز الاداره.

يمكن ان تحدث هذه المشكلة أيضا عند حذف مستخدم وأعاده إنشائه باستخدام الاسم الأساسي للمستخدم (UPN). يتم إنشاء الحساب الجديد باستخدام قيمه مختلفه لبويد (المعرف الفريد ل Passport). عندما يحاول المستخدم الوصول إلى مجموعه مواقع مشتركه أو من OneDrive ، فهذا يعني ان المستخدم لديه بويد غير صحيح. يتضمن السيناريو الثاني مزامنة الدليل مع الوحدة التنظيمية لخدمه Active Directory (OU). إذا قام المستخدمون بتسجيل الدخول إلى SharePoint بالفعل ، سيتم نقله إلى الوحدة التنظيمية والريسينسيد المختلفة مع SharePoint ، وقد يواجهوا هذه المشكلة.

لحل هذه المشكلة ، ينبغي عليك استعاده UPN الاصليه باستخدام الخطوات الواردة في المقالة ، [استعاده مستخدم في Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).

ملاحظه: إذا لم يكن مركز أداره OneDrive أو SharePoint متوفرا لعده مستخدمين لديهم حق الوصول ، فقد تكون هناك مشكله خدمه مؤقته.  [تحقق من لوحه معلومات حماية الخدمة](https://portal.office.com/adminportal/home#/servicehealth).


