---
title: مشاكل في MFA
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: b39c79063c66ea41585c8f9eec372bfac77bc0aa29ded5a5572e06c141b28f80
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54098589"
---
# <a name="issues-with-azure-mfa"></a>مشاكل في Azure MFA
هناك بعض الأمور التي يجب التحقق مما إذا كان المستخدمون لا يمكنهم تسجيل الدخول باستخدام المصادقة متعددة العوامل (MFA)

1. قد يتم حظر المستخدم المتأثر في مدخل Azure Active Directory. إذا كان الأمر كذلك، سيتم رفض محاولات المصادقة لهذا المستخدم المحدد تلقائيا. [الرجاء اتباع الخطوات في هذه المقالة إلغاء حظرها.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. إذا لم يساعد إلغاء حظر المستخدم أو لم يتم حظر المستخدم، يمكنك محاولة إعادة تعيين MFA للمستخدم وسيخوض عملية التسجيل مرة أخرى. [الرجاء اتباع الخطوات في هذه المقالة.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

إذا كانت هذه هي المرة الأولى التي تقوم فيها بتمكين المصادقة متعددة العوامل (MFA) ويتمكن المستخدمون من تسجيل الدخول إلى عملاء لا تستخدم المستعرضات مثل Outlook أو Skype أو غير ذلك، ربما لم يتم تمكين ADAL (مكتبة مصادقة Active Directory) في اشتراك O365. في هذه الحالة، ستحتاج إلى الاتصال Exchange Online Powershell وتشغيل الأمر cmdlet هذا: *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*