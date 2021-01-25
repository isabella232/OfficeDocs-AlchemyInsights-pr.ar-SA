---
title: أذونات API والموافقة عليها
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004343"
- "7756"
ms.openlocfilehash: c99e5e2e8fb9bcc88e5221890ed9c28ed9e7d0c8
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974177"
---
# <a name="api-permissions-and-consent"></a><span data-ttu-id="9e794-102">أذونات API والموافقة عليها</span><span class="sxs-lookup"><span data-stu-id="9e794-102">API permissions and consent</span></span>

<span data-ttu-id="9e794-103">تتبع التطبيقات التي تتكامل مع النظام الأساسي لهويه Microsoft نموذج تخويل يمنح المستخدمين ويتحكم بالتحكم في كيفيه الوصول إلى البيانات.</span><span class="sxs-lookup"><span data-stu-id="9e794-103">Applications that integrate with Microsoft identity platform follow an authorization model that gives users and administrators control over how data can be accessed.</span></span> <span data-ttu-id="9e794-104">تم تحديث تطبيق نموذج التخويل علي نقطه نهاية النظام الأساسي لهويه Microsoft.</span><span class="sxs-lookup"><span data-stu-id="9e794-104">The implementation of the authorization model has been updated on the Microsoft identity platform endpoint.</span></span> <span data-ttu-id="9e794-105">انه يغير كيفيه تفاعل التطبيق مع النظام الأساسي للهوية من Microsoft.</span><span class="sxs-lookup"><span data-stu-id="9e794-105">It changes how an app must interact with the Microsoft identity platform.</span></span> <span data-ttu-id="9e794-106">تغطي [الأذونات والموافقة في نقطه نهاية النظام الأساسي لهويه Microsoft](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) المفاهيم الاساسيه لنموذج التخويل هذا ، بما في ذلك النطاقات والأذونات والموافقة.</span><span class="sxs-lookup"><span data-stu-id="9e794-106">[Permissions and consent in the Microsoft identity platform endpoint](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) covers the basic concepts of this authorization model, including scopes, permissions, and consent.</span></span>

<span data-ttu-id="9e794-107">يسهل [اطار الموافقة علي Azure Active directory (AZURE AD)](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) تطوير تطبيقات العميل المتعددة علي ويب والمستاجرين.</span><span class="sxs-lookup"><span data-stu-id="9e794-107">The [Azure Active Directory (Azure AD) consent framework](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) makes it easy to develop multi-tenant web and native client applications.</span></span> <span data-ttu-id="9e794-108">تسمح هذه التطبيقات بتسجيل الدخول بواسطة حسابات المستخدمين من مستاجر Azure AD والتي تختلف عن تلك التي تم تسجيل التطبيق فيها.</span><span class="sxs-lookup"><span data-stu-id="9e794-108">These applications allow sign-in by user accounts from an Azure AD tenant that's different from the one where the application is registered.</span></span> <span data-ttu-id="9e794-109">قد يحتاج أيضا إلى الوصول إلى واجات برمجه التطبيقات علي الويب مثل Microsoft Graph API (للوصول إلى Azure AD و Intune والخدمات في Microsoft 365) وغيرها من واجات برمجه تطبيقات Microsoft services الأخرى ، بالاضافه إلى واجات برمجه تطبيقات ويب الخاصة بك.</span><span class="sxs-lookup"><span data-stu-id="9e794-109">They may also need to access web APIs such as the Microsoft Graph API (to access Azure AD, Intune, and services in Microsoft 365) and other Microsoft services' APIs, in addition to your own web APIs.</span></span>

