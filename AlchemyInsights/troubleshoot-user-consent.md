---
title: استكشاف الأخطاء وإصلاحها
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
- "9004353"
- "7785"
ms.openlocfilehash: 7249bafe1b047c66d9351a79f1782cfcc1a936a1
ms.sourcegitcommit: 7b213fd5e8a3fdb5c602673dc194d576d372ac96
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/18/2021
ms.locfileid: "49900781"
---
# <a name="troubleshoot-user-consent"></a><span data-ttu-id="9f7b3-102">استكشاف الأخطاء وإصلاحها</span><span class="sxs-lookup"><span data-stu-id="9f7b3-102">Troubleshoot user consent</span></span>

1. <span data-ttu-id="9f7b3-103">يمكنك تكوين الطريقة التي يتم بها الموافقة علي المستخدمين للتطبيقات عبر مدخل Azure أو PowerShell.</span><span class="sxs-lookup"><span data-stu-id="9f7b3-103">You can configure how end-users consent to applications through the Azure Portal or PowerShell.</span></span> <span data-ttu-id="9f7b3-104">راجع [إعدادات موافقه المستخدم](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) للحصول علي مزيد من المعلومات.</span><span class="sxs-lookup"><span data-stu-id="9f7b3-104">See [User consent settings](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) for more information.</span></span>
1. <span data-ttu-id="9f7b3-105">يمكن للمسؤول أيضا استخدام واجهه برمجه التطبيق الخاصة ب [Microsoft Graph](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) لمنح الموافقة علي الأذونات المفوضة بالنيابة عن مستخدم واحد.</span><span class="sxs-lookup"><span data-stu-id="9f7b3-105">An administrator can also use the [Microsoft Graph API](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) to grant consent to delegated permissions on behalf of a single user.</span></span> <span data-ttu-id="9f7b3-106">لمزيد من المعلومات ، راجع [الحصول علي حق الوصول بالنيابة عن مستخدم](https://docs.microsoft.com/graph/auth-v2-user).</span><span class="sxs-lookup"><span data-stu-id="9f7b3-106">For more information, see [Get access on behalf of a user](https://docs.microsoft.com/graph/auth-v2-user).</span></span>
1. <span data-ttu-id="9f7b3-107">[أخطاء الموافقة علي المستخدم](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error): تناقش هذه المقالة الأخطاء التي يمكن ان تحدث اثناء عمليه كونسينتينج إلى تطبيق.</span><span class="sxs-lookup"><span data-stu-id="9f7b3-107">[User Consent Errors](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error): this article discusses errors that can occur during the process of consenting to an application.</span></span> <span data-ttu-id="9f7b3-108">إذا كنت تقوم باستكشاف الأخطاء وإصلاحها ، لا تتضمن اي رسائل خطا ، راجع [سيناريوهات المصادقة ل AZURE AD](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).</span><span class="sxs-lookup"><span data-stu-id="9f7b3-108">If you are troubleshooting unexpected consent prompts that do not contain any error messages, see [Authentication Scenarios for Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).</span></span>