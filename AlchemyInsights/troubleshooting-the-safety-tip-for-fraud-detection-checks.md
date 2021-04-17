---
title: استكشاف الأخطاء في تلميح الأمان للتحقق من الاحتيال وإصلاحها
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: 85faa0086935fb7e7132ee9fdced546bafdb344c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834718"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>استكشاف الأخطاء في تلميح الأمان للتحقق من الاحتيال وإصلاحها

إذا كنت تحصل على تلميح أمان يقول "فشل المرسل في التحقق من الاحتيال وقد لا يكون الشخص الذي يبدو عليه"، ففشل المرسل في اجتياز أي من فحص مصادقة DKIM أو SPF. وأفضل طريقة لحل هذه المشكلة هي أن يفوض المرسل نفسه. إذا كان المرسل يرسل بالنيابة عنك، يجب تخويله بإضافة عنوان IP الخاص به إلى سجل SPF الخاص بك.
  
راجع استكشاف الأخطاء في تلميح الأمان [الأحمر (المريب)](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) وإصلاحها للتحقق من الكشف عن الاحتيال للحصول على مزيد من المعلومات.
  
فيما يلي بعض الارتباطات الأخرى التي يمكن أن تساعدك:
  
- [كيفية استخدام Microsoft إطار نهج المرسل (SPF) لمنع الانتحال](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [إعداد SPF للمساعدة في منع التهزاء](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
