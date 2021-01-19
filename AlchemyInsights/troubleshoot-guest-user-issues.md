---
title: استكشاف مشاكل المستخدم الضيف وإصلاحها
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
ms.openlocfilehash: 0f2a10b918fee067b167ab58ac2544a89e0c8ea1
ms.sourcegitcommit: 7b213fd5e8a3fdb5c602673dc194d576d372ac96
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/18/2021
ms.locfileid: "49900754"
---
# <a name="troubleshoot-guest-user-issues"></a>استكشاف مشاكل المستخدم الضيف وإصلاحها

1. للحصول علي إرشادات حول أداره وصول الضيوف إلى التطبيقات ، راجع [أداره الوصول إلى الضيوف باستخدام مراجعات AZURE AD access](https://docs.microsoft.com/azure/active-directory/governance/manage-guest-access-with-access-reviews).
1. [أضافه مستخدمين ضيوف إلى الدليل في مدخل azure](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal): في هذا التشغيل ، ستقوم باضافه مستخدم ضيف جديد إلى دليلك في azure AD عبر مدخل azure ، وإرسال دعوه ، ويمكنك رؤية المظهر الذي ستبدو عليه عمليه استرداد الدعوة الخاصة بالمستخدم الضيف.
1. [أضافه مستخدم ضيف باستخدام PowerShell](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-invite-powershell): في هذا التشغيل ، ستستخدم الأمر New-AzureADMSInvitation لأضافه مستخدم ضيف واحد إلى مستاجر Azure.
1. لمعرفه كيفيه تعيين المستخدمين والمجموعات إلى تطبيقات المؤسسة في Azure Active Directory (Azure AD) ، من داخل مدخل Azure أو باستخدام PowerShell ، راجع [أداره تعيين المستخدم لتطبيق في Azure Active](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal)directory. 
1. تعمل التعاون في azure Active Directory (Azure AD) مع معظم التطبيقات التي تتكامل مع Azure AD. في هذه [المقالة](https://docs.microsoft.com/azure/active-directory/external-identities/configure-saas-apps)، سنقوم بالإرشادات المتعلقة بتكوين بعض تطبيقات ميناء الشائعة لاستخدامها مع AZURE AD B2B.
1. بصفتك مؤسسه تستخدم إمكانيات التعاون الخاصة ب Azure Active directory (Azure AD) لدعوه المستخدمين الضيوف من مؤسسات الشركاء إلى Azure AD ، يمكنك الآن توفير امكانيه الوصول لمستخدمي B2B هذه إلى التطبيقات المحلية. بإمكان هذه التطبيقات المحلية استخدام المصادقة المستندة إلى SAML أو مصادقه Windows المتكاملة (أيوا) مع تفويض Kerberos المقيد (ككد). للحصول علي مزيد من المعلومات ، راجع [منح المستخدمين في AZURE AD حق الوصول إلى التطبيقات المحلية](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-cloud-to-on-premises).
1. تعرف علي كيفيه [منح حسابات شركاء مداره محليا الوصول إلى موارد السحابة باستخدام التعاون في AZURE AD B2B](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-on-premises-to-cloud).