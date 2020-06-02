---
title: استكشاف أخطاء معلومات الأمان للتحقق من اكتشاف الاحتيال
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: 74913492a086de688067d588e95dd87e6946743b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/02/2020
ms.locfileid: "44504970"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>استكشاف أخطاء معلومات الأمان للتحقق من اكتشاف الاحتيال

إذا كنت تحصل على معلومات أمان تقول "فشل المرسل في التحقق من اكتشاف الاحتيال وقد لا يكون ما يبدو أنه عليه"، فقد فشل المرسل في اجتياز عمليات التحقق من مصادقة DKIM أو SPF. أفضل طريقة لحل هذا هو للمرسل لتخويل أنفسهم. إذا كان المرسل يرسل نيابة عنك، فستحتاج إلى تخويلها بإضافة عنوان IP الخاص بالمرسل إلى سجل SPF الخاص بك.
  
راجع [استكشاف الأخطاء وإصلاحها في معلومات الأمان الحمراء (المشبوهة) للتحقق من اكتشاف الاحتيال](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) لمزيد من المعلومات.
  
فيما يلي بعض الروابط الأخرى التي يمكن أن تساعد:
  
- [كيف تستخدم Microsoft إطار نهج المرسل (SPF) لمنع الانتحال](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [إعداد SPF للمساعدة في منع الانتحال](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
