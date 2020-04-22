---
title: إصلاح مشكلات تسليم البريد الإلكتروني إلى المجلدات العامة التي تم تمكينها بالبريد
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.assetid: ''
ms.openlocfilehash: e261fe60843555fa45927b0a6b36e1ccf79fb028
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716339"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>إصلاح مشكلات تسليم البريد الإلكتروني إلى المجلدات العامة التي تم تمكينها بالبريد

إذا لم يتمكن المرسلون الخارجيون من إرسال رسائل إلى المجلدات العامة التي تم تمكينها بالبريد، وتلقى المرسلون الخطأ: **لا يمكن العثور عليها (550 5.4.1)،** فتحقق من تكوين مجال البريد الإلكتروني للمجلد العام كمجال ترحيل داخلي بدلاً من مجال موثوق به:

1. افتح [مركز إدارة Exchange (EAC).](https://docs.microsoft.com/Exchange/exchange-admin-center)

2. انتقل إلى \> **المجالات المقبولة لتدفق** **البريد،** وحدد المجال المقبول، ثم انقر فوق **تحرير**.

3. في صفحة الخصائص التي تفتح، إذا تم تعيين نوع المجال إلى **"موثوق"،** قم بتغيير القيمة إلى **الترحيل الداخلي** ثم انقر فوق **حفظ**.

إذا تلقى المرسلون الخارجيون الخطأ **ليس لديك إذن (550 5.7.13)**، قم بتشغيل الأمر التالي في [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) لرؤية الأذونات للمستخدمين المجهولين في المجلد العمومي:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`على سبيل `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`المثال، .

للسماح للمستخدمين الخارجيين بإرسال بريد إلكتروني إلى هذا المجلد العام، أضف حق الوصول إلى CreateItems إلى المستخدم Anonymous. على سبيل `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`المثال، .
