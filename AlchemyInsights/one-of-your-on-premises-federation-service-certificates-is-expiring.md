---
title: تنتهي صلاحية إحدى شهادات خدمة الاتحاد المحلي
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: 24c369c61ad7cf7a9fe101ac29271c32e5159c1f
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43761370"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a><span data-ttu-id="cd6e3-102">تنتهي صلاحية إحدى شهادات خدمة الاتحاد المحلي</span><span class="sxs-lookup"><span data-stu-id="cd6e3-102">One of your on-premises Federation Service Certificates is expiring</span></span>

<span data-ttu-id="cd6e3-103">لحل هذه المشكلة، اتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="cd6e3-103">To resolve this issue, follow these steps:</span></span>
  
- <span data-ttu-id="cd6e3-104">قم بتثبيت وحدة الدليل النشط من Microsoft Azure لـ Windows PowerShell على الكمبيوتر (إذا لم يتم تثبيت الوحدة النمطية بالفعل).</span><span class="sxs-lookup"><span data-stu-id="cd6e3-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="cd6e3-105">للقيام بذلك، انتقل إلى [Azure Active Directory PowerShell للرسم البياني](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span><span class="sxs-lookup"><span data-stu-id="cd6e3-105">To do this, go to [Azure Active Directory PowerShell for Graph ](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span></span>
    
- <span data-ttu-id="cd6e3-106">اتبع الخطوات في المقطع "السيناريو 1: انتهت صلاحية شهادة توقيع الرمز المميز AD FS" من [خطأ "كانت هناك مشكلة في الوصول إلى الموقع" من AD FS عندما يسجل مستخدم موحد الدخول إلى Office 365 أو Azure أو Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span><span class="sxs-lookup"><span data-stu-id="cd6e3-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Office 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>
    
- <span data-ttu-id="cd6e3-107">اتبع الخطوات في ر[كيفية تحديث أو إصلاح إعدادات مجال موحد في Office 365 أو Azure أو Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span><span class="sxs-lookup"><span data-stu-id="cd6e3-107">Follow the steps in t[How to update or repair the settings of a federated domain in Office 365, Azure, or Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span></span>
    
<span data-ttu-id="cd6e3-108">لمزيد من المعلومات حول تجديد شهادات الاتحاد، راجع [تجديد الشهادة لـ O365 و Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span><span class="sxs-lookup"><span data-stu-id="cd6e3-108">For more information about renewing Federation certificates, see [Certificate renewal for O365 and Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
  

