---
title: مشاكل سرية في عميل تسجيل التطبيق أو شهادة
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
- "9004352"
- "9685"
ms.openlocfilehash: 990648d286ec801785201e6513b70534c3d80e3f
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/23/2021
ms.locfileid: "51404152"
---
# <a name="app-registration-client-secret-or-certificate-issues"></a><span data-ttu-id="2d8b4-102">مشاكل سرية في عميل تسجيل التطبيق أو شهادة</span><span class="sxs-lookup"><span data-stu-id="2d8b4-102">App Registration client secret or Certificate issues</span></span>

<span data-ttu-id="2d8b4-103">هل تنتهي صلاحية سرية عميل التطبيق؟</span><span class="sxs-lookup"><span data-stu-id="2d8b4-103">Application client secret expiring?</span></span>

<span data-ttu-id="2d8b4-104">بغض النظر عن كيفية إنشاء التطبيق المسجل، سواء من خلال عملية التسجيل القياسية في مدخل تسجيل التطبيقات أو إذا تم إنشاء الخدمة الأساسية في المستأجر الخاص بك باستخدام موافقة التطبيق، يجب إنشاء سرية عميل جديدة قبل انتهاء صلاحية التطبيق الحالي وتحديثها في رمز التطبيق ذي الصلة.</span><span class="sxs-lookup"><span data-stu-id="2d8b4-104">Regardless of how the registered application was created, whether through the standard registration process in the Apps Registration portal or if the Service Principal was created in your tenant using application consent, a new Client Secret will need to be created prior to the expiration of the current one and updated in the related application code.</span></span> <span data-ttu-id="2d8b4-105">الحد الأقصى لفترة الصلاحية هو سنتان.</span><span class="sxs-lookup"><span data-stu-id="2d8b4-105">The maximum validity period is 2 years.</span></span> <span data-ttu-id="2d8b4-106">كتذكير، يجب تسجيل القيمة السرية حيث أنها لن تكون مرئية بعد مغادرة صفحة تسجيلات التطبيق في المدخل.</span><span class="sxs-lookup"><span data-stu-id="2d8b4-106">As a reminder the secret value must be recorded as it will no longer be visible after leaving the App registrations page in the portal.</span></span> <span data-ttu-id="2d8b4-107">لمزيد من المعلومات، راجع [التشغيل السريع:](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app) تسجيل تطبيق في النظام الأساسي لهوية Microsoft وأفضل الممارسات الخاصة ب النظام الأساسي [لهوية Microsoft](https://docs.microsoft.com/azure/active-directory/develop/identity-platform-integration-checklist#security).</span><span class="sxs-lookup"><span data-stu-id="2d8b4-107">For more information, see [Quickstart: Register an app in the Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app) and [Best practices for the Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/identity-platform-integration-checklist#security).</span></span>

<span data-ttu-id="2d8b4-108">لمعرفة المزيد، راجع [إنشاء تطبيق Azure AD](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal)& الأساسي للخدمة في المدخل - النظام الأساسي هوية Microsoft .</span><span class="sxs-lookup"><span data-stu-id="2d8b4-108">To learn more, see [Create an Azure AD app & service principal in the portal - Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal).</span></span>
