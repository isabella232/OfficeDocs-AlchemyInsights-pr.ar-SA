---
title: تنتهي إحدى "شهادات خدمة الاتحاد" المحلي الخاص بك
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: e1afad0bab317af0f60a6ebda8c3ec8be398e38d
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/22/2019
ms.locfileid: "30753017"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a><span data-ttu-id="0fe8f-102">تنتهي إحدى "شهادات خدمة الاتحاد" المحلي الخاص بك</span><span class="sxs-lookup"><span data-stu-id="0fe8f-102">One of your on-premises Federation Service Certificates is expiring</span></span>

<span data-ttu-id="0fe8f-103">لحل هذه المشكلة، اتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="0fe8f-103">To resolve this issue, follow these steps:</span></span>
  
- <span data-ttu-id="0fe8f-104">تثبيت في Microsoft Azure نشط الدليل الوحدة النمطية ل Windows PowerShell على الكمبيوتر (إذا لم يتم تثبيت الوحدة النمطية مسبقاً).</span><span class="sxs-lookup"><span data-stu-id="0fe8f-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="0fe8f-105">للقيام بذلك، انتقل إلى [Azure PowerShell الدليل النشط للرسم البياني](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span><span class="sxs-lookup"><span data-stu-id="0fe8f-105">To do this, go to [Azure Active Directory PowerShell for Graph ](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span></span>
    
- <span data-ttu-id="0fe8f-106">اتبع الخطوات الموجودة في "السيناريو 1: مدة صلاحية شهادة التوقيع الرمز المميز AD FS" المقطع ["كان هناك مشكلة في الوصول إلى الموقع" خطأ من خ الإعلان عند تسجيل مستخدم متحد Office 365، الأزرق السماوي، أو إينتوني](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span><span class="sxs-lookup"><span data-stu-id="0fe8f-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Office 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>
    
- <span data-ttu-id="0fe8f-107">اتبع الخطوات الموجودة في تي[كيفية تحديث أو إصلاح إعدادات المجال المتحد في Office 365، الأزرق السماوي، أو إينتوني](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span><span class="sxs-lookup"><span data-stu-id="0fe8f-107">Follow the steps in t[How to update or repair the settings of a federated domain in Office 365, Azure, or Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span></span>
    
<span data-ttu-id="0fe8f-108">لمزيد من المعلومات حول تجديد الشهادات الاتحاد، راجع [تجديد الشهادة ل O365 وإعلان Azure](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span><span class="sxs-lookup"><span data-stu-id="0fe8f-108">For more information about renewing Federation certificates, see [Certificate renewal for O365 and Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
  

