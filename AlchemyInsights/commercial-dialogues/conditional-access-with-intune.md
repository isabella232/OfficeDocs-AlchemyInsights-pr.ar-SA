---
title: استخدام الوصول الشرطي مع Intune
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6700002"
- "7680"
ms.openlocfilehash: 23afea21668191093d612d68ca6e9ab2a844f4a14977631d33f4fd956fc3c4e7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54005761"
---
# <a name="using-conditional-access-with-intune"></a>استخدام الوصول الشرطي مع Intune

يتطلب استخدام الوصول الشرطي مع Intune 3 خطوات:

- [قم بإنشاء نهج التوافق لتحديد الإعدادات التي يجب أن يتم التحقق من مطابقتها قبل أن يعتبر الجهاز متوافقا. على سبيل المثال، يجب أن يكون لدى الجهاز دبوس من 6 أرقام على الأقل قبل أن يعتبر متوافقا.](https://docs.microsoft.com/mem/intune/protect/create-compliance-policy)
- [أنشئ نهج الوصول الشرطي الذي يحدد الموارد التي يتم حمايتها، والشروط التي يجب أن يتم توفيرها للوصول إلى تلك الموارد. على سبيل المثال، يجب أن يكون الجهاز متوافقا قبل الوصول إلى البريد الإلكتروني الخاص بالشركة.](https://docs.microsoft.com/mem/intune/protect/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)
- [تأكد من أن كل من "سياسات التوافق" و"سياسات الوصول الشرطي" تستهدف مجموعات المستخدمين المطلوبة. قد يتطلب ذلك إنشاء مجموعات معينة من المستخدمين في Azure Active Directory.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-conditional-access)

[قراءة المزيد...](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started)
