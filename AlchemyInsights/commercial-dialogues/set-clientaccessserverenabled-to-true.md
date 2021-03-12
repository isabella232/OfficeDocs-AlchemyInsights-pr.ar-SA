---
title: تعيين ClientAccessServerEnabled إلى True
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: 2adf35662797e9e9e354ddd0c513f5ce2463d07c
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/11/2021
ms.locfileid: "50743153"
---
# <a name="set-clientaccessserverenabled-to-true"></a>تعيين ClientAccessServerEnabled إلى True

إذا لم تتمكن من فتح رسالة بريد إلكتروني مشفرة وبدلا من ذلك رأيت مرفق **rpmsg،** فتابع تنفيذ الخطوات التالية:

1. الاتصال ب Exchange Online PowerShell.

> [!NOTE]
> للاتصال ب Exchange Online PowerShell، يجب تسجيل الدخول باستخدام مسؤول عام أو حساب مسؤول Exchange.

   أ. افتح Windows PowerShell، ثم قم بتشغيل الأمر التالي: `$UserCredential = Get-Credential`
ب. في مربع الحوار طلب اعتماد **Windows PowerShell،** أدخل حساب العمل أو المدرسة وكلمة المرور، ج. انقر فوق **موافق**. 

2. قم بتشغيل الأمر التالي لإنشاء جلسة عمل جديدة:

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    أ. قم بتنفيذ الأمر التالي:
    
    `Import-PSSession $Session -DisableNameChecking`

3. الأمر `Get-IRMConfiguration` "تشغيل".

4. تحقق من **الإعداد ClientAccessServerEnabled.** 

    أ. إذا **تم تعيين إعداد ClientAccessServerEnabled** إلى **False**، ف قم بتشغيل أمر cmdlet التالي: `Set-IRMConfiguration -ClientAccessServerEnabled $True`

> [!TIP]
> أغلق جلسة powershell دائما باستخدام الأمر التالي: `Remove-PSSession $Session`

لمزيد من المعلومات، راجع [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).

