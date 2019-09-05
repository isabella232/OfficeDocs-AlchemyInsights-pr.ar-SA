---
title: انتهاء صلاحية شهادة الاتحاد ADFS
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 6/8/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: eafd31e91340b41b7948fb1fe62889731b816d9a
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/04/2019
ms.locfileid: "36737176"
---
# <a name="adfs-federation-certificate-expiring"></a><span data-ttu-id="8a958-102">انتهاء صلاحية شهادة الاتحاد ADFS</span><span class="sxs-lookup"><span data-stu-id="8a958-102">ADFS Federation Certificate Expiring</span></span>

<span data-ttu-id="8a958-103">لحل هذه المشكلة، اتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="8a958-103">To resolve this issue, follow these steps:</span></span>
  
1. <span data-ttu-id="8a958-104">تثبيت الوحدة النمطية لـ Microsoft Azure Active Directory لـ Windows PowerShell على الكمبيوتر (إذا لم يتم تثبيت الوحدة النمطية بالفعل).</span><span class="sxs-lookup"><span data-stu-id="8a958-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="8a958-105">للقيام بذلك، انتقل إلى [إدارة إعلان Azure باستخدام Windows PowerShell](https://aka.ms/aadposh).</span><span class="sxs-lookup"><span data-stu-id="8a958-105">To do this, go to [Manage Azure AD using Windows PowerShell](https://aka.ms/aadposh).</span></span>

2. <span data-ttu-id="8a958-106">اتبع الخطوات الموجودة في "السيناريو 1: انتهت صلاحية شهادة توقيع الرمز المميز AD FS" من ["كان هناك مشكلة في الوصول إلى الموقع" خطأ من AD FS عند تسجيل دخول مستخدم متحد إلى Office 365 أو Azure إينتوني](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span><span class="sxs-lookup"><span data-stu-id="8a958-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Office 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>

3. <span data-ttu-id="8a958-107">اتبع الخطوات الموجودة في [تحديث أو إصلاح إعدادات مجال متحد في Office 365 أو Azure أو إينتوني](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).</span><span class="sxs-lookup"><span data-stu-id="8a958-107">Follow the steps in [Update or repair the settings of a federated domain in Office 365, Azure, or Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).</span></span>

    <span data-ttu-id="8a958-108">لمزيد من المعلومات حول تجديد شهادات الاتحاد، راجع [تجديد شهادات الاتحاد لOffice 365 و Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span><span class="sxs-lookup"><span data-stu-id="8a958-108">To learn more about renewing Federation certificates, see [Renew federation certificates for Office 365 and Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
