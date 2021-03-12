---
title: تمكين المجال المخصص ل DKIM
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: 1a21101602f47dcb5c9b607d7bbccfacec00f43a
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/11/2021
ms.locfileid: "50743094"
---
# <a name="enable-the-custom-domain-for-dkim"></a><span data-ttu-id="a3384-102">تمكين المجال المخصص ل DKIM</span><span class="sxs-lookup"><span data-stu-id="a3384-102">Enable the custom domain for DKIM</span></span>

<span data-ttu-id="a3384-103">بعد إنشاء سجلات CNAME للمجالات المخصصة، ستحتاج إلى تمكين المجال.</span><span class="sxs-lookup"><span data-stu-id="a3384-103">After you create the CNAME records for your custom domains, you need to enable the domain.</span></span>

<span data-ttu-id="a3384-104">لتمكين المجال، يمكنك تنفيذ الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="a3384-104">To enable the domain, perform the following steps:</span></span>

1. <span data-ttu-id="a3384-105">انتقل إلى [مركز إدارة Exchange](https://outlook.office365.com/ecp/).</span><span class="sxs-lookup"><span data-stu-id="a3384-105">Navigate to the [Exchange admin center](https://outlook.office365.com/ecp/).</span></span>
2. <span data-ttu-id="a3384-106">في الجزء الأيسر، حدد الحماية > **dkim**.</span><span class="sxs-lookup"><span data-stu-id="a3384-106">In the left pane, select **protection > dkim**.</span></span>
3. <span data-ttu-id="a3384-107">حدد المجال، ثم ضمن توقيع رسائل لهذا المجال **باستخدام تواقيع DKIM،** انقر فوق **تمكين**.</span><span class="sxs-lookup"><span data-stu-id="a3384-107">Select the domain, and then under **Sign messages for this domain with DKIM signatures**, click **Enable**.</span></span> <span data-ttu-id="a3384-108">كرر هذه الخطوة لكل مجال.</span><span class="sxs-lookup"><span data-stu-id="a3384-108">Repeat this step for each domain.</span></span>

