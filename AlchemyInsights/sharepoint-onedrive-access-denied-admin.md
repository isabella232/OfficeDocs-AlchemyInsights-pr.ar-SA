---
title: استكشاف أخطاء رسائل "رفض الوصول" وإصلاحها
ms.author: pebaum
author: pebaum
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 57919e6dbd81a5bf3b17fb067485e8eec23b7d4c
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051412"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>استكشاف أخطاء رسائل "رفض الوصول" في مركز مسؤول Sharepoint/اندريف وإصلاحها

إذا كنت تتلقي رسالة رفض وصول عند محاولة الاستعراض إلى مركز مسؤول Sharepoint/اندريف ، الرجاء التاكد من [تعيين ترخيص للمستخدم](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One). إذا كان لدي المستخدم ترخيص ، يجب أيضا التاكد من [تعيين دور مسؤول](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) يمكنه الوصول إلى مراكز الاداره.

يمكن ان تحدث هذه المشكلة أيضا عند حذف مستخدم وأعاده إنشائه بنفس الاسم الأساسي للمستخدم (UPN). يتم إنشاء الحساب الجديد باستخدام قيمه PUID (معرف فريد لPassport) مختلفه. عندما يحاول المستخدم الوصول إلى مجموعه موقع أو اندريف الخاصة بهم ، المستخدم لديه PUID غير صحيحه. يتضمن السيناريو الثاني مزامنة الدليل مع الوحدة التنظيمية "Active Directory" (OU). إذا كان المستخدمون بالفعل تسجيل الدخول إلى SharePoint ، ومن ثم يتم نقلها إلى OU مختلفه resynced مع SharePoint ، فانها قد تواجه هذه المشكلة.

لحل هذه المشكلة ، يجب استعاده UPN الأصلي مع الخطوات التالية في المقالة ، [استعاده مستخدم في Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).

ملاحظه: إذا لم يتوفر اندريف أو مركز مسؤول SharePoint لعده مستخدمين كان لديهم حق الوصول مسبقا ، قد تكون هناك مشكله خدمه مؤقته.  [تحقق من لوحه معلومات صحة الخدمة](https://portal.office.com/adminportal/home#/servicehealth).


