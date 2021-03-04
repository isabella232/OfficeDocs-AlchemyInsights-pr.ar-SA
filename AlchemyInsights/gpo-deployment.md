---
title: نشر GPO
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004400"
- "8602"
ms.openlocfilehash: d31f77e70e8456a4076a8146025f1f8ada977a06
ms.sourcegitcommit: 969219d6dff18d86d679d4d8741d1e39e4ce9539
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/03/2021
ms.locfileid: "50426947"
---
# <a name="gpo-deployment"></a><span data-ttu-id="5c428-102">نشر GPO</span><span class="sxs-lookup"><span data-stu-id="5c428-102">GPO Deployment</span></span>

<span data-ttu-id="5c428-103">غالبا ما تدار إعدادات كائنات المستخدم والكمبيوتر في Azure Active Directory Domain Services (Azure AD DS) باستخدام كائنات نهج المجموعة (GPOs).</span><span class="sxs-lookup"><span data-stu-id="5c428-103">Settings for user and computer objects in Azure Active Directory Domain Services (Azure AD DS) are often managed using Group Policy Objects (GPOs).</span></span> <span data-ttu-id="5c428-104">يتضمن Azure AD DS "GPOs" مضمنا لمستخدمي AADDC والحاويات "أجهزة كمبيوتر AADDC".</span><span class="sxs-lookup"><span data-stu-id="5c428-104">Azure AD DS includes built-in GPOs for the AADDC Users and AADDC Computers containers.</span></span> <span data-ttu-id="5c428-105">يمكنك تخصيص هذه الإعدادات المضمنة في GPOs لتكوين نهج المجموعة كما هو مطلوب بيئة.</span><span class="sxs-lookup"><span data-stu-id="5c428-105">You can customize these built-in GPOs to configure group policy as needed for your environment.</span></span> <span data-ttu-id="5c428-106">لدى أعضاء مجموعة مسؤولي Azure AD DC امتيازات إدارة نهج المجموعة في مجال Azure AD DS، ويمكنهم أيضا إنشاء وحدات GPOs ووحدات تنظيمية مخصصة.</span><span class="sxs-lookup"><span data-stu-id="5c428-106">Members of the Azure AD DC administrators group have group policy administration privileges in the Azure AD DS domain, and can also create custom GPOs and organizational units (OUs).</span></span> <span data-ttu-id="5c428-107">لمزيد من المعلومات حول نهج المجموعة وكيفية عمله، راجع [نظرة عامة حول نهج المجموعة.](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11))</span><span class="sxs-lookup"><span data-stu-id="5c428-107">For more information on what group policy is and how it works, see [Group Policy Overview](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11)).</span></span>

<span data-ttu-id="5c428-108">في البيئة المختلطة، لا يتم مزامنة سياسات المجموعات التي تم تكوينها في بيئة AD DS المحلية مع Azure AD DS.</span><span class="sxs-lookup"><span data-stu-id="5c428-108">In a hybrid environment, group policies configured in an on-premises AD DS environment aren't synchronized to Azure AD DS.</span></span> <span data-ttu-id="5c428-109">لتعريف إعدادات التكوين للمستخدمين أو أجهزة الكمبيوتر في Azure AD DS، قم بتحرير أحد "برامج GPOs" الافتراضية أو قم بإنشاء "نقطة GPO" مخصصة.</span><span class="sxs-lookup"><span data-stu-id="5c428-109">To define configuration settings for users or computers in Azure AD DS, edit one of the default GPOs or create a custom GPO.</span></span>

<span data-ttu-id="5c428-110">توضح لك هذه المقالة ["إدارة](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) نهج المجموعة" كيفية تثبيت أدوات "إدارة نهج المجموعة"، وكيفية تحرير "أدوات إدارة نهج المجموعة" المضمنة، وكيفية إنشاء "أدوات إدارة نهج المجموعة" المخصصة.</span><span class="sxs-lookup"><span data-stu-id="5c428-110">This article [Manage Group Policy](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) shows you how to install the Group Policy Management tools, how ton edit the built-in GPOs, and how to create custom GPOs.</span></span>
