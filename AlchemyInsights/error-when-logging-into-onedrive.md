---
title: 0x8004de40 خطأ عند تشغيل OneDrive
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6886"
- "9003837"
ms.openlocfilehash: e329d7fe881a0fc9514584e06aa2d6e8ebab5b11
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813639"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a><span data-ttu-id="fab28-102">0x8004de40 خطأ عند تشغيل OneDrive</span><span class="sxs-lookup"><span data-stu-id="fab28-102">0x8004de40 error when launching OneDrive</span></span>

<span data-ttu-id="fab28-103">إذا تلقيت رسالة خطأ **0x8004de40** عند تسجيل الدخول إلى OneDrive، ف إعادة تشغيل الكمبيوتر أثناء الاتصال بمجال العمل أو المدرسة.</span><span class="sxs-lookup"><span data-stu-id="fab28-103">If you receive an error **0x8004de40** when  logging into OneDrive, reboot the computer while connected to your work or school domain.</span></span> <span data-ttu-id="fab28-104">إذا تلقيت هذا الخطأ بعد إعادة التشغيل، فجرب ذلك أثناء الاتصال بمجال العمل أو المدرسة:</span><span class="sxs-lookup"><span data-stu-id="fab28-104">If you receive this error after rebooting, try this while connected to your work or school domain:</span></span>

1. <span data-ttu-id="fab28-105">انقر فوق بدء، وا اكتب **cmd** أو **موجه الأوامر**  في مربع البحث، وانقر بيمين فوق تطبيق موجه الأوامر، وحدد  **تشغيل كمسؤول**.</span><span class="sxs-lookup"><span data-stu-id="fab28-105">Click Start, and type **cmd** or **command prompt**  in the search  box, right-click on the command prompt app, and select  **Run as administrator**.</span></span> <span data-ttu-id="fab28-106">إذا تم مطالبتك بكلمة مرور المسؤول أو للتأكيد، فا اكتب كلمة المرور، أو انقر فوق **السماح**.</span><span class="sxs-lookup"><span data-stu-id="fab28-106">If you are prompted for an administrator password or for a confirmation, type the password, or click **Allow**.</span></span>  

2. <span data-ttu-id="fab28-107">في نافذة موجه الأوامر، اكتب **dsregcmd/leave**  وانتظر حتى اكتمال الأمر.</span><span class="sxs-lookup"><span data-stu-id="fab28-107">In the Command Prompt window, type **dsregcmd /leave**  and wait for the command to complete.</span></span> <span data-ttu-id="fab28-108">ثم اكتب **dsregcmd /join** وانتظر حتى اكتمال الأمر.</span><span class="sxs-lookup"><span data-stu-id="fab28-108">Then type **dsregcmd /join** and wait for the command to complete.</span></span>
3. <span data-ttu-id="fab28-109">إعادة تشغيل الكمبيوتر.</span><span class="sxs-lookup"><span data-stu-id="fab28-109">Reboot your computer.</span></span>
