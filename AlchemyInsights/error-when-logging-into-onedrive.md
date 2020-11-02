---
title: ظهور رسالة الخطا 0x8004de40 عند بدء تشغيل OneDrive
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6886"
- "9003837"
ms.openlocfilehash: f689fcf9432e9b356843efe73ed0f79a32735e6f
ms.sourcegitcommit: 1ac3474897abb7c4969e222f934294e05f468536
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/30/2020
ms.locfileid: "48822985"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a><span data-ttu-id="1bdf3-102">ظهور رسالة الخطا 0x8004de40 عند بدء تشغيل OneDrive</span><span class="sxs-lookup"><span data-stu-id="1bdf3-102">0x8004de40 error when launching OneDrive</span></span>

<span data-ttu-id="1bdf3-103">إذا تلقيت رسالة خطا **0x8004de40** عند تسجيل الدخول إلى OneDrive ، فأعد تشغيل الكمبيوتر اثناء الاتصال بمجال العمل أو المؤسسة التعليمية.</span><span class="sxs-lookup"><span data-stu-id="1bdf3-103">If you receive an error **0x8004de40** when  logging into OneDrive, reboot the computer while connected to your work or school domain.</span></span> <span data-ttu-id="1bdf3-104">إذا ظهرت رسالة الخطا هذه بعد أعاده التشغيل ، فحاول القيام بذلك اثناء الاتصال بمجال العمل أو المؤسسة التعليمية:</span><span class="sxs-lookup"><span data-stu-id="1bdf3-104">If you receive this error after rebooting, try this while connected to your work or school domain:</span></span>

1. <span data-ttu-id="1bdf3-105">انقر فوق أبدا ، واكتب **cmd** أو **موجه الأوامر**  في مربع البحث ، وانقر بزر الماوس الأيمن فوق تطبيق موجه الأوامر ، ثم حدد  **تشغيل كمسؤول** .</span><span class="sxs-lookup"><span data-stu-id="1bdf3-105">Click Start, and type **cmd** or **command prompt**  in the search  box, right-click on the command prompt app, and select  **Run as administrator** .</span></span> <span data-ttu-id="1bdf3-106">إذا تمت مطالبتك بإدخال كلمه مرور مسؤول أو تاكيدها ، فاكتب كلمه المرور ، أو انقر فوق **السماح** .</span><span class="sxs-lookup"><span data-stu-id="1bdf3-106">If you are prompted for an administrator password or for a confirmation, type the password, or click **Allow** .</span></span>  

2. <span data-ttu-id="1bdf3-107">في نافذه موجه الأوامر ، اكتب **دسريجكمد/leave خروج**  وانتظر حتى يكتمل الأمر.</span><span class="sxs-lookup"><span data-stu-id="1bdf3-107">In the Command Prompt window, type **dsregcmd /leave**  and wait for the command to complete.</span></span> <span data-ttu-id="1bdf3-108">ثم اكتب **دسريجكمد/join** وانتظر حتى يكتمل الأمر.</span><span class="sxs-lookup"><span data-stu-id="1bdf3-108">Then type **dsregcmd /join** and wait for the command to complete.</span></span>
3. <span data-ttu-id="1bdf3-109">أعد تشغيل الكمبيوتر.</span><span class="sxs-lookup"><span data-stu-id="1bdf3-109">Reboot your computer.</span></span>
