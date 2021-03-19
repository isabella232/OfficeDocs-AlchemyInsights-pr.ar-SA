---
title: انتهت صلاحية شهادة اتحاد ADFS
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
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: a3172bc402a22999a3bf963233cc26db1ddf2a03
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47686701"
---
# <a name="adfs-federation-certificate-expiring"></a><span data-ttu-id="904eb-102">انتهت صلاحية شهادة اتحاد ADFS</span><span class="sxs-lookup"><span data-stu-id="904eb-102">ADFS Federation Certificate Expiring</span></span>

<span data-ttu-id="904eb-103">لحل هذه المشكلة، اتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="904eb-103">To resolve this issue, follow these steps:</span></span>
  
1. <span data-ttu-id="904eb-104">ثبت وحدة Microsoft Azure Active Directory النمطية ل Windows PowerShell على الكمبيوتر (إذا لم تكن الوحدة النمطية مثبتة بالفعل).</span><span class="sxs-lookup"><span data-stu-id="904eb-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="904eb-105">للقيام بذلك، انتقل إلى [إدارة Azure AD باستخدام Windows PowerShell](https://aka.ms/aadposh).</span><span class="sxs-lookup"><span data-stu-id="904eb-105">To do this, go to [Manage Azure AD using Windows PowerShell](https://aka.ms/aadposh).</span></span>

2. <span data-ttu-id="904eb-106">اتبع الخطوات في القسم "السيناريو 1: انتهت صلاحية شهادة توقيع الرمز المميز ل AD FS" من الخطأ "كان هناك مشكلة في الوصول إلى الموقع" من AD FS عند تسجيل مستخدم مقسم إلى [Microsoft 365](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)أو Azure أو Intune .</span><span class="sxs-lookup"><span data-stu-id="904eb-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>

3. <span data-ttu-id="904eb-107">اتبع الخطوات في تحديث إعدادات مجال أو إصلاحها في Microsoft أو [Azure أو Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).</span><span class="sxs-lookup"><span data-stu-id="904eb-107">Follow the steps in [Update or repair the settings of a federated domain in Microsoft, Azure, or Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).</span></span>

    <span data-ttu-id="904eb-108">لمعرفة المزيد حول تجديد شهادات الاتحاد، راجع تجديد شهادات الاتحاد ل [Microsoft 365 و Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span><span class="sxs-lookup"><span data-stu-id="904eb-108">To learn more about renewing Federation certificates, see [Renew federation certificates for Microsoft 365 and Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
