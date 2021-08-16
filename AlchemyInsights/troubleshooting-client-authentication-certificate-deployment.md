---
title: استكشاف الأخطاء في نشر شهادة مصادقة العميل وإصلاحها
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1546"
- "9000076"
ms.openlocfilehash: 78520b416a72a3c93a3d2e7726948d59f83e681d4f09078c2a3cefac7bf1db3d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54020791"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a>استكشاف الأخطاء في نشر شهادة مصادقة العميل وإصلاحها

تستخدم ملفات تعريف شهادات عميل Intune NDES/SCEP و PKCS/PFX بشكل شائع بالتزامن مع أنواع ملفات التعريف الأخرى مثل Wifi و VPN والبريد الإلكتروني للسماح للمستخدمين بالمصادقة على موارد الشركة. عندما تكون أنواع ملفات التعريف هذه مرتبطة بملف تعريف شهادة عميل تعتمد على النشر الناجح لملف التعريف هذا.

غالبا ما يتطلب إعداد البنية الأساسية الأولية والتكوين المقترن لملف تعريف "شهادة العميل" استكشاف الأخطاء وإصلاحها. للحصول على دليل خطوة بخطوة لإعداد موصل NDES بنجاح وإرشادات استكشاف الأخطاء وإصلاحها لعزل المشاكل المتعلقة بنشر الشهادة، راجع: 

- [تكوين البنية الأساسية لدعم SCEP باستخدام Intune](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [نظرة عامة حول استكشاف ملفات تعريف شهادات SCEP وإصلاحها باستخدام Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

استخدم البرامج النصية المرجعية في powershell للمساعدة في التحقق من التكوين. لمزيد من المعلومات، راجع برامج التحقق من صحة موصل شهادة [Intune](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).

  
**المشاكل الشائعة الأخرى**

**عندما أحاول تثبيت موصل شهادة Intune على خادم موصل NDES، تظهر الرسالة "لا يمكن التحقق من كلمة المرور في طلب الشهادة. من الممكن أن يكون قد تم استخدامه بالفعل. احصل على كلمة مرور جديدة لإرسالها مع هذا الطلب."**  

تعني هذه الرسالة أنك تحتاج إلى تشغيل تثبيت موصل الشهادة كمسؤول.

في بعض البيئات، يجب أن تستخدم الخوادم التي يتم فيها تشغيل شهادة Intune خادما وكيلا للاتصال ب Intune، وبالتالي يجب أن يستخدم موصل الشهادة وكيلا. في بعض الحالات، يتجاهل موصل NDES إعدادات الوكيل التي تم تكوينها، وقد يكون من الضروري تكوين إعدادات الوكيل أثناء التشغيل في سياق الأمان في LocalSystem. 
 
الحل هو تشغيل Internet Explorer ك SYSTEM وتكوين وكيل في IE. بعد إعادة تشغيل خدمة موصل Intune، يتصل موصل NDES ب Intune.

**لم تعد أجهزة المستخدمين تتلقى شهادات SCEP من NDES.**

من المحتمل أن تكون شهادة مصادقة العميل الصادرة إلى خادم NDES، والمحددة أثناء تثبيت موصل NDES، قد انتهت صلاحيتها أو مفقودة. لحل هذه المشكلة: 
 
1. إلغاء تثبيت موصل NDES.  
2. استخدم هذه التفاصيل لطلب شهادة مصادقة عميل أو مصادقة خادم جديدة: 
 
    - اسم الموضوع: CN=external fqdn  
    - اسم الموضوع البديل (كلاهما مطلوب): DNS=fqdn الخارجي، DNS=fqdn الداخلي 
 
3. إعادة تثبيت موصل NDES بالشهادة الجديدة.