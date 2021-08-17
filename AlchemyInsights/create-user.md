---
title: إنشاء مستخدم
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003231"
- "9403"
ms.openlocfilehash: afba00ffc6ba082606e0071b41e2917b11e6a39d61cd0df7e468f0238f2ed8e8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54118731"
---
# <a name="create-user"></a>إنشاء مستخدم

**الإعلان:**

- إهمال دعم تسجيل الدخول إلى WebView من Google بدءا من 4 يناير [2021](/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support) . اختبر ما إذا كانت تطبيقاتك قد تتأثر باتباع إرشادات [Google](https://go.microsoft.com/fwlink/?linkid=2157323) حول اختبار التوافق.
- تأكد من استخدام عرض ويب للنظام أو مستعرض النظام عند تسجيل الدخول إلى المستخدمين باستخدام حسابات Google للمستهلكين. لمزيد من المعلومات، راجع مشاكل تسجيل الدخول إلى [التطبيق (التطبيقات) باستخدام مستعرض Chrome فقط](/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications).

**لا يمكنني إنشاء مستخدم جديد في دليل Azure AD**

1. تأكد من أنك م مخولا لإنشاء مستخدم قياسي جديد. يمكن فقط لدور المسؤول العام أو مسؤول المستخدم في Azure Active Directory (AD) إنشاء مستخدم قياسي جديد. إذا لم تكن في أحد هذه الأدوار، فاطلب من المسؤول إضافتك إلى أحد هذه الأدوار أو إنشاء حساب مستخدم جديد لك.
1. تأكد من أن اسم المستخدم في مجال تم التحقق منه في Azure AD. إذا لم يكن لديك أي أسماء مجالات مخصصة متحقق منها في Azure AD، يمكنك استخدام مجال Azure AD الأولي، الذي ينتهي ب *.onmicrosoft.com.
1. تأكد من أن اسم المستخدم في مجال غير متكاتف مع Azure AD من AD الخاص بك. لا يمكن إضافة المستخدمين في السحابة مع أسماء المجالات التي يتم تدائمها من الأسماء في الموقع.
1. تأكد من عدم وجود اسم مستخدم أو جهة اتصال أخرى تريد تعيينه إلى المستخدم الجديد. يجب أن تكون أسماء المستخدمين فريدة عبر Azure AD.
1. راجع [أدوار Azure AD والمسؤولين](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) ل Azure AD.
1. راجع [أسماء مجالات](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) Azure AD.
1. راجع [سجلات التدقيق](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) لرؤية معلومات أكثر تفصيلا حول مستخدم تم إنشاؤه أو حذفه مؤخرا مثل الشخص الذي قام بتنفيذ الإجراء ومتى.
1. لمزيد من المعلومات حول إضافة مستخدمين جدد، راجع استخدام مدخل Azure لإنشاء مستخدم [جديد في Azure AD](/azure/active-directory/active-directory-users-create-azure-portal).
1. [أدوار Azure AD الإدارية](/azure/active-directory/active-directory-assign-admin-roles): أذونات دور المسؤول في Azure Active Directory
1. يمكنك أيضا [استخدام Azure AD PowerShell لإنشاء مستخدم جديد](/powershell/module/azuread/new-azureaduser?view=azureadps-2.0).
