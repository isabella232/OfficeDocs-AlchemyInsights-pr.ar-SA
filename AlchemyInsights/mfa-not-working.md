---
title: المشكلات المتعلقة بوزارة الخارجية
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: 2e79040c249b7825b964a19c51bcc42e5a6afb3f
ms.sourcegitcommit: 514ced512d0d7fff485b6fbf236cd27d6b4166e0
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/26/2019
ms.locfileid: "35250152"
---
# <a name="issues-with-mfa"></a>المشكلات المتعلقة بوزارة الخارجية
وهناك بضعة أشياء للتحقق من حالة المستخدمين لا يمكن تسجيل الدخول باستخدام مصادقة متعددة العوامل (وزارة الخارجية)

1. قد يتم حظر المستخدم المتأثر في موقع الدليل النشط Azure. إذا كان الأمر كذلك، محاولات المصادقة لمستخدم معين سيتم تلقائياً رفض. [الرجاء اتباع الخطوات الموجودة في هذه المقالة لإلغاء حظر هذه الملفات.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. إذا لم يساعد إلغاء منع المستخدم أو المستخدم غير محظور يمكنك محاولة إعادة تعيين ترتيب المنسوجات المتعددة الألياف للمستخدم وسوف تخرج من خلال عملية التسجيل مرة أخرى. [الرجاء اتباع الخطوات الموجودة في هذه المقالة.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

إذا كانت هذه هي المرة الأولى وزارة الخارجية الممكنة والمستخدمين غير قادر على تسجيل الدخول إلى عملاء غير مستعرضات مثل Outlook، Skype، وغيرها، ربما إنبات (مكتبة مصادقة الدليل النشط) غير ممكنة على الاشتراك O365. في هذه الحالة، ستحتاج إلى الاتصال Powershell Exchange عبر إنترنت وتشغيل الأمر cmdlet:  *مجموعة أورجانيزاتيونكونفيج-OAuth2ClientProfileEnabled: $true*