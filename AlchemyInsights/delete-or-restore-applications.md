---
title: حذف التطبيقات أو استعادتها
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004335"
- "7737"
ms.openlocfilehash: 0c7be98650ca87f36b66f0bb38fb665fc81525b7f3410da14b99fb67468c1e73
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54102558"
---
# <a name="delete-or-restore-applications"></a>حذف التطبيقات أو استعادتها

**لحذف تطبيق من مستأجر Azure AD:**

1. في مدخل **Azure AD ،** حدد **تطبيقات المؤسسة**. ثم ابحث عن التطبيق الذي تريد حذفه وحدده.
2. في المقطع **إدارة** في الجزء الأيسر، حدد **خصائص**.
3. حدد **حذف**، ثم حدد **نعم** لتأكيد أنك تريد حذف التطبيق من مستأجر Azure AD.

لمزيد من المعلومات حول كيفية حذف تطبيق، راجع تشغيل سريع: حذف تطبيق من مستأجر [Azure Active Directory (Azure AD).](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant)

في PowerShell، يزيل الأمر [cmdlet Remove-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) تكوينات وكيل التطبيق من تطبيق معين في Azure Active Directory، ويمكنه حذف التطبيق بالكامل إذا تم تحديده.

يمكنك استعادة **تطبيق محذوف** باستخدام PowerShell. بمجرد تحديد التطبيق الذي تريد استعادته، يمكنك استعادته باستخدام [Restore-AzureADDeletedApplication](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication).
