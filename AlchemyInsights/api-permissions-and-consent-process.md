---
title: أذونات API وعملية الموافقة
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004345"
- "9200"
ms.openlocfilehash: 23fed786e7b33adf0b6c76fc71a7e69f2cfcceb7
ms.sourcegitcommit: e5f261f95ffc6074cce89e62ef8c4e9fd519d3ee
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/26/2021
ms.locfileid: "51404163"
---
# <a name="api-permissions-and-consent-process"></a><span data-ttu-id="aaec8-102">أذونات API وعملية الموافقة</span><span class="sxs-lookup"><span data-stu-id="aaec8-102">API Permissions and Consent Process</span></span>

<span data-ttu-id="aaec8-103">لكي يمكن لتطبيقك الوصول إلى البيانات في Microsoft Graph، يجب على المستخدم أو المسؤول منحه الأذونات الصحيحة عبر عملية موافقة.</span><span class="sxs-lookup"><span data-stu-id="aaec8-103">For your app to access data in Microsoft Graph, the user or administrator must grant it the correct permissions via a consent process.</span></span> <span data-ttu-id="aaec8-104">[يسرد مرجع أذونات Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) الأذونات المقترنة بكل مجموعة رئيسية من واجهات برمجة تطبيقات Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="aaec8-104">[Microsoft Graph permissions reference](https://docs.microsoft.com/graph/permissions-reference) lists the permissions associated with each major set of Microsoft Graph APIs.</span></span> <span data-ttu-id="aaec8-105">كما يوفر إرشادات حول كيفية استخدام الأذونات.</span><span class="sxs-lookup"><span data-stu-id="aaec8-105">It also provides guidance about how to use the permissions.</span></span>

<span data-ttu-id="aaec8-106">**إعداد الخدمة الأساسية أو تحديثها**</span><span class="sxs-lookup"><span data-stu-id="aaec8-106">**Set up or update service principal**</span></span>

- <span data-ttu-id="aaec8-107">[إنشاء serviceprincipal](https://docs.microsoft.com/graph/api/serviceprincipal-post-serviceprincipals) - توضح لك هذه المقالة كيفية إنشاء كائن servicePrincipal جديد.</span><span class="sxs-lookup"><span data-stu-id="aaec8-107">[Create serviceprincipal](https://docs.microsoft.com/graph/api/serviceprincipal-post-serviceprincipals) - This article shows you how to create a new servicePrincipal object.</span></span>
- <span data-ttu-id="aaec8-108">إنشاء [تطبيق Azure AD &](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) أساسي للخدمة في المدخل - توضح لك هذه المقالة كيفية إنشاء تطبيق Azure Active Directory (Azure AD) جديد وأهم خدمة يمكن استخدامها مع عنصر تحكم الوصول المستند إلى الدور.</span><span class="sxs-lookup"><span data-stu-id="aaec8-108">[Create an Azure AD app & service principal in the portal](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) - This article shows you how to create a new Azure Active Directory (Azure AD) application and service principal that can be used with the role-based access control.</span></span>
- <span data-ttu-id="aaec8-109">تطبيقات & أساسيات الخدمات في [Azure AD](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) - تصف هذه المقالة تسجيل التطبيقات، وأشياء التطبيقات، وأعراض الخدمة الأساسية في Azure Active Directory: ماهيتها وكيفية استخدامها وكيفية اتسامها ببعضها البعض.</span><span class="sxs-lookup"><span data-stu-id="aaec8-109">[Apps & service principals in Azure AD](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) - This article describes application registration, application objects, and service principals in Azure Active Directory: what they are, how they are used, and how they are related to each other.</span></span>

<span data-ttu-id="aaec8-110">**إضافة تسجيل التطبيق أو تحديثه وتقديم موافقة المسؤول**</span><span class="sxs-lookup"><span data-stu-id="aaec8-110">**Add or update app registration and provide admin consent**</span></span>

- <span data-ttu-id="aaec8-111">[إنشاء تسجيل تطبيق](https://docs.microsoft.com/graph/api/application-post-applications) - توضح لك هذه المقالة كيفية إنشاء كائن تطبيق جديد.</span><span class="sxs-lookup"><span data-stu-id="aaec8-111">[Create an app registration](https://docs.microsoft.com/graph/api/application-post-applications) - This article shows you how to create a new application object.</span></span>
- <span data-ttu-id="aaec8-112">[تحديث تسجيل تطبيق - أذونات API](https://docs.microsoft.com/graph/api/application-update) - توضح لك هذه المقالة كيفية تحديث خصائص كائن تطبيق.</span><span class="sxs-lookup"><span data-stu-id="aaec8-112">[Update an app registration - API permissions](https://docs.microsoft.com/graph/api/application-update) - This article shows you how to update the properties of an application object.</span></span>
- <span data-ttu-id="aaec8-113">[تقديم موافقة المسؤول](https://docs.microsoft.com/graph/security-authorization#grant-permissions-to-an-application) - لموافقة المسؤول وموافقته بشكل عام، نطلب من المسؤول منح الموافقة بشكل صريح.</span><span class="sxs-lookup"><span data-stu-id="aaec8-113">[Provide admin consent](https://docs.microsoft.com/graph/security-authorization#grant-permissions-to-an-application) - For admin consent and consent in general, we require that an admin explicitly grants consent.</span></span>
- <span data-ttu-id="aaec8-114">[RBAC (beta)](https://docs.microsoft.com/graph/api/resources/rbacapplicationmultiple) - حاوية إدارة الدور لتعريفات الدور الموحدة وواجبات الدور لموفري MICROSOFT 365 RBAC الذين يدعمون العديد من الأساسيات والنطاقات المتعددة في تعيين دور واحد.</span><span class="sxs-lookup"><span data-stu-id="aaec8-114">[RBAC (beta)](https://docs.microsoft.com/graph/api/resources/rbacapplicationmultiple) - Role management container for unified role definitions and role assignments for Microsoft 365 RBAC providers that support multiple principals and multiple scopes in a single role assignment.</span></span> <span data-ttu-id="aaec8-115">يختلف ذلك عن نوع مورد *rbacApplication.*</span><span class="sxs-lookup"><span data-stu-id="aaec8-115">This is different from *rbacApplication* resource type.</span></span> <span data-ttu-id="aaec8-116">Microsoft Intune هو مثال لموفر RBAC هذا.</span><span class="sxs-lookup"><span data-stu-id="aaec8-116">Microsoft Intune is an example of such a RBAC provider.</span></span> <span data-ttu-id="aaec8-117">يمكن أن يكون تعيين الدور في Intune صفيفا من الأساسيات صفيفا من مجموعات النطاقات.</span><span class="sxs-lookup"><span data-stu-id="aaec8-117">A role assignment in Intune can have an array of principals and an array of scope groups.</span></span> <span data-ttu-id="aaec8-118">**هذا الإصدار في الإصدار بيتا، مما يعني أنه لا يزال قيد التطوير ولا يوصى باستخدامه في الإنتاج.**</span><span class="sxs-lookup"><span data-stu-id="aaec8-118">**This is in beta, meaning that it is still in development and not recommended for use in production.**</span></span>
