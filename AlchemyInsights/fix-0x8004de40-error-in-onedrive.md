---
title: إصلاح خطا 0x8004de40 في OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: b9bd6dff48f78063e3d47f5fe2f834f59eb9868a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47745117"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="96d90-102">إصلاح خطا 0x8004de40 في OneDrive</span><span class="sxs-lookup"><span data-stu-id="96d90-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="96d90-103">إذا تلقيت رسالة الخطا 0x8004de40 في OneDrive:</span><span class="sxs-lookup"><span data-stu-id="96d90-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="96d90-104">أعد تشغيل الكمبيوتر المتاثر اثناء الاتصال بمجال دليل أسيتفي.</span><span class="sxs-lookup"><span data-stu-id="96d90-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="96d90-105">إذا لم يؤد أعاده التشغيل إلى حل المشكلة ، فقم بأونجوين الجهاز وأعاده الانضمام اليه من Azure AD.</span><span class="sxs-lookup"><span data-stu-id="96d90-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="96d90-106">**ملاحظه**: يجب ان تكون علي شبكه الشركة لديك اثناء تنفيذ هذه الخطوات.</span><span class="sxs-lookup"><span data-stu-id="96d90-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="96d90-107">لا تقم بتنفيذ هذه الخطوات إذا لم تتمكن من الاتصال بالبنية الاساسيه لشركك (علي سبيل المثال ، اثناء السفر).</span><span class="sxs-lookup"><span data-stu-id="96d90-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="96d90-108">افتح موجه أوامر غير مقيد.</span><span class="sxs-lookup"><span data-stu-id="96d90-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="96d90-109">لفتح موجه أوامر غير مقيد ، انقر فوق- **بدء**، وانقر بزر الماوس الأيمن فوق **موجه الأوامر**، ثم انقر فوق **تشغيل كمسؤول**.</span><span class="sxs-lookup"><span data-stu-id="96d90-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="96d90-110">اكتب *دسريجكمد/leave خروج* واضغط علي مفتاح **الإدخال Enter**.</span><span class="sxs-lookup"><span data-stu-id="96d90-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="96d90-111">عند الانتهاء ، اكتب *دسريجكمد/join* واضغط علي مفتاح **الإدخال Enter**.</span><span class="sxs-lookup"><span data-stu-id="96d90-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="96d90-112">عند الانتهاء ، اغلق موجه الأوامر.</span><span class="sxs-lookup"><span data-stu-id="96d90-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="96d90-113">أعد تشغيل الكمبيوتر ، ثم سجل دخولك إلى OneDrive.</span><span class="sxs-lookup"><span data-stu-id="96d90-113">Reboot the computer, and log into OneDrive.</span></span>