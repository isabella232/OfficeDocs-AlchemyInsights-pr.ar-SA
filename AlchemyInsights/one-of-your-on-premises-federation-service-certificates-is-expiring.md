---
title: انتهت صلاحيه أحدي شهادات الخدمة الموحدة المحلية لديك
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: a4c78f3fdbba7786785f31098c9e80e77a165623
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47673484"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a><span data-ttu-id="c567c-102">انتهت صلاحيه أحدي شهادات الخدمة الموحدة المحلية لديك</span><span class="sxs-lookup"><span data-stu-id="c567c-102">One of your on-premises Federation Service Certificates is expiring</span></span>

<span data-ttu-id="c567c-103">لحل هذه المشكلة ، اتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="c567c-103">To resolve this issue, follow these steps:</span></span>
  
- <span data-ttu-id="c567c-104">قم بتثبيت الوحدة النمطية ل Microsoft Azure Active directory ل Windows PowerShell علي الكمبيوتر (إذا لم تكن الوحدة النمطية مثبته بالفعل).</span><span class="sxs-lookup"><span data-stu-id="c567c-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="c567c-105">للقيام بذلك ، انتقل إلى [Azure Active Directory PowerShell ل Graph ](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span><span class="sxs-lookup"><span data-stu-id="c567c-105">To do this, go to [Azure Active Directory PowerShell for Graph ](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span></span>
    
- <span data-ttu-id="c567c-106">اتبع الخطوات الواردة في القسم "السيناريو 1: انتهت صلاحيه الرمز المميز للإعلان عن شهادة" في [الحالة "هناك مشكله في الوصول إلى الموقع" من AD FS عندما يقوم مستخدم خارجي بتسجيل الدخول إلى Microsoft 365 أو Azure أو Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span><span class="sxs-lookup"><span data-stu-id="c567c-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>
    
- <span data-ttu-id="c567c-107">اتبع الخطوات الواردة في [كيفيه تحديث إعدادات مجال متحد أو إصلاحها في Microsoft 365 أو Azure أو Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span><span class="sxs-lookup"><span data-stu-id="c567c-107">Follow the steps in [How to update or repair the settings of a federated domain in Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span></span>
    
<span data-ttu-id="c567c-108">للحصول علي مزيد من المعلومات حول تجديد شهادات الاتحاد ، راجع [تجديد الشهادة ل O365 و AZURE AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span><span class="sxs-lookup"><span data-stu-id="c567c-108">For more information about renewing Federation certificates, see [Certificate renewal for O365 and Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
  

