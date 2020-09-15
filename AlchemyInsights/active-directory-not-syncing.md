---
title: لم تتم مزامنة active directory
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "3754"
ms.openlocfilehash: 3517f424b4dcd89f915acebab747a9bff993fdbd
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47697616"
---
# <a name="active-directory-not-syncing"></a>لم تتم مزامنة active directory

إذا كنت تتلقي أخطاء مزامنة ، علي سبيل المثال "لا يوجد مزامنة حديثه" أو ملاحظه حاله مزامنة الدليل في مدخل مسؤول Office ، فهذا يعني ان هذا الAADConnect لديه إعدادات غير صحيحه أو أذونات غير كافيه لاجراء المزامنة.  

قد يؤدي أعاده تثبيت AADConnect باستخدام الإعدادات السريعة إلى حل المشكلة بسرعة:

1. قم [بتنزيل أحدث إصدار من AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).

2. [اتبع الإرشادات الخاصة بالتثبيت السريع](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).

لمزيد من المعلومات حول حسابات خدمات AADConnect ، راجع [AZURE AD Connect: الحسابات والأذونات](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).
