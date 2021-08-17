---
title: استخدام iOS VPP Applications IOS IOS VPP Rule ID 1018
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: f693d12ff0f9c193cba0c6a6802b22d7acd37532c65986e5f6613e18c021f06b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54083001"
---
# <a name="working-with-ios-vpp-applications"></a>استخدام تطبيقات vPP ل iOS

اقرأ كيفية إدارة تطبيقات [iOS](https://docs.microsoft.com/intune/vpp-apps-ios) التي تم شراؤها من خلال برنامج شراء كمية باستخدام Microsoft Intune للتعرف على الميزات والقيود والخطوات اللازمة لاستخدام برنامج شراء Apple Volume Purchase Program والدعم الخاص به في Microsoft Intune.
  
 **المشاكل الشائعة:** "لقد عينت تطبيق iOS VPP للمستخدمين، ولكن فشل التثبيت."
  
- قد يحدث هذا إذا تم استخدام رمز VPP مميز واحد عبر موفري إدارة أجهزة محمولة متعددين. قد يتم استخدام الرموز المميزة ل VPP من Apple مع موفر واحد فقط. إذا استخدمت رمز VPP مميزا مع عدة موفرين، فيجب إعادة تحميل الرمز المميز إلى Intune.

- قد يفشل التثبيت أيضا إذا تجاوز العدد الإجمالي لعدد التثبيتات عدد التراخيص. لعرض تقرير استخدام للتراخيص، انتقل إلى صفحة تراخيص تطبيقات **Intune** \>  Mobile. للتعرف على كيفية استعادة التراخيص التي يتم استخدامها، راجع [هذه المقالة.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
