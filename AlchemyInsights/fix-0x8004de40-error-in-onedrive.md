---
title: إصلاح 0x8004de40 خطأ في أندريف
ms.author: pebaum
author: Techwriter40
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: aa0e0a63ac1e365a7cdce018626740446040a664
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/04/2019
ms.locfileid: "36755835"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="8a08f-102">إصلاح 0x8004de40 خطأ في أندريف</span><span class="sxs-lookup"><span data-stu-id="8a08f-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="8a08f-103">إذا تلقيت خطأ 0x8004de40 مع أندريف:</span><span class="sxs-lookup"><span data-stu-id="8a08f-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="8a08f-104">إعادة تمهيد الكمبيوتر المتأثر أثناء الاتصال بمجال دليل Acitve.</span><span class="sxs-lookup"><span data-stu-id="8a08f-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="8a08f-105">إذا لم تنجح إعادة التشغيل في حل المشكلة، قم بإلغاء الانضمام إلى جهازك والانضمام إليه من إعلان Azure.</span><span class="sxs-lookup"><span data-stu-id="8a08f-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="8a08f-106">**ملاحظة:** يجب أن تكون على شبكة الشركة أثناء تنفيذ هذه الخطوات.</span><span class="sxs-lookup"><span data-stu-id="8a08f-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="8a08f-107">لا تقم بتنفيذ هذه الخطوات عندما لا تتمكن من الاتصال بالبنية التحتية للشركة (على سبيل المثال، أثناء السفر).</span><span class="sxs-lookup"><span data-stu-id="8a08f-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="8a08f-108">افتح موجه أوامر غير مقيد.</span><span class="sxs-lookup"><span data-stu-id="8a08f-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="8a08f-109">لفتح موجه أوامر غير مقيد، انقر فوق - **ابدأ**، انقر بزر الماوس الأيمن فوق **موجه الأوامر**، ثم انقر فوق **تشغيل كمسؤول**.</span><span class="sxs-lookup"><span data-stu-id="8a08f-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="8a08f-110">اكتب *dsregcmd /leave* واضغط **على Enter**.</span><span class="sxs-lookup"><span data-stu-id="8a08f-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="8a08f-111">عند الاكتمال، اكتب *dsregcmd /join* واضغط **على Enter**.</span><span class="sxs-lookup"><span data-stu-id="8a08f-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="8a08f-112">عند الاكتمال، أغلق موجه الأوامر.</span><span class="sxs-lookup"><span data-stu-id="8a08f-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="8a08f-113">إعادة تمهيد الكمبيوتر ثم قم بتسجيل الدخول إلى أندريف.</span><span class="sxs-lookup"><span data-stu-id="8a08f-113">Reboot the computer, and log into OneDrive.</span></span>