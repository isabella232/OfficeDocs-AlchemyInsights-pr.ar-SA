---
title: إصلاح مشاكل تسليم البريد الكتروني إلى المجلدات العمومية الممكنة للبريد
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
ms.assetid: ''
ms.openlocfilehash: da35ae4bd911fb75f23cc1c99aacbaa2392425dd
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47677915"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>إصلاح مشاكل تسليم البريد الكتروني إلى المجلدات العمومية الممكنة للبريد

إذا تعذر علي المرسلين الخارجيين إرسال رسائل إلى المجلدات العمومية الممكنة للبريد الكتروني ، وتلقي المرسلين الخطا: **تعذر العثور عليه (550 5.4.1)**، تاكد من تكوين مجال البريد الكتروني للمجلد العمومي كمجال الترحيل الداخلي بدلا من مجال موثوق به:

1. فتح [مركز أداره Exchange (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).

2. انتقل إلى **Mail flow** \> **المجالات المقبولة**لتدفق البريد ، وحدد المجال المقبول ، ثم انقر فوق **تحرير**.

3. في صفحه الخصائص التي يتم فتحها ، إذا تم تعيين نوع المجال إلى **مخول**، فقم بتغيير القيمة إلى **الترحيل الداخلي** ثم انقر فوق **حفظ**.

إذا تلقي المرسلون الخارجيون الخطا **(550 5.7.13)**، فقم بتشغيل الأمر التالي في [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) للاطلاع علي الأذونات الخاصة بالمستخدمين المجهولين في المجلد العام:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` علي سبيل المثال ، `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous` .

للسماح للمستخدمين الخارجيين بإرسال البريد الكتروني إلى هذا المجلد العام ، أضف حق وصول كرياتيتيمس إلى المستخدم مجهول. علي سبيل المثال ، `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems` .
