---
title: Exchange PowerShell وإهمال المصادقة الأساسية
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "4577"
ms.openlocfilehash: 24d59860732b42e8d62da8c1a8c37f2018a0d126
ms.sourcegitcommit: 264b782ac2fba8ffd84524180dc4f7d60b45e9a4
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/04/2020
ms.locfileid: "44015676"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a><span data-ttu-id="93d88-102">Exchange PowerShell وإهمال المصادقة الأساسية</span><span class="sxs-lookup"><span data-stu-id="93d88-102">Exchange PowerShell and basic authentication deprecation</span></span>

<span data-ttu-id="93d88-103">للحصول على أحدث المعلومات حول كيفية الاتصال بـ Exchange Online PowerShell بدون استخدام المصادقة الأساسية، [الرجاء الانتقال إلى هنا](https://aka.ms/psbasicauth).</span><span class="sxs-lookup"><span data-stu-id="93d88-103">For the latest information about how to connect to Exchange Online PowerShell without the use of Basic Authentication, [please go here](https://aka.ms/psbasicauth).</span></span>

<span data-ttu-id="93d88-104">الرجاء ملاحظة أن تمكين المصادقة الأساسية ما زال مطلوباً على جهاز العميل.</span><span class="sxs-lookup"><span data-stu-id="93d88-104">Please note that Basic Authentication still needs to be enabled on your client machine.</span></span>
<span data-ttu-id="93d88-105">تستخدم الوحدة النمطية الجديدة للإصدار 2 من PowerShell المصادقة الحديثة لإنشاء اتصال لتمكين كل أوامر Cmdlet للإصدار 2 المستندة إلى REST.</span><span class="sxs-lookup"><span data-stu-id="93d88-105">The new PowerShell V2 module uses Modern Auth to establish connection for enabling all of REST-based V2 Cmdlets.</span></span> <span data-ttu-id="93d88-106">بالإضافة إلى أوامر Cmdlet للإصدار 2، يتم السماح لك أيضاً بالوصول إلى أوامر Cmdlet لـ "PowerShell عن بُعد" (RPS) القديمة التي تتطلب إنشاء جلسة "PowerShell عن بُعد".</span><span class="sxs-lookup"><span data-stu-id="93d88-106">In addition to V2 cmdlets, it also allows you to access older Remote PowerShell (RPS) Cmdlets which requires a Remote PowerShell session to be established.</span></span> <span data-ttu-id="93d88-107">يتطلب إنشاء جلسة "PowerShell عن بُعد" (RPS) على جهاز Windows تمكين المصادقة الأساسية للإدارة عن بعد من Windows "WinRM BasicAuth" على جهاز العميل حتى لو كانت الوحدة النمطية تستخدم آلية المصادقة الحديثة "Modern Auth" لمصادقة الخدمة.</span><span class="sxs-lookup"><span data-stu-id="93d88-107">Establishing an RPS session on Windows machine requires WinRM BasicAuth to be enabled on the client machine even though the module uses Modern Auth mechanism to authenticate to the service.</span></span> <span data-ttu-id="93d88-108">يُستخدم مسار المصادقة الأساسية لـ "WinRM" لنقل الرموز المميزة للمصادقة الحديثة.</span><span class="sxs-lookup"><span data-stu-id="93d88-108">The WinRM Basic Auth pipeline is used for transporting Modern Auth tokens.</span></span> <span data-ttu-id="93d88-109">إذا تم تعطيل المصادقة الأساسية لـ "WinRM" على جهاز العميل، فإن أوامر cmdlet للإصدار 2 الجديدة ستستمر في العمل (ولكن لن تعمل أوامر cmdlet لـ RPS القديمة).</span><span class="sxs-lookup"><span data-stu-id="93d88-109">If WinRM Basic Auth is disabled on the client machine, the new V2 cmdlets will continue to work (but the older RPS cmdlets will not).</span></span>
