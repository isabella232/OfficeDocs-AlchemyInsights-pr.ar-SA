---
title: إنشاء مجموعة
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
- "9003234"
- "7230"
ms.openlocfilehash: ec74b7c098d302d3bdeb5a412fad41efe7b82b98
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816331"
---
# <a name="create-a-group"></a>إنشاء مجموعة

يصف هذا الموضوع إنشاء المجموعة.

**الإذن لإنشاء مجموعة**

تأكد من أنك م مخولا لإنشاء مجموعة جديدة. يمكن للمسؤولين العامين تعطيل إنشاء المجموعة في مدخل Azure أو لوحة Access. قد تحتاج إلى مسؤول لإنشاء المجموعة الجديدة لك، أو من أجل من يعطيك الأذونات المناسبة.

**إدارة أذونات إنشاء المجموعة**

1. يمكن للمسؤولين العامين إدارة أذونات إنشاء المجموعات (لأسباب متعلقة والأمان) أو مجموعات Office 365 التي تم إنشاؤها في مدخل Azure أو لوحة Access، باختيار "يمكن للمستخدمين إنشاء مجموعات أمان في مداخل Azure" أو خيارات "يمكن للمستخدمين إنشاء مجموعات Office 365 في مداخل Azure" في كافة المجموعات عام  >  **(إعدادات)**.
2. يمكنك أيضا تقييد إنشاء المجموعة لتحديد مجموعة من المستخدمين إذا كان لديك ترخيص Azure Active Directory P1 Premium.

**تعطيل إعلام الترحيب لأعضاء مجموعة Office 365 الجدد**

يمكن تعطيل إعلام الترحيب الذي يتم إرساله إلى المستخدمين الذين تم إضافتهم إلى مجموعات Office 365 عن طريق تعيين **UnifiedGroupWelcomeMessageEnabled** إلى False في Powershell. تعرف على هذا الإعداد [هنا](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).

