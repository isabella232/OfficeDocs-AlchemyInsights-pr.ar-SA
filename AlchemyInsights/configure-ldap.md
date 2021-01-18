---
title: تكوين LDAP
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004394"
- "7923"
ms.openlocfilehash: b6e89bca4e924c5570123194cb26358ba2c162ce
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/15/2021
ms.locfileid: "49884775"
---
# <a name="configure-ldap"></a><span data-ttu-id="dfc76-102">تكوين LDAP</span><span class="sxs-lookup"><span data-stu-id="dfc76-102">Configure LDAP</span></span>

<span data-ttu-id="dfc76-103">لتكوين LDAP ، نفذ الإجراءات التالية:</span><span class="sxs-lookup"><span data-stu-id="dfc76-103">To configure LDAP, do the following:</span></span>

1. <span data-ttu-id="dfc76-104">تحقق من صحة المجال علي [مدخل Azure](https://aka.ms/aadds-health).</span><span class="sxs-lookup"><span data-stu-id="dfc76-104">Check your domain’s health on the [Azure portal](https://aka.ms/aadds-health).</span></span>
1. <span data-ttu-id="dfc76-105">تاكد من توفر اشتراك Azure AD صالح ومن تمكين خدمات مجال Azure AD.</span><span class="sxs-lookup"><span data-stu-id="dfc76-105">Ensure a valid Azure AD subscription is available and Azure AD Domain Services has been enabled.</span></span>
1. <span data-ttu-id="dfc76-106">يجب الحصول علي الشهادة المطلوبة لتمكين LDAP الامنه من مرجع مصدق عام موثوق به أو تكون شهادة موقعه ذاتيا.</span><span class="sxs-lookup"><span data-stu-id="dfc76-106">The certificate required to enable secure LDAP must be obtained from a trusted public certification authority or be a self-signed certificate.</span></span>
1. <span data-ttu-id="dfc76-107">تاكد من ان الشهادة تتبع [الإرشادات](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate)المطلوبة.</span><span class="sxs-lookup"><span data-stu-id="dfc76-107">Ensure the certificate follows the required [guidelines](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate).</span></span>

<span data-ttu-id="dfc76-108">**شهادة غير صالحه**</span><span class="sxs-lookup"><span data-stu-id="dfc76-108">**Invalid Certificate**</span></span>
1. <span data-ttu-id="dfc76-109">لتجديد شهادة ، اتبع الخطوات التالية لإنشاء شهادة جديده وريوبلواد: [تكوين LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="dfc76-109">To renew a certificate, follow the steps to create a new certificate and reupload: [Configure LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
1. <span data-ttu-id="dfc76-110">لحل المشكلة المعروفة باستخدام تنبيات LDAP الامنه في خدمات مجالات Azure Active directory ، راجع [حل تنبيات ldap](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="dfc76-110">To resolve known issue with Secure LDAP alerts in Azure Active directory Domain Services, see [Resolve LDAP alerts](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
