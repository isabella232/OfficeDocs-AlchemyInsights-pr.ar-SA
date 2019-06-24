---
title: إصلاح الخطأ 0x8004de40 في أندريف
ms.author: kirks
author: Techwriter40
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 2256fb66cb7a4e2adcff9fda16a80c87e2997f0c
ms.sourcegitcommit: 8f6a1be929b275faa295ba8aeeae17898a47c3b0
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/21/2019
ms.locfileid: "35133964"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="9f637-102">إصلاح الخطأ 0x8004de40 في أندريف</span><span class="sxs-lookup"><span data-stu-id="9f637-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="9f637-103">إذا تلقيت خطأ 0x8004de40 أندريف:</span><span class="sxs-lookup"><span data-stu-id="9f637-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="9f637-104">إعادة تمهيد الكمبيوتر المتأثرة أثناء الاتصال بالمجال الدليل Acitve.</span><span class="sxs-lookup"><span data-stu-id="9f637-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="9f637-105">إذا لم يصلح إعادة تشغيل المشكلة، فصل والعودة إلى الجهاز من الإعلان Azure.</span><span class="sxs-lookup"><span data-stu-id="9f637-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="9f637-106">**ملاحظة**: يجب أن يكون على شبكة الشركة أثناء تنفيذ هذه الخطوات.</span><span class="sxs-lookup"><span data-stu-id="9f637-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="9f637-107">عدم إجراء الخطوات التالية عندما لم تكن قادرة على الاتصال بالبنية الأساسية للشركة الخاصة بك (على سبيل المثال، أثناء السفر).</span><span class="sxs-lookup"><span data-stu-id="9f637-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="9f637-108">فتح موجه أوامر غير مقيد.</span><span class="sxs-lookup"><span data-stu-id="9f637-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="9f637-109">لفتح موجه أوامر غير مقيد، انقر فوق- **ابدأ**زر الماوس الأيمن فوق **موجه الأوامر**وانقر فوق **تشغيل كمسؤول**.</span><span class="sxs-lookup"><span data-stu-id="9f637-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="9f637-110">اكتب */leave دسريجكمد* ، ثم اضغط **Enter**.</span><span class="sxs-lookup"><span data-stu-id="9f637-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="9f637-111">عند الانتهاء، اكتب */join دسريجكمد* واضغط **Enter**.</span><span class="sxs-lookup"><span data-stu-id="9f637-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="9f637-112">عند الانتهاء، أغلق موجه الأوامر.</span><span class="sxs-lookup"><span data-stu-id="9f637-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="9f637-113">إعادة تشغيل الكمبيوتر وتسجيل الدخول إلى أندريف.</span><span class="sxs-lookup"><span data-stu-id="9f637-113">Reboot the computer, and log into OneDrive.</span></span>