---
title: نهج حماية التطبيقات
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/22/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1073"
- "6700006"
ms.openlocfilehash: 929400dcf0ca18ce8f52cb11e5c907064449480e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47716880"
---
# <a name="application-protection-policy"></a>نهج حماية التطبيقات

إذا كنت جديدا في نهج حماية التطبيقات (التطبيق) ، فراجع [نظره عامه حول نهج حماية التطبيق](https://docs.microsoft.com/intune/apps/app-protection-policy).

لبدء استخدام التطبيق ، راجع [كيفيه إنشاء نهج حماية التطبيق وتعيينها](https://docs.microsoft.com/intune/app-protection-policies).

متطلبات نهج حماية التطبيق:

- يملك المستخدم ترخيص Intune أو EMS.
- ينتمي المستخدم إلى مجموعه مستهدفه بواسطة نهج حماية التطبيق.
- يتم تسجيل دخول مستخدم واحد فقط للشركات إلى تطبيقات محمية علي جهاز.
- قام التطبيق بتنفيذ [INTUNE SDK](https://docs.microsoft.com/intune/app-sdk-get-started). للحصول علي قائمه بالتطبيقات التي تدعم SDK ، راجع [التطبيقات المحمية في Microsoft Intune](https://docs.microsoft.com/intune/apps-supported-intune-apps).

يتم تطبيق النهج بعد قيام المستخدم الذي يلبي المتطلبات أعلاه بتسجيل الدخول إلى تطبيق تم تمكينه في Intune SDK. تتمثل أسهل طريقه لتحديد ما إذا كان النهج مطبقا بالطلب ان يقوم المستخدم بتعيين رقم pin في النهج. 

لمزيد من المعلومات، اطلع على:

[الاسئله المتداولة حول التطبيق/الMAM](https://docs.microsoft.com/intune/apps/troubleshoot-mam)  

[كيفيه التحقق من صحة اعداد نهج حماية التطبيق](https://docs.microsoft.com/intune/app-protection-policies-validate)

[فهم توقيت تسليم نهج حماية التطبيق](https://docs.microsoft.com/intune/app-protection-policy-delivery)  

[كيفيه مراقبه نهج حماية التطبيق](https://docs.microsoft.com/intune/app-protection-policies-monitor)