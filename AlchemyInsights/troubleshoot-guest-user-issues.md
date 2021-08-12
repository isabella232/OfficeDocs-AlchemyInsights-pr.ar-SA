---
title: استكشاف مشاكل المستخدمين الضيوف وإصلاحها
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004358"
- "7822"
ms.openlocfilehash: 9e6030919721b4c0805a26ca45d365f31d88894e86ea08225f47576e7d152047
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53939366"
---
# <a name="troubleshoot-guest-user-issues"></a>استكشاف مشاكل المستخدمين الضيوف وإصلاحها

1. للحصول على إرشادات حول إدارة وصول الضيف إلى التطبيقات، راجع إدارة وصول الضيف [باستخدام مراجعات الوصول إلى Azure AD](https://docs.microsoft.com/azure/active-directory/governance/manage-guest-access-with-access-reviews).
1. إضافة مستخدمين ضيوف إلى دليلك في مدخل [Azure](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal): في هذه العملية السريعة، ستضيف مستخدما ضيفا جديدا إلى دليل Azure AD عبر مدخل Azure، وأرسل دعوة، وشاهد كيف تبدو عملية استرداد دعوة المستخدم الضيف.
1. [إضافة مستخدم ضيف باستخدام PowerShell](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-invite-powershell): في هذا New-AzureADMSInvitation السريع، يمكنك استخدام الأمر New-AzureADMSInvitation لإضافة مستخدم ضيف واحد إلى مستأجر Azure.
1. للتعرف على كيفية تعيين مستخدمين ومجموعات لتطبيقات المؤسسة في Azure Active Directory (Azure AD)، إما من داخل مدخل Azure أو باستخدام PowerShell، راجع إدارة تعيين المستخدم لتطبيق في [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal). 
1. يعمل تعاون Azure Active Directory (Azure AD) B2B مع معظم التطبيقات التي تتكامل مع Azure AD. في هذه [المقالة](https://docs.microsoft.com/azure/active-directory/external-identities/configure-saas-apps)، نمشي عبر إرشادات لتكوين بعض تطبيقات SaaS الشائعة لاستخدامها مع Azure AD B2B.
1. كمنظمة تستخدم Azure Active Directory (Azure AD) قدرات التعاون B2B لدعوة المستخدمين الضيوف من المؤسسات الشريكة إلى Azure AD، يمكنك الآن توفير حق الوصول لمستخدمي B2B هؤلاء إلى التطبيقات المحلية. يمكن لهذه التطبيقات المحليه استخدام المصادقة المستندة إلى SAML أو المصادقة Windows (IWA) مع Kerberos المقيدة (KCD). لمزيد من المعلومات، راجع [منح مستخدمي B2B في Azure AD](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-cloud-to-on-premises)حق الوصول إلى التطبيقات الخاصة بك في الموقع.
1. تعرف على كيفية منح حسابات الشركاء المدارة محليا حق الوصول إلى موارد السحابة [باستخدام تعاون Azure AD B2B](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-on-premises-to-cloud).