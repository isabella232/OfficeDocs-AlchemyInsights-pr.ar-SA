---
title: Exchange PowerShell وإهمال المصادقة الأساسية
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "4577"
ms.openlocfilehash: 01938a59b53ccf8b7867ed9c256e141205d31dff
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813459"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a><span data-ttu-id="1aad1-102">Exchange PowerShell وإهمال المصادقة الأساسية</span><span class="sxs-lookup"><span data-stu-id="1aad1-102">Exchange PowerShell and basic authentication deprecation</span></span>

<span data-ttu-id="1aad1-103">للحصول على أحدث المعلومات حول كيفية الاتصال بـ Exchange Online PowerShell بدون استخدام المصادقة الأساسية، [الرجاء الانتقال إلى هنا](https://aka.ms/exops-docs).</span><span class="sxs-lookup"><span data-stu-id="1aad1-103">For the latest information about how to connect to Exchange Online PowerShell without the use of Basic Authentication, [please go here](https://aka.ms/exops-docs).</span></span> <span data-ttu-id="1aad1-104">لا تستخدم الوحدة النمطية PowerShell V2 المصادقة الأساسية.</span><span class="sxs-lookup"><span data-stu-id="1aad1-104">The PowerShell V2 module does not use basic authentication.</span></span>

<span data-ttu-id="1aad1-105">الرجاء ملاحظة أن تمكين المصادقة الأساسية ما زال مطلوباً على جهاز العميل.</span><span class="sxs-lookup"><span data-stu-id="1aad1-105">Please note that Basic Authentication still needs to be enabled on your client machine.</span></span>
<span data-ttu-id="1aad1-106">تستخدم الوحدة النمطية الجديدة للإصدار 2 من PowerShell المصادقة الحديثة لإنشاء اتصال لتمكين كل أوامر Cmdlet للإصدار 2 المستندة إلى REST.</span><span class="sxs-lookup"><span data-stu-id="1aad1-106">The new PowerShell V2 module uses Modern Auth to establish connection for enabling all of REST-based V2 Cmdlets.</span></span> <span data-ttu-id="1aad1-107">بالإضافة إلى أوامر Cmdlet للإصدار 2، يتم السماح لك أيضاً بالوصول إلى أوامر Cmdlet لـ "PowerShell عن بُعد" (RPS) القديمة التي تتطلب إنشاء جلسة "PowerShell عن بُعد".</span><span class="sxs-lookup"><span data-stu-id="1aad1-107">In addition to V2 cmdlets, it also allows you to access older Remote PowerShell (RPS) Cmdlets which requires a Remote PowerShell session to be established.</span></span> <span data-ttu-id="1aad1-108">يتطلب إنشاء جلسة "PowerShell عن بُعد" (RPS) على جهاز Windows تمكين المصادقة الأساسية للإدارة عن بعد من Windows "WinRM BasicAuth" على جهاز العميل حتى لو كانت الوحدة النمطية تستخدم آلية المصادقة الحديثة "Modern Auth" لمصادقة الخدمة.</span><span class="sxs-lookup"><span data-stu-id="1aad1-108">Establishing an RPS session on Windows machine requires WinRM BasicAuth to be enabled on the client machine even though the module uses Modern Auth mechanism to authenticate to the service.</span></span> <span data-ttu-id="1aad1-109">يُستخدم مسار المصادقة الأساسية لـ "WinRM" لنقل الرموز المميزة للمصادقة الحديثة.</span><span class="sxs-lookup"><span data-stu-id="1aad1-109">The WinRM Basic Auth pipeline is used for transporting Modern Auth tokens.</span></span> <span data-ttu-id="1aad1-110">إذا تم تعطيل المصادقة الأساسية لـ "WinRM" على جهاز العميل، فإن أوامر cmdlet للإصدار 2 الجديدة ستستمر في العمل (ولكن لن تعمل أوامر cmdlet لـ RPS القديمة).</span><span class="sxs-lookup"><span data-stu-id="1aad1-110">If WinRM Basic Auth is disabled on the client machine, the new V2 cmdlets will continue to work (but the older RPS cmdlets will not).</span></span>
