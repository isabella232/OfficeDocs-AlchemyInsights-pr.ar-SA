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
ms.openlocfilehash: 6e86c6b4c9c6adcbeac504acd5a10f2139d04237
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/08/2021
ms.locfileid: "50692420"
---
# <a name="using-conditional-access-with-intune"></a>استخدام الوصول الشرطي مع Intune

يتطلب استخدام "الوصول المشروط" مع Intune ثلاث خطوات:

- [أنشئ نهج توافق لتحديد الإعدادات التي يجب أن يتم التحقق من مطابقتها قبل أن يعتبر الجهاز متوافقا. على سبيل المثال، يجب أن يكون رقم pin في الجهاز 6 أرقام على الأقل قبل أن يعتبر متوافقا.](https://docs.microsoft.com/mem/intune/protect/create-compliance-policy)
- [أنشئ نهج الوصول المشروط الذي يحدد الموارد التي يتم حمايتها، والشروط التي يجب أن يتم تأمينها للوصول إلى تلك الموارد. على سبيل المثال، يجب أن يكون الجهاز متوافقا قبل الوصول إلى البريد الإلكتروني الخاص بالشركة.](https://docs.microsoft.com/mem/intune/protect/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)
- [تأكد من أن كل من "سياسات التوافق" و"سياسات الوصول المشروط" تستهدف مجموعات المستخدمين المطلوبة. قد يتطلب ذلك إنشاء مجموعات معينة من المستخدمين في Azure Active Directory.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-conditional-access)

[قراءة المزيد...](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started)
