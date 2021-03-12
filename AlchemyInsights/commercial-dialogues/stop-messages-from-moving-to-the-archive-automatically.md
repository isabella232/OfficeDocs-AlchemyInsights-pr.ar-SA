---
title: إيقاف نقل الرسائل إلى الأرشيف تلقائيا
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100008"
- "7217"
ms.openlocfilehash: 2cb3e29dfd4f422e946b7887d4d44f373ff03794
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/11/2021
ms.locfileid: "50743141"
---
# <a name="stop-messages-from-moving-to-the-archive-automatically"></a><span data-ttu-id="1fdec-102">إيقاف نقل الرسائل إلى الأرشيف تلقائيا</span><span class="sxs-lookup"><span data-stu-id="1fdec-102">Stop messages from moving to the archive automatically</span></span>

<span data-ttu-id="1fdec-103">إذا كنت تستخدم نهج استبقاء، يمكنك تغيير عمر الاستبقاء في هذا النهج لمنع أرشفة الرسائل تلقائيا.</span><span class="sxs-lookup"><span data-stu-id="1fdec-103">If you are using a retention policy, you can change the retention age in that policy to stop messages from archiving automatically.</span></span> <span data-ttu-id="1fdec-104">إليك كيفية تنفيذ ذلك:</span><span class="sxs-lookup"><span data-stu-id="1fdec-104">Here's how:</span></span>

1. <span data-ttu-id="1fdec-105">في مركز [إدارة Exchange،](https://go.microsoft.com/fwlink/?linkid=2059104)اختر **علامات استبقاء إدارة**  >  **التوافق**.</span><span class="sxs-lookup"><span data-stu-id="1fdec-105">In the [Exchange admin center](https://go.microsoft.com/fwlink/?linkid=2059104), choose **compliance management** > **retention tags**.</span></span> <span data-ttu-id="1fdec-106">حدد موقع علامة الاستبقاء نقل إلى أرشفة.</span><span class="sxs-lookup"><span data-stu-id="1fdec-106">Locate your Move to Archive retention tag.</span></span>
2. <span data-ttu-id="1fdec-107">في علامة الاستبقاء، غير فترة الاستبقاء (فترة الأرشيف) إلى عدم إيقاف أرشفة العناصر تلقائيا بواسطة نهج استبقاء. </span><span class="sxs-lookup"><span data-stu-id="1fdec-107">In the retention tag, change the retention period (archive period) to **Never** to stop items from being automatically archived by a retention policy.</span></span>

> [!NOTE]
> <span data-ttu-id="1fdec-108">سيغير هذا إعداد الأرشيف لكل علب البريد مع تطبيق علامة الاستبقاء هذه عليها.</span><span class="sxs-lookup"><span data-stu-id="1fdec-108">This will change the archive setting for all mailboxes with this retention tag applied to them.</span></span>
