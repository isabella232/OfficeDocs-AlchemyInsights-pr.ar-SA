---
title: 'استكشاف أخطاء البريد الصوتي '
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/09/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002347"
- "7564"
ms.openlocfilehash: a2d26da512838ae112c352fe21366074b69fa224
ms.sourcegitcommit: 3802f2f4db4f53a408a360187db67f2296448c21
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/09/2020
ms.locfileid: "49676731"
---
# <a name="troubleshooting-voicemail"></a><span data-ttu-id="a8e71-102">استكشاف أخطاء البريد الصوتي</span><span class="sxs-lookup"><span data-stu-id="a8e71-102">Troubleshooting Voicemail</span></span>

<span data-ttu-id="a8e71-103">تاكد من ان ميزه مشغول علي مشغول.</span><span class="sxs-lookup"><span data-stu-id="a8e71-103">Ensure that the Busy on Busy feature is intentional.</span></span>

<span data-ttu-id="a8e71-104">إذا لم تكن هذه الميزة ضرورية علي هذا المستخدم:</span><span class="sxs-lookup"><span data-stu-id="a8e71-104">If this feature is not needed on this user:</span></span>

1. <span data-ttu-id="a8e71-105">انتقل إلى [مركز أداره الفرق](https://admin.teams.microsoft.com/policies/calling).</span><span class="sxs-lookup"><span data-stu-id="a8e71-105">Go to [Teams Admin center](https://admin.teams.microsoft.com/policies/calling).</span></span>
1. <span data-ttu-id="a8e71-106">في الصفحة اليمني ، انتقل إلى  >  أداره **نهج الاتصال** الصوتي  >  **النهج** في **نهج الاتصال**.</span><span class="sxs-lookup"><span data-stu-id="a8e71-106">On the left rail navigate **Voice** > **Calling policies** > **Manage Policies** on the **Calling Policy**.</span></span>
1. <span data-ttu-id="a8e71-107">حدد **أداره المستخدمين**.</span><span class="sxs-lookup"><span data-stu-id="a8e71-107">Select **Manage Users**.</span></span>
1. <span data-ttu-id="a8e71-108">يتوفر البحث عن المستخدم وتغيير نهج الاتصال إلى الآخر الذي يكون **مشغولا عليه مشغولا عند اجراء مكالمة** **لإيقاف التشغيل**.</span><span class="sxs-lookup"><span data-stu-id="a8e71-108">Search for user and change the Calling Policy to one that has **Busy on Busy is available when in a call** to **Off**.</span></span>
1. <span data-ttu-id="a8e71-109">انقر فوق **تطبيق**.</span><span class="sxs-lookup"><span data-stu-id="a8e71-109">Click **Apply**.</span></span>
> [!NOTE]
> <span data-ttu-id="a8e71-110">قد تستغرق التغييرات في النهج ما يصل إلى 24 ساعة للنسخ المتماثل.</span><span class="sxs-lookup"><span data-stu-id="a8e71-110">Changes to policies can take up to 24 hours to replicate.</span></span>

<span data-ttu-id="a8e71-111">للحصول علي مزيد من المعلومات حول هذه الميزة ، يمكنك الاشاره إلى: [مشغول علي مشغول متوفر اثناء اجراء مكالمة](https://docs.microsoft.com/microsoftteams/teams-calling-policy#busy-on-busy-is-available-while-in-a-call).</span><span class="sxs-lookup"><span data-stu-id="a8e71-111">For more information on this feature refer to: [Busy on Busy is available while in a call](https://docs.microsoft.com/microsoftteams/teams-calling-policy#busy-on-busy-is-available-while-in-a-call).</span></span>
