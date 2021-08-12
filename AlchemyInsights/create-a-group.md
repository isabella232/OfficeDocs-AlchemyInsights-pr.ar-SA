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
ms.openlocfilehash: 4530abb3bf597458ea22441203a0db24b4b109f0760258310072891014c4b454
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53929292"
---
# <a name="create-a-group"></a>إنشاء مجموعة

يصف هذا الموضوع إنشاء المجموعة.

**الإذن لإنشاء مجموعة**

تأكد من أنك م مخولا لإنشاء مجموعة جديدة. يمكن للمسؤولين العامين تعطيل إنشاء المجموعة في مدخل Azure أو لوحة Access. قد تحتاج إلى مسؤول لإنشاء المجموعة الجديدة لك، أو من أجل من يعطيك الأذونات المناسبة.

**إدارة أذونات إنشاء المجموعة**

1. يمكن للمسؤولين العامين إدارة أذونات إنشاء المجموعات (لأسباب متعلقة ب الأمان) أو مجموعات Office 365 التي تم إنشاؤها في مدخل Azure أو لوحة Access، باختيار "يمكن للمستخدمين إنشاء مجموعات أمان في مداخل Azure" أو خيارات "يمكن للمستخدمين إنشاء مجموعات Office 365 في مداخل Azure" في كافة المجموعات عام  >  **(الإعدادات)**.
2. يمكنك أيضا تقييد إنشاء المجموعة لتحديد مجموعة من المستخدمين إذا كان لديك ترخيص Azure Active Directory P1 Premium.

**تعطيل إعلام الترحيب لأعضاء Office 365 الجدد**

يمكن تعطيل إعلام الترحيب الذي يتم إرساله إلى المستخدمين Office 365 المجموعات من خلال تعيين **UnifiedGroupWelcomeMessageEnabled** إلى False في Powershell. تعرف على هذا الإعداد [هنا](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).

