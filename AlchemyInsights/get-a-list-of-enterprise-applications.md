---
title: الحصول على قائمة "تطبيقات المؤسسة"
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
- "9004342"
- "9837"
ms.openlocfilehash: f5c1a77e415d4bbaa5718a6668af95934db7e5ae
ms.sourcegitcommit: e5f261f95ffc6074cce89e62ef8c4e9fd519d3ee
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/26/2021
ms.locfileid: "51404170"
---
# <a name="get-a-list-of-enterprise-applications"></a><span data-ttu-id="6c04b-102">الحصول على قائمة "تطبيقات المؤسسة"</span><span class="sxs-lookup"><span data-stu-id="6c04b-102">Get a list of Enterprise Applications</span></span>

1. <span data-ttu-id="6c04b-103">للحصول **على** قائمة تطبيقات المؤسسة (كل التطبيقات أو التي تمت تصفيتها حسب اسم العرض والمعرف ومعرف URIs وغير ذلك) من خلال الأمر Powershell، راجع [Get-AzureADApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadapplication).</span><span class="sxs-lookup"><span data-stu-id="6c04b-103">To **get a list of enterprise applications** (all applications or filtered by Display name, ID, Identifier URIs, etc.) through Powershell command, see [Get-AzureADApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadapplication).</span></span>
2. <span data-ttu-id="6c04b-104">للحصول على قائمة بالأشياء الأساسية للخدمة (كل العناصر أو تمت تصفيتها حسب الم ID) من خلال الأمر Powershell، راجع [Get-AzureADServicePrincipal (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadserviceprincipal).</span><span class="sxs-lookup"><span data-stu-id="6c04b-104">To get a list of service principal objects (all objects or filtered by ID) through Powershell command, see [Get-AzureADServicePrincipal (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadserviceprincipal).</span></span>
3. <span data-ttu-id="6c04b-105">إذا كنت تريد الحصول على قائمة تطبيقات SAML التي تم تكوينها، فقد يساعدك اتباع **برامج PowerShell النصية:**</span><span class="sxs-lookup"><span data-stu-id="6c04b-105">If you want to **get a list of SAML configured apps, following PowerShell scripts** may help you:</span></span>

    <span data-ttu-id="6c04b-106">سيكون لكل تطبيق سواء كان تطبيق OAuth أو تطبيق SAML (كلا من التطبيقات المعرضية وغير المعرضية) اثنين من الكائنات التي تم إنشاؤها في AAD عند حدوث التسجيل.</span><span class="sxs-lookup"><span data-stu-id="6c04b-106">Every Application be it an OAuth app or SAML app (both gallery and non-gallery apps) would have two objects created in AAD when their registration happens.</span></span> <span data-ttu-id="6c04b-107">يسمى أحدهما كائن التطبيق والآخر هو كائن الخدمة الأساسي.</span><span class="sxs-lookup"><span data-stu-id="6c04b-107">One is called the Application Object and the other is the Service Principal object.</span></span> <span data-ttu-id="6c04b-108">عند تفريغ خصائص كائن الخدمة الأساسي باستخدام PowerShell، قد تجد أن كل تطبيق لديه عدد معين من العلامات المقترنة به مثل:</span><span class="sxs-lookup"><span data-stu-id="6c04b-108">When you dump the properties of a Service Principal Object using PowerShell, you would find that every application has a certain number of Tags associated with it like:</span></span>

    - <span data-ttu-id="6c04b-109">سيكون لتطبيقات OAuth علامة تسمى "**WindowsAzureActiveDirectoryIntegratedApp**"</span><span class="sxs-lookup"><span data-stu-id="6c04b-109">OAuth apps would have a tag called "**WindowsAzureActiveDirectoryIntegratedApp**"</span></span>
    - <span data-ttu-id="6c04b-110">معرض تطبيقات SAML سيكون لها علامة تسمى "**WindowsAzureActiveDirectoryGalleryApplicationPrimaryV1**"</span><span class="sxs-lookup"><span data-stu-id="6c04b-110">Gallery SAML Apps would have a tag called "**WindowsAzureActiveDirectoryGalleryApplicationPrimaryV1**"</span></span>
    - <span data-ttu-id="6c04b-111">قد يكون لتطبيقات SAML غير المعرض علامة تسمى "**WindowsAzureActiveDirectoryCustomSingleSignOnApplication**"</span><span class="sxs-lookup"><span data-stu-id="6c04b-111">Non-Gallery SAML Apps would have a tag called "**WindowsAzureActiveDirectoryCustomSingleSignOnApplication**"</span></span>

    <span data-ttu-id="6c04b-112">وبالتالي، يمكنك استخدام هذه العلامات والعثور على نوع التطبيق.</span><span class="sxs-lookup"><span data-stu-id="6c04b-112">Hence, you can use these tags and find out what kind of app it is.</span></span> <span data-ttu-id="6c04b-113">العلامة "**WindowsAzureActiveDirectoryIntegratedApp**" شائعة في جميع أنواع التطبيقات.</span><span class="sxs-lookup"><span data-stu-id="6c04b-113">The tag "**WindowsAzureActiveDirectoryIntegratedApp**" is common to all types of apps.</span></span> <span data-ttu-id="6c04b-114">يمكنك استخدام قصاصة متبعة لتضمين جميع تطبيقات SAML (المعرض وغير المعرض):</span><span class="sxs-lookup"><span data-stu-id="6c04b-114">You can use following snippet to list all the SAML apps (both gallery and non-gallery):</span></span>

    `$type = "SAML APP"`

    `Get-AzureADServicePrincipal -All true | Where-Object {(.Tags -contains "WindowsAzureActiveDirectoryGalleryApplicationNonPrimaryV1") -or (_.Tags -contains "WindowsAzureActiveDirectoryCustomSingleSignOnApplication")} | Select DisplayName, @{Name="AppType"; Expression={type}}_.`

    <span data-ttu-id="6c04b-115">لمزيد من المعلومات، راجع تحديد التطبيقات التي تم تمكين [SAML لها في Azure AD](https://docs.microsoft.com/answers/questions/24259/identify-saml-enabled-apps-in-azure-ad.html).</span><span class="sxs-lookup"><span data-stu-id="6c04b-115">For more information, see [Identify SAML-enabled apps in Azure AD](https://docs.microsoft.com/answers/questions/24259/identify-saml-enabled-apps-in-azure-ad.html).</span></span>

4. <span data-ttu-id="6c04b-116">**البحث عن تطبيقات** ويب وإدراجها فقط : استخدم الأمر أدناه للحصول على جميع تطبيقات Azure AD التي تتضمن نوع التطبيق "Web app/API"</span><span class="sxs-lookup"><span data-stu-id="6c04b-116">**Find and list only Web applications**: Use the below command to get all Azure AD applications with the application type "Web app/API"</span></span>

    <span data-ttu-id="6c04b-117">Get-AzureADApplication -All:$true | Where-Object { $_. PublicClient -ne $true } | FT</span><span class="sxs-lookup"><span data-stu-id="6c04b-117">Get-AzureADApplication -All:$true | Where-Object { $_.PublicClient -ne $true } | FT</span></span>
5. <span data-ttu-id="6c04b-118">**البحث عن التطبيقات الأصلية وإد** قائمتها فقط : تشغيل الأمر التالي للحصول على جميع تطبيقات العميل الأصلية (جهاز سطح المكتب/الجهاز المحمول).</span><span class="sxs-lookup"><span data-stu-id="6c04b-118">**Find and list Native applications alone**: Run the following command to get all the native client (desktop/mobile device) applications.</span></span>

    <span data-ttu-id="6c04b-119">Get-AzureADApplication -All:$true | Where-Object { $_. PublicClient -eq $true } | FT</span><span class="sxs-lookup"><span data-stu-id="6c04b-119">Get-AzureADApplication -All:$true | Where-Object { $_.PublicClient -eq $true } | FT</span></span>
6. <span data-ttu-id="6c04b-120">تصدير كافة تفاصيل تطبيق **Azure AD** المسجل إلى CSV : يصدر الأمر أدناه جميع تطبيقات Azure AD مع التفاصيل المطلوبة إلى ملف csv:</span><span class="sxs-lookup"><span data-stu-id="6c04b-120">**Export All Registered Azure AD Application Details to CSV**: The below command exports all the Azure AD apps with required details to csv file:</span></span>

    - <span data-ttu-id="6c04b-121">Get-AzureADApplication -All:$true | Select-Object DisplayName و AppID و PublicClient و AvailableToOtherTenants و HomePage و LogoutUrl |</span><span class="sxs-lookup"><span data-stu-id="6c04b-121">Get-AzureADApplication -All:$true | Select-Object DisplayName, AppID, PublicClient, AvailableToOtherTenants, HomePage, LogoutUrl |</span></span>
    - <span data-ttu-id="6c04b-122">Export-Csv "C:\AzureADApps.csv" -NoTypeInformation -ترميز UTF8</span><span class="sxs-lookup"><span data-stu-id="6c04b-122">Export-Csv "C:\AzureADApps.csv" -NoTypeInformation -Encoding UTF8</span></span>

7. <span data-ttu-id="6c04b-123">**الحاجة إلى تصدير قائمة تطبيقات Azure** غير التي تم استخدامها – تقرير التدقيق</span><span class="sxs-lookup"><span data-stu-id="6c04b-123">**Need to export a list of unused Azure apps** – Audit report</span></span>

    <span data-ttu-id="6c04b-124">يمكن أن يظهر Azure AD سجلات التطبيقات لمدة تصل إلى 30 يوما فقط شريطة أن يكون لديك ترخيص Azure AD Premium.</span><span class="sxs-lookup"><span data-stu-id="6c04b-124">Azure AD can show application logs for only up to 30 days provided you have Azure AD Premium license.</span></span>
    <span data-ttu-id="6c04b-125">لديك خياران للاحتفاظ بالبيانات لمدة أطول من 30 يوما.</span><span class="sxs-lookup"><span data-stu-id="6c04b-125">You have two options to retain the data for longer than 30 days.</span></span> <span data-ttu-id="6c04b-126">يمكنك استخدام [واجهات برمجة التطبيقات لتقارير Azure AD](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-reporting-api) لاسترداد البيانات برمجيا وتخزينها في قاعدة بيانات.</span><span class="sxs-lookup"><span data-stu-id="6c04b-126">You can use the [Azure AD Reporting APIs](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-reporting-api) to retrieve the data programmatically and store it in a database.</span></span> <span data-ttu-id="6c04b-127">بدلا من ذلك، يمكنك دمج سجلات التدقيق في نظام SIEM جهة خارجية.</span><span class="sxs-lookup"><span data-stu-id="6c04b-127">Alternatively, you can integrate audit logs into a third party SIEM system.</span></span>

    <span data-ttu-id="6c04b-128">يمكنك أيضا تنزيل قائمة التطبيقات لجميع التطبيقات والتطبيقات المملوكة ضمن Azure Active directory>تسجيلات التطبيقات>تنزيل>جميع التطبيقات/التطبيقات المملوكة.</span><span class="sxs-lookup"><span data-stu-id="6c04b-128">You can also download the app list for all applications and owned applications under Azure Active directory>App Registrations>Download>All applications/Owned applications.</span></span>

    <span data-ttu-id="6c04b-129">للحصول على قائمة التطبيقات من خلال MS Graph، راجع تطبيقات القائمة [- Microsoft Graph v1.0 ونوع](https://docs.microsoft.com/graph/api/application-list) مورد التطبيق - Microsoft [Graph v1.0](https://docs.microsoft.com/graph/api/resources/application).</span><span class="sxs-lookup"><span data-stu-id="6c04b-129">To get a list of applications through MS Graph, see [List applications - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-list) and [application resource type - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/resources/application).</span></span>
