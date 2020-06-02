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
ms.openlocfilehash: 9430b9786b35dda9fb2604fb6ae3c39c8c258d6e
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/02/2020
ms.locfileid: "44505366"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>استكشاف أخطاء الوصول الرسائل المرفوضة في Sharepoint/OneDrive Admin Center

إذا كنت تتلقى رسالة رفض الوصول عند محاولة الاستعراض إلى مركز مسؤول Sharepoint/OneDrive، يرجى التأكد من [تعيين ترخيص للمستخدم](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users). إذا كان لدى المستخدم ترخيص، يجب عليك [أيضًا](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) التأكد من تعيين دور مسؤول يمكنه الوصول إلى مراكز الإدارة.

يمكن أن تحدث هذه المشكلة أيضاً عند حذف مستخدم وإعادة إنشائه بنفس اسم المستخدم الرئيسي (UPN). يتم إنشاء الحساب الجديد باستخدام قيمة PUID مختلفة (معرف فريد من جواز السفر). عندما يحاول المستخدم الوصول إلى مجموعة موقع أو OneDrive الخاص بهم، يكون لدى المستخدم PUID غير صحيح. يتضمن سيناريو الثاني مزامنة الدليل مع وحدة تنظيمية "الدليل النشط" (OU). إذا قام المستخدمون بتسجيل الدخول بالفعل إلى SharePoint، ثم تم نقلهم إلى OU مختلف وإعادة مزامنتهم مع SharePoint، فقد يواجهون هذه المشكلة.

لحل هذه المشكلة، يجب استعادة UPN الأصلي مع الخطوات في المقالة استعادة [مستخدم في Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).

ملاحظة: إذا كان مركز OneDrive أو SharePoint Admin غير متوفر للعديد من المستخدمين الذين سبق لهم الوصول، فقد تكون هناك مشكلة في الخدمة المؤقتة.  [تحقق من لوحة معلومات صحة الخدمة](https://portal.office.com/adminportal/home#/servicehealth).


