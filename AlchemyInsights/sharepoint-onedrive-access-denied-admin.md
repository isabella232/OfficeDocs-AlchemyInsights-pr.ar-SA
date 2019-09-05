---
title: استكشاف أخطاء رسائل تم رفض الوصول وإصلاحها
ms.author: pebaum
author: Techwriter40
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 4e6fdc6fbf745d1702bf1a7b3474ac82f6662305
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/04/2019
ms.locfileid: "36751263"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>استكشاف أخطاء الرسائل التي تم رفض الوصول إليها في مركز مسؤول Sharepoint/OneDrive

إذا كنت تتلقى رسالة تم رفض الوصول عند محاولة الاستعراض إلى مركز مسؤول Sharepoint/OneDrive، الرجاء التأكد من [تعيين ترخيص للمستخدم](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One). إذا كان لدى المستخدم ترخيص، يجب عليك أيضاً التأكد من [تعيين دور مسؤول](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) يمكنه الوصول إلى مراكز المسؤول.

يمكن أن تحدث هذه المشكلة أيضًا عند حذف مستخدم وإعادة إنشائه بنفس اسم المستخدم الأساسي (UPN). يتم إنشاء الحساب الجديد باستخدام قيمة PUID (معرف فريد جواز السفر) مختلفة. عندما يحاول المستخدم الوصول إلى مجموعة موقع أو أندريف الخاصة بهم، لدى المستخدم PUID غير صحيح. يتضمن سيناريو ثاني مزامنة الدليل مع وحدة تنظيمية "Active Directory" (OU). إذا قام المستخدمون بالفعل بتسجيل الدخول إلى SharePoint، ثم يتم نقلها إلى وحدة الوحدة التنظيمية مختلفة وإعادة مزامنتها مع SharePoint، فقد تواجه هذه المشكلة.

لحل هذه المشكلة، يجب استعادة UPN الأصلي مع الخطوات الموجودة في المقالة [استعادة مستخدم في Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).

ملاحظة: إذا لم يكن مركز مسؤول OneDrive أو SharePoint متوفرًا للعديد من المستخدمين الذين كان لديهم حق الوصول مسبقًا، فقد تكون هناك مشكلة خدمة مؤقتة.  [تحقق من لوحة معلومات صحة الخدمة](https://portal.office.com/adminportal/home#/servicehealth).


