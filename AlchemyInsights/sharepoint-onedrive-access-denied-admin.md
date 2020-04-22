---
title: استكشاف أخطاء الوصول الرسائل المرفوضة
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 82e11458529b8a49e583b1a6963a51e2a466bfd6
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43758355"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>استكشاف أخطاء الوصول الرسائل المرفوضة في Sharepoint/OneDrive Admin Center

إذا كنت تتلقى رسالة رفض الوصول عند محاولة الاستعراض إلى مركز مسؤول Sharepoint/OneDrive، يرجى التأكد من [تعيين ترخيص للمستخدم](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One). إذا كان لدى المستخدم ترخيص، يجب عليك [أيضًا](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) التأكد من تعيين دور مسؤول يمكنه الوصول إلى مراكز الإدارة.

يمكن أن تحدث هذه المشكلة أيضاً عند حذف مستخدم وإعادة إنشائه بنفس اسم المستخدم الرئيسي (UPN). يتم إنشاء الحساب الجديد باستخدام قيمة PUID مختلفة (معرف فريد من جواز السفر). عندما يحاول المستخدم الوصول إلى مجموعة موقع أو OneDrive الخاص بهم، يكون لدى المستخدم PUID غير صحيح. يتضمن سيناريو الثاني مزامنة الدليل مع وحدة تنظيمية "الدليل النشط" (OU). إذا قام المستخدمون بتسجيل الدخول بالفعل إلى SharePoint، ثم تم نقلهم إلى OU مختلف وإعادة مزامنتهم مع SharePoint، فقد يواجهون هذه المشكلة.

لحل هذه المشكلة، يجب استعادة UPN الأصلي مع الخطوات في المقالة استعادة [مستخدم في Microsoft 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).

ملاحظة: إذا كان مركز OneDrive أو SharePoint Admin غير متوفر للعديد من المستخدمين الذين سبق لهم الوصول، فقد تكون هناك مشكلة في الخدمة المؤقتة.  [تحقق من لوحة معلومات صحة الخدمة](https://portal.office.com/adminportal/home#/servicehealth).


