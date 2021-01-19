---
title: مشاكل الموافقة علي المسؤول
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
- "9004354"
- "7786"
ms.openlocfilehash: 6154b4b9cce51be3271cb25132f409319d8da14b
ms.sourcegitcommit: 113b802081101de70810fc73938ea92f7518d8c6
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/18/2021
ms.locfileid: "49900748"
---
# <a name="admin-consent-issues"></a><span data-ttu-id="f95cc-102">مشاكل الموافقة علي المسؤول</span><span class="sxs-lookup"><span data-stu-id="f95cc-102">Admin consent issues</span></span>

1. <span data-ttu-id="f95cc-103">تمكين [سير عمل الموافقة علي المسؤول](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) للسماح للمستخدمين بطلب موافقه المسؤول مباشره من شاشه الموافقة.</span><span class="sxs-lookup"><span data-stu-id="f95cc-103">Enable the [admin consent workflow](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) to allow users to request administrator approval directly from the consent screen.</span></span>

1. <span data-ttu-id="f95cc-104">إذا رايت أنت أو المستخدمون الذين لديهم أخطاء غير متوقعه اثناء عمليه الموافقة ، فراجع هذه المقالة لمعرفه الخطوات المتعلقة باستكشاف الأخطاء وإصلاحها: [خطا غير متوقع عند اجراء موافقه علي تطبيق](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).</span><span class="sxs-lookup"><span data-stu-id="f95cc-104">If you or your application's users are seeing unexpected errors during the consent process, see this article for troubleshooting steps: [Unexpected error when performing consent to an application](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).</span></span>

1. <span data-ttu-id="f95cc-105">تعرف علي [المزيد حول موافقه المسؤول علي النظام الأساسي للهوية من Microsoft](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent)، والطريقة التي تعمل بها [مطالبه الموافقة](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent) ، وكيفيه [تقييم طلب الموافقة علي المسؤول علي مستوي المستاجر](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent).</span><span class="sxs-lookup"><span data-stu-id="f95cc-105">Learn more about [Admin consent on the Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent), how the [consent prompt](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent) works, and how to [evaluate a request for tenant-wide admin consent](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent).</span></span>

1. <span data-ttu-id="f95cc-106">تتبع التطبيقات التي تتكامل مع النظام الأساسي لهويه Microsoft نموذج تخويل يمنح المستخدمين ويتحكم بالتحكم في كيفيه الوصول إلى البيانات.</span><span class="sxs-lookup"><span data-stu-id="f95cc-106">Applications that integrate with Microsoft identity platform follow an authorization model that gives users and administrators control over how data can be accessed.</span></span> <span data-ttu-id="f95cc-107">تم تحديث تطبيق نموذج التخويل علي نقطه نهاية النظام الأساسي لهويه Microsoft ، وهو يغير كيفيه تفاعل التطبيق مع النظام الأساسي للهوية Microsoft.</span><span class="sxs-lookup"><span data-stu-id="f95cc-107">The implementation of the authorization model has been updated on the Microsoft identity platform endpoint, and it changes how an app must interact with the Microsoft identity platform.</span></span> <span data-ttu-id="f95cc-108">اطلع علي [الأذونات والموافقة في نقطه نهاية النظام الأساسي لهويه Microsoft](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) للحصول علي نظره عامه حول نموذج التخويل هذا ، بما في ذلك النطاقات والأذونات والموافقة.</span><span class="sxs-lookup"><span data-stu-id="f95cc-108">See [Permissions and consent in the Microsoft identity platform endpoint](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) for an overview of this authorization model, including scopes, permissions, and consent.</span></span>