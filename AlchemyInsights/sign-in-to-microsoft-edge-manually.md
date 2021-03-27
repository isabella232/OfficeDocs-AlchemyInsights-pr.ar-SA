---
title: تسجيل الدخول إلى Microsoft Edge يدويا
ms.author: v-smandalika
author: v-smandalika
ms.date: 12/03/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "9003844"
- "6893"
- "8332"
- "9004625"
ms.openlocfilehash: f380d09dc14788205638cdee6aebe0b084ecab2f
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398644"
---
# <a name="sign-in-to-microsoft-edge-manually"></a>تسجيل الدخول إلى Microsoft Edge يدويا

إذا لم يكن المستخدم قد سجل الدخول تلقائيا أثناء تجربة التشغيل الأولى، يمكن للمستخدم تسجيل الدخول يدويا من خلال إعدادات المستعرض أو قائمة الهوية من قائمة منتحلة. لإدارة تسجيل الدخول، استخدم السياسات التالية:

1. [NonRemovableProfileEnabled](https://docs.microsoft.com/deployedge/microsoft-edge-policies#nonremovableprofileenabled) - للتأكد من أن المستخدم لديه دائما ملف تعريف عمل في Microsoft Edge.
2. [RestrictSigninToPattern](https://docs.microsoft.com/deployedge/microsoft-edge-policies#restrictsignintopattern) - لتقييد تسجيل الدخول إلى مجموعة من الحسابات الموثوق بها.
3. [BrowserSignin](https://docs.microsoft.com/deployedge/microsoft-edge-policies#browsersignin) - لتعطيل تسجيل الدخول أو إجبار المستخدمين على تسجيل الدخول.

