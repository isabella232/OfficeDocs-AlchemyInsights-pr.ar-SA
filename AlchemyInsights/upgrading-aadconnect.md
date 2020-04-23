---
title: 932 ترقية AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: fcc5fddb5cfd15407d0533449035317d187931ed
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766480"
---
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="19172-102">ترقية اتصال Azure AD</span><span class="sxs-lookup"><span data-stu-id="19172-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="19172-103">بشكل افتراضي، يتم تمكين الترقية التلقائية لـ Azure AD Connect، مما يساعد على ضمان تشغيل أحدث إصدار.</span><span class="sxs-lookup"><span data-stu-id="19172-103">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version.</span></span> <span data-ttu-id="19172-104">للتحقق من إعدادات الترقية التلقائية، استخدم **cmdlet Get-ADSyncAutoUpgrade** في Azure AD PowerShell.</span><span class="sxs-lookup"><span data-stu-id="19172-104">To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell.</span></span> <span data-ttu-id="19172-105">سيعود cmdlet إحدى القيم التالية:</span><span class="sxs-lookup"><span data-stu-id="19172-105">The cmdlet will return one of following values:</span></span>

- <span data-ttu-id="19172-106">**ممكّن:** تم تمكين الترقية التلقائية.</span><span class="sxs-lookup"><span data-stu-id="19172-106">**Enabled**: Automatic upgrade is enabled.</span></span>

- <span data-ttu-id="19172-107">**معطل:** تم تعطيل الترقية التلقائية.</span><span class="sxs-lookup"><span data-stu-id="19172-107">**Disabled**: Automatic upgrade is disabled.</span></span>

- <span data-ttu-id="19172-108">**مع وقف التنفيذ:** لم يعد النظام مؤهلاً لتلقي ترقيات تلقائية.</span><span class="sxs-lookup"><span data-stu-id="19172-108">**Suspended**: The system is no longer eligible to receive automatic upgrades.</span></span> <span data-ttu-id="19172-109">لا يمكنك تكوين هذه القيمة; تم تعيينها من قبل النظام.</span><span class="sxs-lookup"><span data-stu-id="19172-109">You can't configure this value; it's set by the system.</span></span>

<span data-ttu-id="19172-110">لمزيد من المعلومات، راجع [الترقية التلقائية](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span><span class="sxs-lookup"><span data-stu-id="19172-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>

<span data-ttu-id="19172-111">لتحميل أحدث إصدار من Azure AD [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594)Connect، انتقل إلى .</span><span class="sxs-lookup"><span data-stu-id="19172-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
