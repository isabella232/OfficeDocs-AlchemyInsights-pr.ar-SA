---
title: مشاكل إدارة المستخدمين
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9209"
- "9005371"
ms.openlocfilehash: 4b61686381de0cafa38857ca7a96b3a81aa191ec
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/19/2021
ms.locfileid: "51034815"
---
# <a name="user-management-issues"></a>مشاكل إدارة المستخدمين

**ماذا يحدث للمستخدمين المعينين حاليا للتطبيق إذا قمت بتعطيل الخاصية "تعيين المستخدم مطلوب" (قم بتعيين هذه الخاصية إلى لا)؟**

لا يؤثر **تعطيل تعيين** المستخدم المطلوب على المستخدمين المعينين حاليا. سيسمح تعطيل هذه الخاصية فقط لجميع المستخدمين بالوصول إلى التطبيق. وسيبقى جميع المستخدمين المدرجين والمستخدمين المعينين إلى مجموعات في التطبيق صالحين.

- لتقييد تطبيقك إلى مجموعة معينة من المستخدمين، راجع - تقييد تطبيق Azure AD إلى مجموعة من المستخدمين - النظام الأساسي [لهوية Microsoft | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/develop/howto-restrict-your-app-to-a-set-of-users#:~:text=Select%20the%20application%20you%20want%2cand%20set%20it%20to%20Yes.).
- لتعيين المستخدمين والمجموعات، لتطبيقات المؤسسة في Azure Active Directory (Azure AD)، إما من داخل مدخل Azure أو باستخدام PowerShell، راجع إدارة تعيين المستخدم لتطبيق في [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal).
- لتفويض أذونات إنشاء التطبيق وإدارته، راجع تفويض أذونات مسؤول إدارة التطبيقات [- Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/roles/delegate-app-roles).
- **إخفاء تطبيقات المؤسسة المحددة عن المستخدمين** - استخدم الخطوات التالية لإخفاء جميع تطبيقات Microsoft 365 من لوحة **MyApps.** وستبقى التطبيقات مرئية في مدخل Office 365.

 1. سجل الدخول إلى مدخل Azure كمسؤول عام للدراج. 
 2. حدد **Azure Active Directory**. 
 3. حدد **المستخدمون**. 
 4. حدد **إعدادات المستخدم**. 
 5. ضمن **تطبيقات المؤسسة،** انقر فوق **إدارة كيفية تشغيل المستخدمين النهائيين للتطبيقات وعرضها**. 
 6. بالنسبة **للمستخدمين، يمكنهم رؤية تطبيقات Office 365 فقط في مدخل Office 365،** انقر فوق **نعم**. 
 7. انقر فوق **حفظ**. 
 8. لمزيد من التفاصيل، راجع إخفاء تطبيق Enterprise من تجربة المستخدم [في Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/manage-apps/hide-application-from-user-portal#:~:text=%20Hide%20an%20application%20from%20the%20end%20user,6%20Click%20Properties.%207%20Click%20Save.%20See%20More.)

- إذا كنت تعرض تطبيق "برامج" كخدمة (SaaS) للعديد من المؤسسات، يمكنك تكوين تطبيقك لقبول تسجيل الدخول من أي مستأجر Azure Active Directory (Azure AD). يسمى هذا التكوين "جعل تطبيقك متعدد المستأجرين". وسيتمكن المستخدمون في أي مستأجر Azure AD من تسجيل الدخول إلى تطبيقك بعد الموافقة على استخدام حسابهم مع تطبيقك. لمزيد من المعلومات، راجع إنشاء التطبيقات التي تقوم تسجيل الدخول إلى [مستخدمي Azure AD - النظام الأساسي لهوية Microsoft | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant).

- **كيف يمكن للمستخدم الوصول إلى التطبيق بمجرد تعيينه للتطبيق؟**

يحتوي كل تطبيق في شفرة تطبيق Enterprise على ارتباط يمكن للمستخدمين الوصول إليه. يمكن للمستخدمين أيضا الوصول إلى التطبيق من خلال **مدخل Myapps** بطريقة سهلة.

- **هل تريد معرفة التطبيقات ونوع التطبيقات التي يستخدمها المستخدمون؟**

يمكنك تنزيل تقارير تسجيل الدخول خلال آخر 30 يوما من portal.azure.com > **Azure Active directory**> Signins> تقارير التنزيل.

- تعرف على كيفية منح موافقة المسؤول على نطاق [المستأجر لتطبيق](https://docs.microsoft.com/azure/active-directory/manage-apps/grant-admin-consent) وتكوين كيفية موافقة [المستخدمين النهائيين على التطبيقات.](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent)

- فهم [كيفية عمل الموافقة](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) وإدارة الموافقة على [التطبيقات](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests).


