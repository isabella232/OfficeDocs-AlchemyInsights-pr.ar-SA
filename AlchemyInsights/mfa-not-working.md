---
title: قضايا مع وزاره الخارجية
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
ms.openlocfilehash: a415116b9ba437cb13426896119cd1b40d9ab491
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/29/2019
ms.locfileid: "37768824"
---
# <a name="issues-with-azure-mfa"></a>قضايا مع وزاره الخارجية Azure
هناك بضعة أشياء للتحقق ما إذا كان المستخدمين لا يمكن تسجيل الدخول باستخدام المصادقة متعددة العوامل (وزاره الخارجية)

1. قد يتم حظر المستخدم المتاثر في موقع الدليل النشط Azure. إذا كانت هذه هي الحالة ، سيتم تلقائيا رفض محاولات المصادقة لهذا المستخدم المحدد. [الرجاء اتباع الخطوات التالية في هذه المقالة للغاء حظرها.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. إذا كان إلغاء حظر المستخدم لم يساعد أو لم يتم حظر المستخدم يمكنك محاولة أعاده تعيين وزاره الخارجية للمستخدم وانها سوف تذهب من خلال عمليه التسجيل مره أخرى. [الرجاء اتباع الخطوات التالية في هذه المقالة.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

إذا كانت هذه هي المرة الاولي التي قمت بتمكين وزاره الخارجية والمستخدمين غير قادرين علي تسجيل الدخول إلى العملاء غير المستعرضات مثل Outlook ، سكايب ، وما إلى ذلك ، وربما لم يتم تمكين ال (مكتبه مصادقه الدليل النشط) علي الاشتراك O365 الخاص بك. في هذه الحالة سوف تحتاج إلى الاتصال Powershell Exchange عبر الإنترنت وتشغيل هذا cmdlet:  *مجموعه-اورجانيزاتيونكونفيج-OAuth2ClientProfileEnabled: $true*