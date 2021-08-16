---
title: إصلاح مشاكل تسليم البريد الإلكتروني إلى المجلدات العامة التي تم تمكين البريد لها
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.openlocfilehash: ff1400f694ae037a8658356af068b4c20b8fa9d9908dafedb90db7bb6859530f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54068799"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>إصلاح مشاكل تسليم البريد الإلكتروني إلى المجلدات العامة التي تم تمكين البريد لها

إذا لم يتمكن المرسلون الخارجيون من إرسال رسائل إلى المجلدات العامة التي تم تمكينها للبريد، وتلقي المرسلون الخطأ: لا يمكن العثور **على (550 5.4.1)**، فتحقق من تكوين مجال البريد الإلكتروني للمجلد العمومي ك مجال الإرسال الداخلي بدلا من مجال موثوق:

1. افتح Exchange [إدارة (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).

2. انتقل إلى **المجالات المقبولة لتدفق** \> **البريد**، وحدد المجال المقبول، ثم انقر فوق **تحرير**.

3. في صفحة الخصائص التي تفتح، إذا تم تعيين نوع المجال إلى **موثوق**، فغير القيمة إلى ترحيل **داخلي** ثم انقر فوق **حفظ**.

إذا تلقى المرسلون الخارجيون الخطأ الذي لم يكن لديك **الإذن (550 5.7.13)**، ف قم بتشغيل الأمر التالي في [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) لرؤية الأذونات للمستخدمين المجهولين في المجلد العمومي:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` على سبيل `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous` المثال، .

للسماح للمستخدمين الخارجيين بإرسال بريد إلكتروني إلى هذا المجلد العام، أضف الوصول CreateItems مباشرة إلى المستخدم المجهول. على سبيل `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems` المثال، .
