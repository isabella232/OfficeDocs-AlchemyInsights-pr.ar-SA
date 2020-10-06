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
ms.openlocfilehash: 74a26306766ed7952a3bbbcb06f1f0113a113024
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/06/2020
ms.locfileid: "48366451"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>إصلاح مشاكل تسليم البريد الكتروني إلى المجلدات العمومية الممكنة للبريد

إذا تعذر علي المرسلين الخارجيين إرسال رسائل إلى المجلدات العمومية الممكنة للبريد الكتروني ، وتلقي المرسلين الخطا: **تعذر العثور عليه (550 5.4.1)**، تاكد من تكوين مجال البريد الكتروني للمجلد العمومي كمجال الترحيل الداخلي بدلا من مجال موثوق به:

1. فتح [مركز أداره Exchange (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).

2. انتقل إلى **Mail flow** \> **المجالات المقبولة**لتدفق البريد ، وحدد المجال المقبول ، ثم انقر فوق **تحرير**.

3. في صفحه الخصائص التي يتم فتحها ، إذا تم تعيين نوع المجال إلى **مخول**، فقم بتغيير القيمة إلى **الترحيل الداخلي** ثم انقر فوق **حفظ**.

إذا تلقي المرسلون الخارجيون الخطا **(550 5.7.13)**، فقم بتشغيل الأمر التالي في [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) للاطلاع علي الأذونات الخاصة بالمستخدمين المجهولين في المجلد العام:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` علي سبيل المثال ، `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous` .

للسماح للمستخدمين الخارجيين بإرسال البريد الكتروني إلى هذا المجلد العام ، أضف حق وصول كرياتيتيمس إلى المستخدم مجهول. علي سبيل المثال ، `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems` .
