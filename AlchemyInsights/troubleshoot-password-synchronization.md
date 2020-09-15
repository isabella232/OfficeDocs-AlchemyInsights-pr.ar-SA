---
title: استكشاف أخطاء مزامنة كلمه المرور وإصلاحها
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 96f63f2ae8e5de246bce7fc15a9b2c3d604f2eb8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664913"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="ecc5b-102">استكشاف أخطاء مزامنة كلمه المرور وإصلاحها</span><span class="sxs-lookup"><span data-stu-id="ecc5b-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="ecc5b-103">لاستكشاف أخطاء مزامنة كلمات المرور وإصلاحها ، أبدا باستخدام المهمة التالية لاستكشاف الأخطاء وإصلاحها في AAD</span><span class="sxs-lookup"><span data-stu-id="ecc5b-103">To troubleshoot password synchronization issues, start by using this AAD Connect troubleshooting task to determine why passwords are not syncing.</span></span> <span data-ttu-id="ecc5b-104">للبدء ، انتقل إلى [أداره المزامنة المباشرة](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).</span><span class="sxs-lookup"><span data-stu-id="ecc5b-104">To begin, go to [Manage direct sync](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).</span></span>  

1. <span data-ttu-id="ecc5b-105">افتح جلسة Windows PowerShell جديده علي خادم Azure AD Connect ، وحدد الخيار **تشغيل كمسؤول** .</span><span class="sxs-lookup"><span data-stu-id="ecc5b-105">Open a new Windows PowerShell session on your Azure AD Connect server, and select the **Run as Administrator** option.</span></span>

2. <span data-ttu-id="ecc5b-106">شغل Set اكسيكوتيونبوليسي ريموتيسيجنيد أو Set-اكسيكوتيونبوليسي غير مقيد.</span><span class="sxs-lookup"><span data-stu-id="ecc5b-106">Run Set-ExecutionPolicy RemoteSigned or Set-ExecutionPolicy Unrestricted.</span></span>

3. <span data-ttu-id="ecc5b-107">أبدا تشغيل معالج Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="ecc5b-107">Start the Azure AD Connect wizard.</span></span>

4. <span data-ttu-id="ecc5b-108">انتقل إلى صفحه المهام الاضافيه > **استكشاف الأخطاء وإصلاحها**  >  **Next**.</span><span class="sxs-lookup"><span data-stu-id="ecc5b-108">Go to the Additional Tasks page > **Troubleshoot** > **Next**.</span></span>

5. <span data-ttu-id="ecc5b-109">حدد **تشغيل** لفتح قائمه استكشاف الأخطاء وإصلاحها في PowerShell.</span><span class="sxs-lookup"><span data-stu-id="ecc5b-109">Select **Launch** to open the PowerShell troubleshooting menu.</span></span>

6. <span data-ttu-id="ecc5b-110">حدد **استكشاف أخطاء مزامنة كلمه المرور وإصلاحها**.</span><span class="sxs-lookup"><span data-stu-id="ecc5b-110">Select **Troubleshoot Password Synchronization**.</span></span>

    <span data-ttu-id="ecc5b-111">تحدث هذه المشكلة عاده بعدم مزامنة كلمه المرور لحساب مستخدم معين.</span><span class="sxs-lookup"><span data-stu-id="ecc5b-111">The issue is usually that a password is not synchronized for a specific user account.</span></span>

    <span data-ttu-id="ecc5b-112">**ملاحظات** تفشل مزامنة كلمه المرور إذا كانت آخر مزامنة ناجحه لكلمه المرور قد تم منذ بعض الوقت.</span><span class="sxs-lookup"><span data-stu-id="ecc5b-112">**Notes** Password synchronization fails if the last successful password sync was some time ago.</span></span>

<span data-ttu-id="ecc5b-113">للحصول علي المزيد من المساعدة في استكشاف أخطاء مزامنة كلمه المرور [وإصلاحها ، راجع استكشاف أخطاء مزامنة تجزئه كلمه المرور باستخدام مزامنة AZURE AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span><span class="sxs-lookup"><span data-stu-id="ecc5b-113">For more help troubleshooting password synchronization, see [Troubleshoot password hash synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>