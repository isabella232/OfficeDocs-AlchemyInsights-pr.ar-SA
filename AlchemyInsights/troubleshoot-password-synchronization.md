---
title: استكشاف أخطاء مزامنة كلمة المرور وإصلاحها
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 54b5a033b7cbb99520425b31800364ed4a99a4e6
ms.sourcegitcommit: 1d01b8b48eef2d5d10c375dcf802cd36e9d6bf61
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 07/23/2020
ms.locfileid: "45387864"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="7a5a9-102">استكشاف أخطاء مزامنة كلمة المرور وإصلاحها</span><span class="sxs-lookup"><span data-stu-id="7a5a9-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="7a5a9-103">لاستكشاف مشكلات مزامنة كلمة المرور وإصلاحها، ابدأ باستخدام مهمة استكشاف أخطاء AAD Connect لاستكشاف الأخطاء وإصلاحها لتحديد سبب عدم مزامنة كلمات المرور.</span><span class="sxs-lookup"><span data-stu-id="7a5a9-103">To troubleshoot password synchronization issues, start by using this AAD Connect troubleshooting task to determine why passwords are not syncing.</span></span> <span data-ttu-id="7a5a9-104">للبدء، انتقل إلى [إدارة المزامنة المباشرة](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).</span><span class="sxs-lookup"><span data-stu-id="7a5a9-104">To begin, go to [Manage direct sync](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).</span></span>  

1. <span data-ttu-id="7a5a9-105">افتح جلسة عمل جديدة لـ Windows PowerShell على خادم Azure AD Connect، وحدد الخيار **تشغيل كمسؤول.**</span><span class="sxs-lookup"><span data-stu-id="7a5a9-105">Open a new Windows PowerShell session on your Azure AD Connect server, and select the **Run as Administrator** option.</span></span>

2. <span data-ttu-id="7a5a9-106">تشغيل مجموعة التنفيذ عن بعدIgnSigned أو تعيين تنفيذPolispoli.</span><span class="sxs-lookup"><span data-stu-id="7a5a9-106">Run Set-ExecutionPolicy RemoteSigned or Set-ExecutionPolicy Unrestricted.</span></span>

3. <span data-ttu-id="7a5a9-107">بدء تشغيل معالج الاتصال الإعلان Azure.</span><span class="sxs-lookup"><span data-stu-id="7a5a9-107">Start the Azure AD Connect wizard.</span></span>

4. <span data-ttu-id="7a5a9-108">انتقل إلى صفحة المهام الإضافية > **استكشاف الأخطاء**  >  **وإصلاحها بعد ذلك**.</span><span class="sxs-lookup"><span data-stu-id="7a5a9-108">Go to the Additional Tasks page > **Troubleshoot** > **Next**.</span></span>

5. <span data-ttu-id="7a5a9-109">حدد **Launch** لفتح القائمة PowerShell لاستكشاف الأخطاء وإصلاحها.</span><span class="sxs-lookup"><span data-stu-id="7a5a9-109">Select **Launch** to open the PowerShell troubleshooting menu.</span></span>

6. <span data-ttu-id="7a5a9-110">حدد **استكشاف أخطاء مزامنة كلمة المرور وإصلاحها**.</span><span class="sxs-lookup"><span data-stu-id="7a5a9-110">Select **Troubleshoot Password Synchronization**.</span></span>

    <span data-ttu-id="7a5a9-111">المشكلة عادةً لا تتم مزامنة كلمة مرور لحساب مستخدم معين.</span><span class="sxs-lookup"><span data-stu-id="7a5a9-111">The issue is usually that a password is not synchronized for a specific user account.</span></span>

    <span data-ttu-id="7a5a9-112">**ملاحظات** فشل مزامنة كلمة المرور إذا كانت آخر مزامنة ناجحة لكلمة المرور منذ بعض الوقت.</span><span class="sxs-lookup"><span data-stu-id="7a5a9-112">**Notes** Password synchronization fails if the last successful password sync was some time ago.</span></span>

<span data-ttu-id="7a5a9-113">لمزيد من المساعدة في استكشاف أخطاء مزامنة كلمة المرور وإصلاحها، راجع [استكشاف أخطاء مزامنة تجزئة كلمة المرور وإصلاحها مع مزامنة Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span><span class="sxs-lookup"><span data-stu-id="7a5a9-113">For more help troubleshooting password synchronization, see [Troubleshoot password hash synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>