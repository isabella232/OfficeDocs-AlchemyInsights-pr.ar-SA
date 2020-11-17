---
title: إنشاء مجموعه
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
- "9003234"
- "7230"
ms.openlocfilehash: b8cb3f1de991bfe7197607d5e8964a018e31c122
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 11/17/2020
ms.locfileid: "49088487"
---
# <a name="create-a-group"></a>إنشاء مجموعه

يصف هذا الموضوع إنشاء المجموعة.

**اذن إنشاء مجموعه**

تاكد من انك مصرحت لك بإنشاء مجموعه جديده. يمكن للمسؤولين العموميين تعطيل إنشاء المجموعة في مدخل Azure أو لوحه الوصول. قد تحتاج إلى مسؤول لإنشاء المجموعة الجديدة لك ، أو لمنحك الأذونات المناسبة.

**أداره أذونات إنشاء المجموعة**

1. بإمكان المسؤولين العموميين أداره أذونات إنشاء المجموعة (لأسباب تتعلق بالأمان) أو مجموعات Office 365 التي تم إنشاؤها في مدخل azure أو لوحه الوصول ، عن طريق اختيار "يمكن للمستخدمين إنشاء مجموعات الأمان في azure مداخل" أو "يمكن للمستخدمين إنشاء مجموعات من office **365 في azure** portal  >  **General (Settings)**.
2. يمكنك أيضا تقييد إنشاء المجموعة لتحديد مجموعه من المستخدمين إذا كان لديك ترخيص Azure Active directory P1.

**تعطيل الاعلامات الخاصة بأعضاء مجموعه Office 365 الجديدة**

يمكن تعطيل الاعلام بالترحيب المرسل إلى المستخدمين الذين تمت اضافتهم إلى مجموعات Office 365 عن طريق اعداد **أونيفيدجروبويلكوميميساجينابليد** to False في Powershell. تعرف علي هذا الاعداد [هنا](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).

