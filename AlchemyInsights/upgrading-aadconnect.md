---
title: 932 آدكونيكت الترقية
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: ff3f74348599788edd8ce0991fe49bb6a54b55af
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/22/2019
ms.locfileid: "36506070"
---
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="32186-102">ترقية الإعلان Azure الاتصال</span><span class="sxs-lookup"><span data-stu-id="32186-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="32186-103">بشكل افتراضي، يتم تمكين تحديث تلقائي للاتصال الإعلان أزور، التي تساعد على ضمان أنك تقوم بتشغيل أحدث إصدار.</span><span class="sxs-lookup"><span data-stu-id="32186-103">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version.</span></span> <span data-ttu-id="32186-104">للتحقق من إعدادات الترقية التلقائية، استخدم cmdlet **الحصول على أدسينكاوتوبجرادي** في PowerShell الإعلان Azure.</span><span class="sxs-lookup"><span data-stu-id="32186-104">To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell.</span></span> <span data-ttu-id="32186-105">Cmdlet سيتم إرجاع إحدى القيم التالية:</span><span class="sxs-lookup"><span data-stu-id="32186-105">The cmdlet will return one of following values:</span></span>

- <span data-ttu-id="32186-106">**تمكين**: تمكين التحديث التلقائي.</span><span class="sxs-lookup"><span data-stu-id="32186-106">**Enabled**: Automatic upgrade is enabled.</span></span>

- <span data-ttu-id="32186-107">**تعطيل**: تم تعطيل التحديث التلقائي.</span><span class="sxs-lookup"><span data-stu-id="32186-107">**Disabled**: Automatic upgrade is disabled.</span></span>

- <span data-ttu-id="32186-108">**معلق**: النظام لم تعد مؤهلة للحصول على تحديثات تلقائية.</span><span class="sxs-lookup"><span data-stu-id="32186-108">**Suspended**: The system is no longer eligible to receive automatic upgrades.</span></span> <span data-ttu-id="32186-109">لا يمكنك تكوين هذه القيمة؛ يتم تعيينها بواسطة النظام.</span><span class="sxs-lookup"><span data-stu-id="32186-109">You can't configure this value; it's set by the system.</span></span>

<span data-ttu-id="32186-110">لمزيد من المعلومات، راجع [تحديث تلقائي](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span><span class="sxs-lookup"><span data-stu-id="32186-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>

<span data-ttu-id="32186-111">لتنزيل أحدث إصدار من الاتصال الإعلان أزور، انتقل إلى [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span><span class="sxs-lookup"><span data-stu-id="32186-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
