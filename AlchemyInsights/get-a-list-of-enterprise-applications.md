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
# <a name="get-a-list-of-enterprise-applications"></a>الحصول على قائمة "تطبيقات المؤسسة"

1. للحصول **على** قائمة تطبيقات المؤسسة (كل التطبيقات أو التي تمت تصفيتها حسب اسم العرض والمعرف ومعرف URIs وغير ذلك) من خلال الأمر Powershell، راجع [Get-AzureADApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadapplication).
2. للحصول على قائمة بالأشياء الأساسية للخدمة (كل العناصر أو تمت تصفيتها حسب الم ID) من خلال الأمر Powershell، راجع [Get-AzureADServicePrincipal (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadserviceprincipal).
3. إذا كنت تريد الحصول على قائمة تطبيقات SAML التي تم تكوينها، فقد يساعدك اتباع **برامج PowerShell النصية:**

    سيكون لكل تطبيق سواء كان تطبيق OAuth أو تطبيق SAML (كلا من التطبيقات المعرضية وغير المعرضية) اثنين من الكائنات التي تم إنشاؤها في AAD عند حدوث التسجيل. يسمى أحدهما كائن التطبيق والآخر هو كائن الخدمة الأساسي. عند تفريغ خصائص كائن الخدمة الأساسي باستخدام PowerShell، قد تجد أن كل تطبيق لديه عدد معين من العلامات المقترنة به مثل:

    - سيكون لتطبيقات OAuth علامة تسمى "**WindowsAzureActiveDirectoryIntegratedApp**"
    - معرض تطبيقات SAML سيكون لها علامة تسمى "**WindowsAzureActiveDirectoryGalleryApplicationPrimaryV1**"
    - قد يكون لتطبيقات SAML غير المعرض علامة تسمى "**WindowsAzureActiveDirectoryCustomSingleSignOnApplication**"

    وبالتالي، يمكنك استخدام هذه العلامات والعثور على نوع التطبيق. العلامة "**WindowsAzureActiveDirectoryIntegratedApp**" شائعة في جميع أنواع التطبيقات. يمكنك استخدام قصاصة متبعة لتضمين جميع تطبيقات SAML (المعرض وغير المعرض):

    `$type = "SAML APP"`

    `Get-AzureADServicePrincipal -All true | Where-Object {(.Tags -contains "WindowsAzureActiveDirectoryGalleryApplicationNonPrimaryV1") -or (_.Tags -contains "WindowsAzureActiveDirectoryCustomSingleSignOnApplication")} | Select DisplayName, @{Name="AppType"; Expression={type}}_.`

    لمزيد من المعلومات، راجع تحديد التطبيقات التي تم تمكين [SAML لها في Azure AD](https://docs.microsoft.com/answers/questions/24259/identify-saml-enabled-apps-in-azure-ad.html).

4. **البحث عن تطبيقات** ويب وإدراجها فقط : استخدم الأمر أدناه للحصول على جميع تطبيقات Azure AD التي تتضمن نوع التطبيق "Web app/API"

    Get-AzureADApplication -All:$true | Where-Object { $_. PublicClient -ne $true } | FT
5. **البحث عن التطبيقات الأصلية وإد** قائمتها فقط : تشغيل الأمر التالي للحصول على جميع تطبيقات العميل الأصلية (جهاز سطح المكتب/الجهاز المحمول).

    Get-AzureADApplication -All:$true | Where-Object { $_. PublicClient -eq $true } | FT
6. تصدير كافة تفاصيل تطبيق **Azure AD** المسجل إلى CSV : يصدر الأمر أدناه جميع تطبيقات Azure AD مع التفاصيل المطلوبة إلى ملف csv:

    - Get-AzureADApplication -All:$true | Select-Object DisplayName و AppID و PublicClient و AvailableToOtherTenants و HomePage و LogoutUrl |
    - Export-Csv "C:\AzureADApps.csv" -NoTypeInformation -ترميز UTF8

7. **الحاجة إلى تصدير قائمة تطبيقات Azure** غير التي تم استخدامها – تقرير التدقيق

    يمكن أن يظهر Azure AD سجلات التطبيقات لمدة تصل إلى 30 يوما فقط شريطة أن يكون لديك ترخيص Azure AD Premium.
    لديك خياران للاحتفاظ بالبيانات لمدة أطول من 30 يوما. يمكنك استخدام [واجهات برمجة التطبيقات لتقارير Azure AD](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-reporting-api) لاسترداد البيانات برمجيا وتخزينها في قاعدة بيانات. بدلا من ذلك، يمكنك دمج سجلات التدقيق في نظام SIEM جهة خارجية.

    يمكنك أيضا تنزيل قائمة التطبيقات لجميع التطبيقات والتطبيقات المملوكة ضمن Azure Active directory>تسجيلات التطبيقات>تنزيل>جميع التطبيقات/التطبيقات المملوكة.

    للحصول على قائمة التطبيقات من خلال MS Graph، راجع تطبيقات القائمة [- Microsoft Graph v1.0 ونوع](https://docs.microsoft.com/graph/api/application-list) مورد التطبيق - Microsoft [Graph v1.0](https://docs.microsoft.com/graph/api/resources/application).
