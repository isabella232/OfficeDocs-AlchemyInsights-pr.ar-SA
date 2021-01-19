---
title: مشاكل الموافقة علي المسؤول
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004354"
- "7786"
ms.openlocfilehash: 6154b4b9cce51be3271cb25132f409319d8da14b
ms.sourcegitcommit: 113b802081101de70810fc73938ea92f7518d8c6
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/18/2021
ms.locfileid: "49900748"
---
# <a name="admin-consent-issues"></a>مشاكل الموافقة علي المسؤول

1. تمكين [سير عمل الموافقة علي المسؤول](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) للسماح للمستخدمين بطلب موافقه المسؤول مباشره من شاشه الموافقة.

1. إذا رايت أنت أو المستخدمون الذين لديهم أخطاء غير متوقعه اثناء عمليه الموافقة ، فراجع هذه المقالة لمعرفه الخطوات المتعلقة باستكشاف الأخطاء وإصلاحها: [خطا غير متوقع عند اجراء موافقه علي تطبيق](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).

1. تعرف علي [المزيد حول موافقه المسؤول علي النظام الأساسي للهوية من Microsoft](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent)، والطريقة التي تعمل بها [مطالبه الموافقة](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent) ، وكيفيه [تقييم طلب الموافقة علي المسؤول علي مستوي المستاجر](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent).

1. تتبع التطبيقات التي تتكامل مع النظام الأساسي لهويه Microsoft نموذج تخويل يمنح المستخدمين ويتحكم بالتحكم في كيفيه الوصول إلى البيانات. تم تحديث تطبيق نموذج التخويل علي نقطه نهاية النظام الأساسي لهويه Microsoft ، وهو يغير كيفيه تفاعل التطبيق مع النظام الأساسي للهوية Microsoft. اطلع علي [الأذونات والموافقة في نقطه نهاية النظام الأساسي لهويه Microsoft](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) للحصول علي نظره عامه حول نموذج التخويل هذا ، بما في ذلك النطاقات والأذونات والموافقة.