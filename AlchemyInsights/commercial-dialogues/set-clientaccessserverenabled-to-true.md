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
ms.openlocfilehash: b134c952e3cc5305d8f3e6f44031e7f33d7938b67ff122c46cb74bbd33cbf59e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53994852"
---
# <a name="set-clientaccessserverenabled-to-true"></a>تعيين ClientAccessServerEnabled إلى True

إذا لم تتمكن من فتح رسالة بريد إلكتروني مشفرة وبدلا من ذلك رأيت مرفق **rpmsg،** فتابع تنفيذ الخطوات التالية:

1. الاتصال Exchange Online PowerShell.

> [!NOTE]
> للاتصال ب PowerShell Exchange Online، يجب تسجيل الدخول باستخدام مسؤول عام أو Exchange مسؤول.

   a. افتح Windows PowerShell، ثم قم بتشغيل الأمر التالي:`$UserCredential = Get-Credential`
b. في مربع **Windows PowerShell طلب** بيانات الاعتماد، أدخل حساب العمل أو المدرسة وكلمة المرور، ج. انقر فوق **موافق**. 

2. قم بتشغيل الأمر التالي لإنشاء جلسة عمل جديدة:

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    a. قم بتنفيذ الأمر التالي:
    
    `Import-PSSession $Session -DisableNameChecking`

3. الأمر `Get-IRMConfiguration` "تشغيل".

4. تحقق من **الإعداد ClientAccessServerEnabled.** 

    a. إذا **تم تعيين إعداد ClientAccessServerEnabled** إلى **False**، ف قم بتشغيل أمر cmdlet التالي: `Set-IRMConfiguration -ClientAccessServerEnabled $True`

> [!TIP]
> أغلق جلسة powershell دائما باستخدام الأمر التالي: `Remove-PSSession $Session`

لمزيد من المعلومات، راجع Exchange Online [PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).

