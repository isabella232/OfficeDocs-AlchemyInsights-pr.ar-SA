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
ms.openlocfilehash: 2fed99ebf553a9bfda436d81797c841987759e98
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51810471"
---
# <a name="issues-with-azure-mfa"></a>مشاكل في Azure MFA
هناك بعض الأمور التي يجب التحقق مما إذا كان المستخدمون لا يمكنهم تسجيل الدخول باستخدام المصادقة متعددة العوامل (MFA)

1. قد يتم حظر المستخدم المتأثر في مدخل Azure Active Directory. إذا كان الأمر كذلك، سيتم رفض محاولات المصادقة لهذا المستخدم المحدد تلقائيا. [الرجاء اتباع الخطوات في هذه المقالة إلغاء حظرها.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. إذا لم يساعد إلغاء حظر المستخدم أو لم يتم حظر المستخدم، يمكنك محاولة إعادة تعيين MFA للمستخدم وسيخوض عملية التسجيل مرة أخرى. [الرجاء اتباع الخطوات في هذه المقالة.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

إذا كانت هذه هي المرة الأولى التي تقوم فيها بتمكين المصادقة متعددة العوامل (MFA) ويتمكن المستخدمون من تسجيل الدخول إلى عملاء لا تستخدم المستعرضات مثل Outlook وسكايب وغير ذلك، ربما لم يتم تمكين ADAL (مكتبة مصادقة Active Directory) في اشتراك O365. في هذه الحالة، ستحتاج إلى الاتصال ب Exchange Online Powershell وتشغيل الأمر cmdlet هذا:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*