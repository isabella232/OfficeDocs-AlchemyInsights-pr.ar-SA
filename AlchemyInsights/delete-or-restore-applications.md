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
# <a name="delete-or-restore-applications"></a><span data-ttu-id="5fe9b-102">حذف التطبيقات أو استعادتها</span><span class="sxs-lookup"><span data-stu-id="5fe9b-102">Delete or restore applications</span></span>

<span data-ttu-id="5fe9b-103">**لحذف تطبيق من مستاجر AZURE AD**:</span><span class="sxs-lookup"><span data-stu-id="5fe9b-103">**To delete an application from your Azure AD tenant**:</span></span>

1. <span data-ttu-id="5fe9b-104">في **مدخل AZURE AD**، حدد **تطبيقات المؤسسة**.</span><span class="sxs-lookup"><span data-stu-id="5fe9b-104">In the **Azure AD portal**, select **Enterprise applications**.</span></span> <span data-ttu-id="5fe9b-105">ثم ابحث عن التطبيق الذي تريد حذفه وحدده.</span><span class="sxs-lookup"><span data-stu-id="5fe9b-105">Then find and select the application you want to delete.</span></span>
2. <span data-ttu-id="5fe9b-106">في المقطع **أداره** في الجزء الأيمن ، حدد **خصائص**.</span><span class="sxs-lookup"><span data-stu-id="5fe9b-106">In the **Manage** section in the left pane, select **Properties**.</span></span>
3. <span data-ttu-id="5fe9b-107">حدد **حذف**، ثم حدد **نعم** لتاكيد رغبتك في حذف التطبيق من مستاجر Azure AD.</span><span class="sxs-lookup"><span data-stu-id="5fe9b-107">Select **Delete**, and then select **Yes** to confirm you want to delete the app from your Azure AD tenant.</span></span>

<span data-ttu-id="5fe9b-108">للحصول علي مزيد من المعلومات حول كيفيه حذف تطبيق ، راجع [تشغيل: حذف تطبيق من مستاجر Azure Active directory (AZURE AD)](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant).</span><span class="sxs-lookup"><span data-stu-id="5fe9b-108">For more information on how to delete an app, see [Quickstart: Delete an application from your Azure Active Directory (Azure AD) tenant](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant).</span></span>

<span data-ttu-id="5fe9b-109">في PowerShell ، يزيل الأمر [أزوريدابليكاتيونبروكسيابليكيشن](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) cmdlet تكوينات وكيل التطبيق من تطبيق معين في Azure Active directory ، ويمكنه حذف التطبيق بالبالكامل إذا تم تحديده.</span><span class="sxs-lookup"><span data-stu-id="5fe9b-109">In PowerShell, the [Remove-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) cmdlet removes Application Proxy configurations from a specific application in Azure Active Directory, and can delete the application completely if specified.</span></span>

<span data-ttu-id="5fe9b-110">يمكنك **استعاده تطبيق محذوف** باستخدام PowerShell.</span><span class="sxs-lookup"><span data-stu-id="5fe9b-110">You can **restore a deleted application** using PowerShell.</span></span> <span data-ttu-id="5fe9b-111">بمجرد تحديد التطبيق الذي تريد استعادته ، يمكنك استعادته باستخدام [أزوريديليتيدابليكيشن](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication).</span><span class="sxs-lookup"><span data-stu-id="5fe9b-111">Once the application you want to restore has been identified, you can restore it using [Restore-AzureADDeletedApplication](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication).</span></span>
