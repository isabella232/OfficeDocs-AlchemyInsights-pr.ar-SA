---
title: استكشاف مشاكل موافقة المستخدم وإصلاحها
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
ms.openlocfilehash: db784c133fec554604ad09f5b27941879d97ff238f926ff6338d0f3b7c3c4105
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54007885"
---
# <a name="troubleshoot-user-consent"></a>استكشاف مشاكل موافقة المستخدم وإصلاحها

1. يمكنك تكوين كيفية موافقة المستخدمين النهائيين على التطبيقات من خلال مدخل Azure أو PowerShell. راجع [إعدادات موافقة المستخدم](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) للحصول على مزيد من المعلومات.
1. يمكن للمسؤول أيضا استخدام واجهة برمجة تطبيقات [Microsoft Graph](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) لمنح الموافقة على الأذونات المفوضة بالنيابة عن مستخدم واحد. لمزيد من المعلومات، راجع الوصول نيابة [عن مستخدم](https://docs.microsoft.com/graph/auth-v2-user).
1. [أخطاء موافقة المستخدم](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error): تناقش هذه المقالة الأخطاء التي يمكن أن تحدث أثناء عملية الموافقة على أحد التطبيقات. إذا كنت تقوم استكشاف أخطاء طلبات الموافقة غير المتوقعة التي لا تحتوي على أي رسائل خطأ وإصلاحها، فا راجع سيناريوهات المصادقة [ل Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).