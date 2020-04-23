---
title: إصلاح 0x8004de40 خطأ في OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 5da4271f242597b195ef61d553fd4a2ffb313025
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716015"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="90cbc-102">إصلاح 0x8004de40 خطأ في OneDrive</span><span class="sxs-lookup"><span data-stu-id="90cbc-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="90cbc-103">إذا تلقيت خطأ 0x8004de40 مع OneDrive:</span><span class="sxs-lookup"><span data-stu-id="90cbc-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="90cbc-104">إعادة تشغيل الكمبيوتر المتأثر أثناء الاتصال بمجال دليل Acitve.</span><span class="sxs-lookup"><span data-stu-id="90cbc-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="90cbc-105">إذا لم تعمل إعادة التشغيل على حل المشكلة، فإلغاء الانضمام إلى جهازك وإعادة الانضمام إليه من Azure AD.</span><span class="sxs-lookup"><span data-stu-id="90cbc-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="90cbc-106">**ملاحظة:** يجب أن تكون على شبكة الشركة أثناء تنفيذ هذه الخطوات.</span><span class="sxs-lookup"><span data-stu-id="90cbc-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="90cbc-107">لا تقم بتنفيذ هذه الخطوات عندما لا تتمكن من الاتصال بالبنية التحتية للشركة (على سبيل المثال، أثناء السفر).</span><span class="sxs-lookup"><span data-stu-id="90cbc-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="90cbc-108">افتح موجه أمر مرتفع.</span><span class="sxs-lookup"><span data-stu-id="90cbc-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="90cbc-109">لفتح مطالبة أمر مرتفعة، انقر فوق - **ابدأ،** انقر بزر الماوس الأيمن **موجه الأوامر،** ثم انقر فوق **تشغيل كمسؤول**.</span><span class="sxs-lookup"><span data-stu-id="90cbc-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="90cbc-110">نوع *dsregcmd / ترك* واضغط **أدخل**.</span><span class="sxs-lookup"><span data-stu-id="90cbc-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="90cbc-111">عند الانتهاء، اكتب *dsregcmd / الانضمام* واضغط **أدخل**.</span><span class="sxs-lookup"><span data-stu-id="90cbc-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="90cbc-112">عند الانتهاء، أغلق موجه الأمر.</span><span class="sxs-lookup"><span data-stu-id="90cbc-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="90cbc-113">إعادة تشغيل الكمبيوتر، وتسجيل الدخول إلى OneDrive.</span><span class="sxs-lookup"><span data-stu-id="90cbc-113">Reboot the computer, and log into OneDrive.</span></span>