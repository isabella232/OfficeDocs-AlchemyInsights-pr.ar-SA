---
title: شهادة اتحاد ADFS تنتهي صلاحيتها
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: 14e7da6220dfa96edca5d9ec5c32e003480a9eaf
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43710394"
---
# <a name="adfs-federation-certificate-expiring"></a><span data-ttu-id="d64c2-102">شهادة اتحاد ADFS تنتهي صلاحيتها</span><span class="sxs-lookup"><span data-stu-id="d64c2-102">ADFS Federation Certificate Expiring</span></span>

<span data-ttu-id="d64c2-103">لحل هذه المشكلة، اتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="d64c2-103">To resolve this issue, follow these steps:</span></span>
  
1. <span data-ttu-id="d64c2-104">قم بتثبيت وحدة الدليل النشط من Microsoft Azure لـ Windows PowerShell على الكمبيوتر (إذا لم يتم تثبيت الوحدة النمطية بالفعل).</span><span class="sxs-lookup"><span data-stu-id="d64c2-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="d64c2-105">للقيام بذلك، انتقل إلى [إدارة Azure AD باستخدام Windows PowerShell](https://aka.ms/aadposh).</span><span class="sxs-lookup"><span data-stu-id="d64c2-105">To do this, go to [Manage Azure AD using Windows PowerShell](https://aka.ms/aadposh).</span></span>

2. <span data-ttu-id="d64c2-106">اتبع الخطوات في المقطع "السيناريو 1: انتهت صلاحية شهادة توقيع الرمز المميز AD FS" من ["كانت هناك مشكلة في الوصول إلى الموقع" من AD FS عندما يسجل مستخدم موحد الدخول إلى Microsoft 365 أو Azure أو Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span><span class="sxs-lookup"><span data-stu-id="d64c2-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>

3. <span data-ttu-id="d64c2-107">اتبع الخطوات في [تحديث أو إصلاح إعدادات مجال موحد في Microsoft أو Azure أو Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).</span><span class="sxs-lookup"><span data-stu-id="d64c2-107">Follow the steps in [Update or repair the settings of a federated domain in Microsoft, Azure, or Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).</span></span>

    <span data-ttu-id="d64c2-108">لمعرفة المزيد حول تجديد شهادات الاتحاد، راجع [تجديد شهادات الاتحاد لـ Microsoft 365 وAzure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span><span class="sxs-lookup"><span data-stu-id="d64c2-108">To learn more about renewing Federation certificates, see [Renew federation certificates for Microsoft 365 and Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
