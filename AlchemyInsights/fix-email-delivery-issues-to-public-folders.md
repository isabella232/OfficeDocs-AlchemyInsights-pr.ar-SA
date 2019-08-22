---
title: إصلاح مشاكل التسليم الإلكتروني للمجلدات العمومية التي تعتمد البريد
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.assetid: ''
ms.openlocfilehash: f7b5e5a230d26870d5e95e8762b5874f73723c6d
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/22/2019
ms.locfileid: "36525082"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>إصلاح مشاكل التسليم الإلكتروني للمجلدات العمومية التي تعتمد البريد

إذا لم يكن المرسلين الخارجيين لا يمكن إرسال الرسائل إلى المجلدات العمومية التي تعتمد البريد ومرسلي رسالة الخطأ: **تعذر العثور على (550 5.4.1)**، تحقق من مجال بريد إلكتروني للمجلد العمومي تم تكوينه كمجال ترحيل داخلي بدلاً من المجال الموثوق:

1. فتح [مركز مسؤول Exchange (شرق)](https://docs.microsoft.com/Exchange/exchange-admin-center).

2. انتقل إلى **تدفق البريد** \> **مجالات مقبولة**، حدد المجال المقبول، وثم انقر فوق **تحرير**.

3. في الخصائص ذلك الفتح الصفحة إذا تم تعيين نوع المجال إلى **حجية**وتغيير القيمة إلى **ترحيل داخلي** وثم انقر فوق **حفظ**.

في حالة ظهور المرسلين الخارجيين الخطأ **ليس لديك الإذن (550 5.7.13)**، تشغيل الأمر التالي في [PowerShell Exchange عبر إنترنت](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) لعرض الأذونات للمستخدمين المجهولين في المجلد العمومي:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`على سبيل المثال، `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.

للسماح للمستخدمين الخارجيين بإرسال بريد إلكتروني إلى هذا المجلد العمومي، إضافة الوصول كريتيتيمس اليمين للمستخدم المجهول. على سبيل المثال، `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.
