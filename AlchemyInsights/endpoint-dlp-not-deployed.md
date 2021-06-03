---
title: نقطة النهاية DLP غير منشرة على جهاز المستخدم
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/27/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11470"
- "9000292"
ms.openlocfilehash: 948835f5468b480536c176bfdf3b4eefb76b3bdb
ms.sourcegitcommit: c32233a1b7e6f1b07913d25f90189a58a8de2560
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/27/2021
ms.locfileid: "52731246"
---
# <a name="endpoint-dlp-not-deployed-to-users-device"></a><span data-ttu-id="6c226-102">نقطة النهاية DLP غير منشرة على جهاز المستخدم</span><span class="sxs-lookup"><span data-stu-id="6c226-102">Endpoint DLP not deployed to user's device</span></span>

<span data-ttu-id="6c226-103">إذا لم يتم تطبيق إعداد منع فقدان بيانات نقطة النهاية (DLP) على جهاز مستخدم، فتأكد من أنك تلبي هذه المتطلبات:</span><span class="sxs-lookup"><span data-stu-id="6c226-103">If the Endpoint data loss prevention (DLP) setting has not applied to a user's device, confirm you meet these requirements:</span></span>

- <span data-ttu-id="6c226-104">Windows 10 x64 1809 أو أي وقت لاحق مثبتا على الجهاز.</span><span class="sxs-lookup"><span data-stu-id="6c226-104">Windows 10 x64 build 1809 or later is installed on the device.</span></span>
- <span data-ttu-id="6c226-105">تم تثبيت إصدار عميل مكافحة البرامج الضارة 4.18.2009.7 أو إصدار أحدث.</span><span class="sxs-lookup"><span data-stu-id="6c226-105">Anti-malware client version 4.18.2009.7 or later is installed.</span></span>
- <span data-ttu-id="6c226-106">الجهاز هو **أحد** هذه:</span><span class="sxs-lookup"><span data-stu-id="6c226-106">The device is **one** of these:</span></span>
    
    - <span data-ttu-id="6c226-107">Azure Active Directory (Azure AD) المنضم</span><span class="sxs-lookup"><span data-stu-id="6c226-107">Azure Active Directory (Azure AD) joined</span></span>
    - <span data-ttu-id="6c226-108">Azure AD المختلط المنضم</span><span class="sxs-lookup"><span data-stu-id="6c226-108">Hybrid Azure AD joined</span></span>
    - <span data-ttu-id="6c226-109">AAD مسجل</span><span class="sxs-lookup"><span data-stu-id="6c226-109">AAD registered</span></span>

- <span data-ttu-id="6c226-110">لفرض إجراءات النهج، تأكد من تثبيت microsoft Chromium Edge على جهاز نقطة النهاية.</span><span class="sxs-lookup"><span data-stu-id="6c226-110">To enforce policy actions, make sure Microsoft Chromium Edge browser is installed on the endpoint device.</span></span>

<span data-ttu-id="6c226-111">للحصول على متطلبات إضافية لنشر نقطة النهاية DLP، راجع بدء استخدام منع [فقدان بيانات نقطة النهاية](/microsoft-365/compliance/endpoint-dlp-getting-started#prepare-your-endpoints).</span><span class="sxs-lookup"><span data-stu-id="6c226-111">For additional requirements for deploying Endpoint DLP, see [Get started with Endpoint data loss prevention](/microsoft-365/compliance/endpoint-dlp-getting-started#prepare-your-endpoints).</span></span>