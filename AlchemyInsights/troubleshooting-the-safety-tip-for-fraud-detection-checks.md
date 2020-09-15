---
title: استكشاف أخطاء التحقق من الاحتيال وإصلاحها
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: e42b498070bf5d9bfc36110667da8cc0fd431524
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658397"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>استكشاف أخطاء التحقق من الاحتيال وإصلاحها

إذا كنت تحصل علي تلميح أمان يقول "فشل المرسل في التحقق من البحث عن الاحتيال الخاص بنا وقد لا يكون من يبدو انه" ، فهذا يعني ان المرسل لم يتمكن من تمرير اي من المستخدمين الذين لديهم اي من اليم إلى DKIM SPF. أفضل طريقه لحل هذه المشكلة هي لتخويل المرسل نفسه. إذا كان المرسل يرسل بالنيابة عنك ، فيجب عليك تخويله عن طريق أضافه عنوان IP الخاص بالمرسل إلى سجل SPF.
  
راجع [استكشاف أخطاء تلميح الأمان الأحمر (المشبوه) للتحقق من اكتشاف الاحتيال](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) للحصول علي مزيد من المعلومات.
  
اليك بعض الارتباطات الأخرى التي يمكنها مساعدتك:
  
- [كيفيه استخدام Microsoft لاطار عمل نهج المرسل (SPF) لمنع الانتحال](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [اعداد SPF للمساعدة علي منع الانتحال](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
