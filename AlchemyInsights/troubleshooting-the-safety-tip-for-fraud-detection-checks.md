---
title: استكشاف الأخطاء وإصلاحها تلميح الأمان عمليات التحقق من الاحتيال
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
ms.openlocfilehash: c7ee1fcc887a3221b5f2acda1aa6ae6beb03cb96686d4ecb7828a02f8ff48302
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53955953"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>استكشاف الأخطاء وإصلاحها تلميح الأمان عمليات التحقق من الاحتيال

إذا كنت تحصل على رسالة تلميح الأمان تقول "فشل المرسل في التحقق من الاحتيال وقد لا يكون الشخص الذي يبدو عليه"، ففشل المرسل في اجتياز أي من عمليات التحقق من مصادقة DKIM أو SPF. وأفضل طريقة لحل هذه المشكلة هي أن يفوض المرسل نفسه. إذا كان المرسل يرسل بالنيابة عنك، يجب تخويله بإضافة عنوان IP الخاص به إلى سجل SPF الخاص بك.
  
راجع استكشاف الأخطاء الحمراء [(المريبة) وإصلاحها تلميح الأمان التحقق](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) من الكشف عن الاحتيال للحصول على مزيد من المعلومات.
  
فيما يلي بعض الارتباطات الأخرى التي يمكن أن تساعدك:
  
- [كيفية استخدام Microsoft إطار نهج المرسل (SPF) لمنع الانتحال](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [إعداد SPF للمساعدة في منع التهزاء](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
