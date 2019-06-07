---
title: استكشاف أخطاء رسائل "رفض الوصول"
ms.author: kirks
author: Techwriter40
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: c204f1889e03886fdfd3d1c760a4a2beb82b0836
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/07/2019
ms.locfileid: "34760328"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>استكشاف أخطاء رسائل "رفض الوصول" في "مركز مسؤول" Sharepoint/أونيدريفي

إذا كنت تتلقى رسالة وصول مرفوض عند محاولة الاستعراض إلى "مركز مسؤول" Sharepoint/أندريف، الرجاء التأكد من أن تقوم [تعيين ترخيص للمستخدم](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One). إذا كان المستخدم لديه ترخيص، يجب أيضا التأكد من أنها [المعين لدور مسؤول](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) الوصول إليها مراكز الإدارة.

قد تحدث هذه المشكلة أيضا عند حذف مستخدم وإعادة إنشائها باستخدام نفس اسم المستخدم الأساسي (UPN). يتم إنشاء حساب جديد باستخدام قيمة PUID (المعرف الفريد ل Passport) مختلفة. عندما يحاول المستخدم الوصول إلى مجموعة موقع أو أندريف بها، لدى المستخدم PUID غير صحيحة. سيناريو ثاني يتضمن الدليل المزامنة مع وحدة "خدمة active Directory" تنظيمية (OU). إذا كان المستخدمون قد مسبقاً بتسجيل الدخول إلى SharePoint، ثم يتم نقلها إلى OU مختلفة و resynced مع SharePoint، قد تواجه هذه المشكلة.

لحل هذه المشكلة، يجب عليك استعادة UPN الأصلي باستخدام الخطوات المذكورة في المقالة، [استعادة مستخدم في Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).

ملاحظة: إذا لم يتوفر أحد مراكز أندريف أو مسؤول SharePoint للعديد من المستخدمين الذين تم الوصول، قد يكون هناك مشكلة في خدمة مؤقت.  [تحقق من لوحة المعلومات الصحية الخدمة](https://portal.office.com/adminportal/home#/servicehealth).


