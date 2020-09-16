---
title: المشاكل المتعلقة بالMFA
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: 718af9bfbc0a64cdfc96528e5062fb96c8d0f2d3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47755118"
---
# <a name="issues-with-azure-mfa"></a>المشاكل المتعلقة باستخدام Azure MFA
هناك بعض الأمور التي يجب التحقق من عدم تمكن المستخدمين من تسجيل الدخول باستخدام مصادقه متعددة العوامل (MFA)

1. قد يكون المستخدم المتاثر محظورا في مدخل Azure Active directory. إذا كانت هذه هي الحالة ، سيتم رفض محاولات المصادقة لهذا المستخدم المحدد تلقائيا. [الرجاء اتباع الخطوات المذكورة في هذه المقالة للغاء حظرها.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. إذا لم يساعدك إلغاء حظر المستخدم أو إذا لم يتم حظر المستخدم ، فيمكنك محاولة أعاده تعيين MFA للمستخدم سيمر علي عمليه التسجيل مره أخرى. [الرجاء اتباع الخطوات الواردة في هذه المقالة.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

إذا كانت هذه هي المرة الاولي التي تقوم فيها بتمكين MFA وكان المستخدمون غير قادرين علي تسجيل الدخول إلى العملاء الذين لا يستخدمون برنامج Outlook ، أو Skype ، وغير ذلك ، فهذا يعني انه لم يتم تمكين الأمر ADAL (مكتبه مصادقه Active directory) علي اشتراكك في O365. في هذه الحالة ستحتاج إلى الاتصال ب Exchange Online Powershell وتشغيل أمر cmdlet هذا:  *Set-get-organizationconfig-OAuth2ClientProfileEnabled: $true*