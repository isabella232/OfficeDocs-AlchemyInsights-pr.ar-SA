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
ms.openlocfilehash: d436184bdc0e283db217ea734fb2c8e05f85b4e7
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/22/2019
ms.locfileid: "36525046"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="9e35f-102">إصلاح الخطأ 0x8004de40 في أندريف</span><span class="sxs-lookup"><span data-stu-id="9e35f-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="9e35f-103">إذا تلقيت خطأ 0x8004de40 أندريف:</span><span class="sxs-lookup"><span data-stu-id="9e35f-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="9e35f-104">إعادة تمهيد الكمبيوتر المتأثرة أثناء الاتصال بالمجال الدليل Acitve.</span><span class="sxs-lookup"><span data-stu-id="9e35f-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="9e35f-105">إذا لم يصلح إعادة تشغيل المشكلة، فصل والعودة إلى الجهاز من الإعلان Azure.</span><span class="sxs-lookup"><span data-stu-id="9e35f-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="9e35f-106">**ملاحظة**: يجب أن يكون على شبكة الشركة أثناء تنفيذ هذه الخطوات.</span><span class="sxs-lookup"><span data-stu-id="9e35f-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="9e35f-107">عدم إجراء الخطوات التالية عندما لم تكن قادرة على الاتصال بالبنية الأساسية للشركة الخاصة بك (على سبيل المثال، أثناء السفر).</span><span class="sxs-lookup"><span data-stu-id="9e35f-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="9e35f-108">فتح موجه أوامر غير مقيد.</span><span class="sxs-lookup"><span data-stu-id="9e35f-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="9e35f-109">لفتح موجه أوامر غير مقيد، انقر فوق- **ابدأ**زر الماوس الأيمن فوق **موجه الأوامر**وانقر فوق **تشغيل كمسؤول**.</span><span class="sxs-lookup"><span data-stu-id="9e35f-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="9e35f-110">اكتب */leave دسريجكمد* ، ثم اضغط **Enter**.</span><span class="sxs-lookup"><span data-stu-id="9e35f-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="9e35f-111">عند الانتهاء، اكتب */join دسريجكمد* واضغط **Enter**.</span><span class="sxs-lookup"><span data-stu-id="9e35f-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="9e35f-112">عند الانتهاء، أغلق موجه الأوامر.</span><span class="sxs-lookup"><span data-stu-id="9e35f-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="9e35f-113">إعادة تشغيل الكمبيوتر وتسجيل الدخول إلى أندريف.</span><span class="sxs-lookup"><span data-stu-id="9e35f-113">Reboot the computer, and log into OneDrive.</span></span>