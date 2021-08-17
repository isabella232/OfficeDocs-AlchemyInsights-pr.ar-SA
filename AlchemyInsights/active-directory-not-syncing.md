---
title: لا تتم مزامنة Active Directory
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "1300023"
- "3754"
- "4531"
ms.openlocfilehash: d4615d335b9aeef69148cd93ff9f44bec6d7d876
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/13/2021
ms.locfileid: "58314191"
---
# <a name="active-directory-not-syncing"></a>لا تتم مزامنة Active Directory

إذا كنت تتلقى أخطاء في المزامنة، مثل "لا توجد مزامنة حديثة"، أو لاحظت حالة مزامنة الدليل في مدخل مسؤول Office، تقول "آخر مزامنة منذ أكثر من 3 أيام"، فقد يكون ذلك بسبب وجود إعدادات غير صحيحة أو أذونات غير كافية لتنفيذ المزامنة.  

قد يحل إعادة تثبيت AADConnect باستخدام الإعدادات المعبرة المشكلة بسرعة:

1. [قم بتنزيل أحدث إصدار من AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).

2. [اتبع إرشادات التثبيت السريع.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)

يجب تثبيت Azure AD Connect على نظام التشغيل Windows Server 2012 أو أحدث. يجب أن يكون هذا الخادم مشتركاً وقد يكون عبارة عن وحدة تحكم بالمجال أو خادم عضو. للحصول على قائمة كاملة بمتطلبات Azure AD الاتصال والمتطلبات الأساسية، راجع المتطلبات الأساسية ل [Azure AD الاتصال](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-prerequisites).

لمزيد من المعلومات حول حسابات خدمة AADConnect، راجع [Azure AD الاتصال: الحسابات والأذونات](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).
