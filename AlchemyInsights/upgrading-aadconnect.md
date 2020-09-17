---
title: 932 ترقيه AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 5c8ec5d9282c53c655e28f5d38fe36fc3ab005b8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806026"
---
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="5f189-102">ترقيه Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="5f189-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="5f189-103">بشكل افتراضي ، يتم تمكين الترقية التلقائية ل Azure AD Connect ، مما يساعد علي التاكد من تشغيل الإصدار الأخير.</span><span class="sxs-lookup"><span data-stu-id="5f189-103">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version.</span></span> <span data-ttu-id="5f189-104">للتحقق من إعدادات الترقية التلقائية ، استخدم الأمر **أدسينكاوتوبجرادي** Cmdlet في Azure AD PowerShell.</span><span class="sxs-lookup"><span data-stu-id="5f189-104">To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell.</span></span> <span data-ttu-id="5f189-105">سيقوم أمر cmdlet بإرجاع أحدي القيم التالية:</span><span class="sxs-lookup"><span data-stu-id="5f189-105">The cmdlet will return one of following values:</span></span>

- <span data-ttu-id="5f189-106">**ممكن**: تم تمكين الترقية التلقائية.</span><span class="sxs-lookup"><span data-stu-id="5f189-106">**Enabled**: Automatic upgrade is enabled.</span></span>

- <span data-ttu-id="5f189-107">**معطل**: تم تعطيل الترقية التلقائية.</span><span class="sxs-lookup"><span data-stu-id="5f189-107">**Disabled**: Automatic upgrade is disabled.</span></span>

- <span data-ttu-id="5f189-108">**معلق**: لم يعد النظام مؤهلا لتلقي الترقيات التلقائية.</span><span class="sxs-lookup"><span data-stu-id="5f189-108">**Suspended**: The system is no longer eligible to receive automatic upgrades.</span></span> <span data-ttu-id="5f189-109">لا يمكنك تكوين هذه القيمة ؛ تم تعيينه بواسطة النظام.</span><span class="sxs-lookup"><span data-stu-id="5f189-109">You can't configure this value; it's set by the system.</span></span>

<span data-ttu-id="5f189-110">لمزيد من المعلومات ، راجع [الترقية التلقائية](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span><span class="sxs-lookup"><span data-stu-id="5f189-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>

<span data-ttu-id="5f189-111">لتنزيل الإصدار الأخير من Azure AD Connect ، انتقل إلى [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594) .</span><span class="sxs-lookup"><span data-stu-id="5f189-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
