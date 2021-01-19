---
title: استكشاف الأخطاء وإصلاحها
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
- "9004353"
- "7785"
ms.openlocfilehash: 7249bafe1b047c66d9351a79f1782cfcc1a936a1
ms.sourcegitcommit: 7b213fd5e8a3fdb5c602673dc194d576d372ac96
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/18/2021
ms.locfileid: "49900781"
---
# <a name="troubleshoot-user-consent"></a>استكشاف الأخطاء وإصلاحها

1. يمكنك تكوين الطريقة التي يتم بها الموافقة علي المستخدمين للتطبيقات عبر مدخل Azure أو PowerShell. راجع [إعدادات موافقه المستخدم](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) للحصول علي مزيد من المعلومات.
1. يمكن للمسؤول أيضا استخدام واجهه برمجه التطبيق الخاصة ب [Microsoft Graph](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) لمنح الموافقة علي الأذونات المفوضة بالنيابة عن مستخدم واحد. لمزيد من المعلومات ، راجع [الحصول علي حق الوصول بالنيابة عن مستخدم](https://docs.microsoft.com/graph/auth-v2-user).
1. [أخطاء الموافقة علي المستخدم](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error): تناقش هذه المقالة الأخطاء التي يمكن ان تحدث اثناء عمليه كونسينتينج إلى تطبيق. إذا كنت تقوم باستكشاف الأخطاء وإصلاحها ، لا تتضمن اي رسائل خطا ، راجع [سيناريوهات المصادقة ل AZURE AD](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).