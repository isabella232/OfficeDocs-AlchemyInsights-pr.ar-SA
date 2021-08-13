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
ms.openlocfilehash: 4bfbe6b2dd9a2112f0cb7af0d6e7a46693bc70680895fd674ddb0332b7071797
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53937088"
---
# <a name="active-directory-not-syncing"></a>لا تتم مزامنة Active Directory

إذا كنت تتلقى أخطاء في المزامنة، مثل "لا توجد مزامنة حديثة"، أو لاحظت حالة مزامنة الدليل في مدخل مسؤول Office، تقول "آخر مزامنة منذ أكثر من 3 أيام"، فقد يكون سبب ذلك أن AADConnect لديه إعدادات غير صحيحة أو أذونات غير كافية لتنفيذ المزامنة.  

قد يحل إعادة تثبيت AADConnect باستخدام الإعدادات المعبرة المشكلة بسرعة:

1. [قم بتنزيل أحدث إصدار من AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).

2. [اتبع إرشادات التثبيت السريع.](/azure/active-directory/hybrid/how-to-connect-install-express)

يجب تثبيت Azure AD Connect على نظام التشغيل Windows Server 2012 أو أحدث. يجب أن يكون هذا الخادم مشتركاً وقد يكون عبارة عن وحدة تحكم بالمجال أو خادم عضو. للحصول على قائمة كاملة بمتطلبات Azure AD الاتصال والمتطلبات الأساسية، راجع المتطلبات الأساسية ل [Azure AD الاتصال](/azure/active-directory/hybrid/how-to-connect-install-prerequisites).

لمزيد من المعلومات حول حسابات خدمة AADConnect، راجع [Azure AD الاتصال: الحسابات والأذونات](/azure/active-directory/hybrid/reference-connect-accounts-permissions).
