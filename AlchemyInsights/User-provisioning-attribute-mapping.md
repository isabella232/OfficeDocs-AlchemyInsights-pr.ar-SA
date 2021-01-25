---
title: تعيين سمه توفير المستخدم
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/22/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7851"
- "9004348"
ms.openlocfilehash: 8bbf554c533d960a304901d7cbb492b87e9bec71
ms.sourcegitcommit: 953a8567ebcd9835f8c5c49472b223107c92549b
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/22/2021
ms.locfileid: "49949635"
---
# <a name="user-provisioning-attribute-mapping"></a><span data-ttu-id="af4e1-102">تعيين سمه توفير المستخدم</span><span class="sxs-lookup"><span data-stu-id="af4e1-102">User-provisioning attribute mapping</span></span>

1. <span data-ttu-id="af4e1-103">لاستكشاف مشاكل التعيين للسمة المعروفة وإصلاحها ، راجع [تعيينات السمات](https://docs.microsoft.com/azure/active-directory/app-provisioning/known-issues#attribute-mappings).</span><span class="sxs-lookup"><span data-stu-id="af4e1-103">To troubleshoot known attribute-mapping issues, see [Attribute mappings](https://docs.microsoft.com/azure/active-directory/app-provisioning/known-issues#attribute-mappings).</span></span> 
2. <span data-ttu-id="af4e1-104">توفر Microsoft Azure Active directory (AD) دعما لتوفير المستخدمين لتطبيقات ميناء التابعة لجات خارجيه مثل Salesforce و G المجموعة وغيرها.</span><span class="sxs-lookup"><span data-stu-id="af4e1-104">Microsoft Azure Active Directory (AD) provides support for user provisioning to third-party SaaS applications such as Salesforce, G Suite and others.</span></span> <span data-ttu-id="af4e1-105">إذا قمت بتمكين توفير المستخدم لتطبيق ميناء تابع لجهة خارجيه ، سيتحكم مدخل Azure في قيم سماته من خلال تعيينات السمات.</span><span class="sxs-lookup"><span data-stu-id="af4e1-105">If you enable user provisioning for a third-party SaaS application, the Azure portal controls its attribute values through attribute-mappings.</span></span> <span data-ttu-id="af4e1-106">للتعرف علي كيفيه تخصيص السمات الافتراضية ، راجع [تخصيص سمه توفير المستخدم-تعيينات لتطبيقات ميناء في Azure Active](https://docs.microsoft.com/azure/active-directory/app-provisioning/customize-application-attributes)directory.</span><span class="sxs-lookup"><span data-stu-id="af4e1-106">To learn how to customize the default attribute-mappings, see [Customize user provisioning attribute-mappings for SaaS applications in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/app-provisioning/customize-application-attributes).</span></span>
    - <span data-ttu-id="af4e1-107">للحصول علي مزيد من المعلومات حول توفير المستخدم لتطبيق ميناء ، راجع [ما هو التطبيق التلقائي لميناء الذي يوفره المستخدم في AZURE AD ؟](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning)</span><span class="sxs-lookup"><span data-stu-id="af4e1-107">To learn more about SaaS app user provisioning, see [What is automated SaaS app user provisioning in Azure AD?](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning)</span></span> 
3. <span data-ttu-id="af4e1-108">عند تخصيص السمات لتوفير المستخدم ، قد تجد ان السمة التي تريد تعيينها لا تظهر في قائمه السمات المصدر.</span><span class="sxs-lookup"><span data-stu-id="af4e1-108">When customizing attribute-mappings for user provisioning, you might find that the attribute you want to map doesn't appear in the Source attribute list.</span></span> <span data-ttu-id="af4e1-109">تعرض لك [مزامنة سمه من Active directory المحلي إلى AZURE AD لتوفيرها إلى مقاله تطبيق](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning-sync-attributes-for-mapping) كيفيه أضافه السمة المفقودة عن طريق مزامنتها من الإعلان المحلي إلى Azure AD.</span><span class="sxs-lookup"><span data-stu-id="af4e1-109">The [Sync an attribute from your on-premises Active Directory to Azure AD for provisioning to an application](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning-sync-attributes-for-mapping) article shows you how to add the missing attribute by synchronizing it from your on-premises AD to Azure AD.</span></span>
