---
title: إصلاح خطا 0x8004de40 في اندريف
ms.author: pebaum
author: pebaum
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 48b29f57763ca22a71a23b2afddcac0e8e8a95db
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/15/2019
ms.locfileid: "40052024"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="97581-102">إصلاح خطا 0x8004de40 في اندريف</span><span class="sxs-lookup"><span data-stu-id="97581-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="97581-103">إذا تلقيت خطا 0x8004de40 مع اندريف:</span><span class="sxs-lookup"><span data-stu-id="97581-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="97581-104">أعاده تمهيد الكمبيوتر المتاثر اثناء الاتصال بمجال دليل Acitve.</span><span class="sxs-lookup"><span data-stu-id="97581-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="97581-105">إذا لم يصلح أعاده التشغيل المشكلة ، قم بإلغاء الانضمام والانضمام إلى جهازك من Azure AD.</span><span class="sxs-lookup"><span data-stu-id="97581-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="97581-106">**ملاحظه**: يجب ان تكون علي شبكه الشركة اثناء تنفيذ هذه الخطوات.</span><span class="sxs-lookup"><span data-stu-id="97581-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="97581-107">لا تقم بتنفيذ هذه الخطوات عندما لا تتمكن من الاتصال بالبنية الاساسيه للشركة (علي سبيل المثال ، اثناء السفر).</span><span class="sxs-lookup"><span data-stu-id="97581-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="97581-108">افتح موجه أوامر غير مقيد.</span><span class="sxs-lookup"><span data-stu-id="97581-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="97581-109">لفتح موجه أوامر غير مقيد ، انقر فوق **أبدا**، انقر بزر الماوس الأيمن فوق **موجه الأوامر**، ثم انقر فوق **تشغيل كمسؤول**.</span><span class="sxs-lookup"><span data-stu-id="97581-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="97581-110">اكتب *dsregcmd/اترك* واضغط **Enter**.</span><span class="sxs-lookup"><span data-stu-id="97581-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="97581-111">عند الاكتمال ، اكتب *dsregcmd/join* واضغط **Enter**.</span><span class="sxs-lookup"><span data-stu-id="97581-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="97581-112">عند الاكتمال ، اغلق موجه الأوامر.</span><span class="sxs-lookup"><span data-stu-id="97581-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="97581-113">أعاده تمهيد الكمبيوتر ، وتسجيل الدخول إلى OneDrive.</span><span class="sxs-lookup"><span data-stu-id="97581-113">Reboot the computer, and log into OneDrive.</span></span>