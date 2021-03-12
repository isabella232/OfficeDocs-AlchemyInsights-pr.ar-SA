---
title: مشاكل تتعلق بالمستأجرين
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7824"
- "9004325"
ms.openlocfilehash: 43f75564667bbb952076d4c12d7a1dd1e7e99731
ms.sourcegitcommit: 4e2d640a618c786700e8b276533554d51956f080
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/29/2021
ms.locfileid: "50713291"
---
# <a name="issues-with-tenants"></a><span data-ttu-id="dc6a7-102">مشاكل تتعلق بالمستأجرين</span><span class="sxs-lookup"><span data-stu-id="dc6a7-102">Issues with tenants</span></span>

<span data-ttu-id="dc6a7-103">ينظم Azure Active Directory (Azure AD) كائنات مثل المستخدمين والتطبيقات في مجموعات تسمى المستأجرين.</span><span class="sxs-lookup"><span data-stu-id="dc6a7-103">Azure Active Directory (Azure AD) organizes objects like users and apps into groups called tenants.</span></span> <span data-ttu-id="dc6a7-104">تسمح المستأجرات للمسؤول بتعيين سياسات على المستخدمين داخل المؤسسة والتطبيقات على التطبيقات التي تملكها المؤسسة لتلبية سياسات الأمان والتشغيل الخاصة بهم.</span><span class="sxs-lookup"><span data-stu-id="dc6a7-104">Tenants allow an administrator to set policies on the users within the organization and the on apps that the organization owns to meet their security and operational policies.</span></span> <span data-ttu-id="dc6a7-105">لمزيد من المعلومات، [راجع Tenancy في Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/develop/single-and-multi-tenant-apps)</span><span class="sxs-lookup"><span data-stu-id="dc6a7-105">For more information, see [Tenancy in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/single-and-multi-tenant-apps).</span></span>

<span data-ttu-id="dc6a7-106">لمزيد من المعلومات المتعلقة بإدارة المستأجر، راجع المقالات التالية:</span><span class="sxs-lookup"><span data-stu-id="dc6a7-106">For more information related to tenant management, see the following articles:</span></span>

- <span data-ttu-id="dc6a7-107">[سريع: إعداد مستأجر](https://docs.microsoft.com/azure/active-directory/develop/quickstart-create-new-tenant) - يعرض لك كيفية إنشاء مستأجر جديد.</span><span class="sxs-lookup"><span data-stu-id="dc6a7-107">[Quickstart: Set up a tenant](https://docs.microsoft.com/azure/active-directory/develop/quickstart-create-new-tenant) - Shows you how to create a new tenant.</span></span>

- <span data-ttu-id="dc6a7-108">[حذف مستأجر في Azure Active Directory](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto) - يعرض لك كيفية حذف مستأجر.</span><span class="sxs-lookup"><span data-stu-id="dc6a7-108">[Delete a tenant in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto) - Shows you how to delete a tenant.</span></span>

<span data-ttu-id="dc6a7-109">**مشاكل تتعلق بالمستأجرين المتعددين**</span><span class="sxs-lookup"><span data-stu-id="dc6a7-109">**Issues with multi-tenants**</span></span>

<span data-ttu-id="dc6a7-110">للحصول على معلومات حول كيفية إدارة المشاكل المتعلقة بتعدد المستأجرين، راجع المقالات التالية:</span><span class="sxs-lookup"><span data-stu-id="dc6a7-110">For information on how to manage issues regarding multi-tenants, see the following articles:</span></span>

- <span data-ttu-id="dc6a7-111">كيفية: تسجيل الدخول إلى أي مستخدم [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant) باستخدام نمط تطبيق متعدد المستأجرين - يظهر لك كيفية التحويل من مستأجر واحد إلى تطبيق متعدد المستأجرين.</span><span class="sxs-lookup"><span data-stu-id="dc6a7-111">[How to: Sign in any Azure Active Directory user using the multi-tenant application pattern](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant) - Shows you how to convert from a single-tenant to a multi-tenant application.</span></span>
- <span data-ttu-id="dc6a7-112">إعداد تسجيل الدخول إلى مؤسسة Azure Active Directory معينة في [Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/identity-provider-azure-ad-single-tenant?pivots=b2c-user-flow) - يظهر لك كيفية تمكين تسجيل الدخول للمستخدمين من مؤسسة Azure AD معينة باستخدام تدفق مستخدم في Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="dc6a7-112">[Set up sign-in for a specific Azure Active Directory organization in Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/identity-provider-azure-ad-single-tenant?pivots=b2c-user-flow) - Shows you how to enable sign-in for users from a specific Azure AD organization using a user flow in Azure AD B2C.</span></span>
- <span data-ttu-id="dc6a7-113">إعداد تسجيل الدخول إلى Azure Active Directory متعدد المستأجرين باستخدام نهج مخصصة في [Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/identity-provider-azure-ad-multi-tenant?pivots=b2c-custom-policy) يظهر لك كيفية تمكين تسجيل الدخول للمستخدمين باستخدام نقطة نهاية متعددة المستأجرين ل Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="dc6a7-113">[Set up sign-in for multi-tenant Azure Active Directory using custom policies in Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/identity-provider-azure-ad-multi-tenant?pivots=b2c-custom-policy)  shows you how to enable sign-in for users using the multi-tenant endpoint for Azure Active Directory (Azure AD).</span></span>






