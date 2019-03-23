---
title: الاتحاد ADFS انتهاء مدة صلاحية الشهادة
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 6/8/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: 518261787b1b0df99ee7b3dc3e51dec70e4373bc
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/22/2019
ms.locfileid: "30755141"
---
# <a name="adfs-federation-certificate-expiring"></a><span data-ttu-id="ca281-102">الاتحاد ADFS انتهاء مدة صلاحية الشهادة</span><span class="sxs-lookup"><span data-stu-id="ca281-102">ADFS Federation Certificate Expiring</span></span>

<span data-ttu-id="ca281-103">لحل هذه المشكلة، اتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="ca281-103">To resolve this issue, follow these steps:</span></span>
  
1. <span data-ttu-id="ca281-104">تثبيت في Microsoft Azure نشط الدليل الوحدة النمطية ل Windows PowerShell على الكمبيوتر (إذا لم يتم تثبيت الوحدة النمطية مسبقاً).</span><span class="sxs-lookup"><span data-stu-id="ca281-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="ca281-105">للقيام بذلك، انتقل إلى [إدارة استخدام Windows PowerShell الإعلان Azure](https://aka.ms/aadposh).</span><span class="sxs-lookup"><span data-stu-id="ca281-105">To do this, go to [Manage Azure AD using Windows PowerShell](https://aka.ms/aadposh).</span></span>
    
2. <span data-ttu-id="ca281-106">اتبع الخطوات الموجودة في "السيناريو 1: مدة صلاحية شهادة التوقيع الرمز المميز AD FS" المقطع ["كان هناك مشكلة في الوصول إلى الموقع" خطأ من خ الإعلان عند تسجيل مستخدم متحد Office 365، الأزرق السماوي، أو إينتوني](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span><span class="sxs-lookup"><span data-stu-id="ca281-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Office 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>
    
3. <span data-ttu-id="ca281-107">اتبع الخطوات في [كيفية تحديث أو إصلاح إعدادات المجال المتحد في Office 365، الأزرق السماوي، أو إينتوني](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span><span class="sxs-lookup"><span data-stu-id="ca281-107">Follow the steps in [How to update or repair the settings of a federated domain in Office 365, Azure, or Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span></span>
    
    <span data-ttu-id="ca281-108">لمزيد من المعلومات حول تجديد الشهادات الاتحاد، راجع [تجديد شهادات الاتحاد Office 365 و Active Directory Azure](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span><span class="sxs-lookup"><span data-stu-id="ca281-108">To learn more about renewing Federation certificates, see [Renew federation certificates for Office 365 and Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
    

