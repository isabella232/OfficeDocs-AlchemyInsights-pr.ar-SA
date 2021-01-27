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
ms.openlocfilehash: 4df9a98644f6bc7a30f9009719c5198db591afc9
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/27/2021
ms.locfileid: "50014708"
---
# <a name="delete-or-restore-applications"></a>حذف التطبيقات أو استعادتها

**لحذف تطبيق من مستاجر AZURE AD**:

1. في **مدخل AZURE AD**، حدد **تطبيقات المؤسسة**. ثم ابحث عن التطبيق الذي تريد حذفه وحدده.
2. في المقطع **أداره** في الجزء الأيمن ، حدد **خصائص**.
3. حدد **حذف**، ثم حدد **نعم** لتاكيد رغبتك في حذف التطبيق من مستاجر Azure AD.

للحصول علي مزيد من المعلومات حول كيفيه حذف تطبيق ، راجع [تشغيل: حذف تطبيق من مستاجر Azure Active directory (AZURE AD)](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant).

في PowerShell ، يزيل الأمر [أزوريدابليكاتيونبروكسيابليكيشن](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) cmdlet تكوينات وكيل التطبيق من تطبيق معين في Azure Active directory ، ويمكنه حذف التطبيق بالبالكامل إذا تم تحديده.

يمكنك **استعاده تطبيق محذوف** باستخدام PowerShell. بمجرد تحديد التطبيق الذي تريد استعادته ، يمكنك استعادته باستخدام [أزوريديليتيدابليكيشن](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication).
