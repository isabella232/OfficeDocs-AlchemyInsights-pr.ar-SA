---
title: استكشاف الأخطاء في SSPR وإصلاحها
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/04/2021
ms.topic: article
ms.audience: Admin
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "6128"
ms.openlocfilehash: 85bfc812dcffce008a6fa5394a6069bd64c514d6
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429284"
---
# <a name="troubleshoot-sspr"></a>استكشاف الأخطاء في SSPR وإصلاحها

**أواجه مشكلة في تكوين إعادة تعيين كلمة المرور**

- إذا كنت مسؤولا وتبحث عن كيفية تمكين إعادة تعيين كلمة المرور ذاتي الخدمة، فشاهد البرنامج التعليمي لتمكين [SSPR،](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr)لتكوين إعادة تعيين كلمة المرور لم مؤسستك. قد تحتاج أيضا إلى مراجعة [متطلبات الترخيص.](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-licensing?WT.mc_id=Portal-Microsoft_Azure_Support) يجب أن يكون لديك ترخيص واحد على الأقل تم تعيينه في مؤسستك.
    - **مستخدمو السحابة فقط** - أي SKU مدفوعة من Office 365 (O365) أو Azure AD Basic
    - المستخدمون في السحابة **و/أو** المحليون - Azure AD Premium P1 أو P2 أو Enterprise Mobility + Security (EMS) أو Secure Productive Enterprise (SPE)
- لمزيد من الأسئلة حول إعادة تعيين كلمة مرور الخدمة الذاتية، راجع [الأسئلة الشائعة.](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-faq?WT.mc_id=Portal-Microsoft_Azure_Support)

**أتلقى رسالة خطأ**

راجع هذه المقالة للعثور على الأخطاء الشائعة وحلولها: استكشاف أخطاء إعادة تعيين كلمة مرور الخدمة الذاتية [وإصلاحها](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support)

**أواجه مشكلة في نهج إعادة تعيين كلمة المرور**

- إذا لم يكن نهج إعادة تعيين كلمة المرور قيد التشغيل كما هو متوقع، أو إذا كانت لديك أسئلة حول نهج إعادة تعيين كلمة المرور، فراجع هذه المقالة: نهج كلمات المرور والقيود في [Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support)
- لا تنطبق سياسات إعادة تعيين كلمة المرور على المسؤولين. تفرض Microsoft نهج إعادة تعيين كلمة مرور افتراضية وقوية ذات بوابة لأي دور مسؤول Azure. تأكد من أنك تقوم باختباره مع مستخدم ليس مسؤولا. لمزيد من المعلومات حول نهج إعادة تعيين المسؤول، راجع هذه المقالة: إعادة تعيين المسؤول [لاختلافات النهج.](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-reset-policy-differences)

**لا أريد أن يسجل المستخدمون معلومات أمان إضافية لإعادة تعيين كلمة المرور**

يمكنك تعبئة البيانات مسبقا (سمات البريد الإلكتروني والهاتف) للمستخدمين باستخدام API أو PowerShell أو Azure AD Connect. لمعرفة كيفية القراءة:

- [نشر إعادة تعيين كلمة المرور دون مطالبة المستخدمين بالتسجيل](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support#set-and-read-authentication-data-using-powershell)
- [البيانات التي تستخدمها إعادة تعيين كلمة المرور](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**أريد أن يسجل المستخدمون معلومات الأمان الإضافية لإعادة تعيين كلمة المرور**

1. يجب على المستخدمين تسجيل معلومات الأمان لإعادة تعيين كلمة مرور الخدمة الذاتية عن طريق توجيههم إلى [aka.ms/ssprsetup.](https://mysignins.microsoft.com/security-info)
1. بعد تعبئة البيانات للمستخدم (بواسطة المستخدم أو المسؤول)، قم توجيه [](https://passwordreset.microsoftonline.com/) المستخدم إلى aka.ms/sspr بحيث يمكن تمكين المستخدمين من إعادة تعيين كلمات المرور الخاصة بهم.
1. إذا كان المستخدمون لا يزالوا  يعانون من مشاكل، فهم على المرجح أن يكونوا مستخدمين موحوحين أو مزامنتهم بكلمات **مرور.** وهذا يعني أنه من المرجح وجود مشكلة في خدمة "كتابة كلمة المرور".