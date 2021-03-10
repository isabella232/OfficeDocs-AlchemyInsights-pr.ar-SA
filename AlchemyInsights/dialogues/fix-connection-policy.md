---
title: إصلاح نهج الاتصال
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
- "9000760"
- "7391"
ms.openlocfilehash: 0b6286350e706e493f6d30b7978aacedc02daff5
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/09/2021
ms.locfileid: "50692512"
---
# <a name="fix-connection-policy"></a><span data-ttu-id="8f770-102">إصلاح نهج الاتصال</span><span class="sxs-lookup"><span data-stu-id="8f770-102">Fix connection policy</span></span>

<span data-ttu-id="8f770-103">تم وضع علامة آمن على البريد الإلكتروني وتسليمه إلى علبة الوارد الخاصة للمستخدم لأنه تم وضع علامة آمن على عنوان IP المرسل في نهج تصفية الاتصال.</span><span class="sxs-lookup"><span data-stu-id="8f770-103">The email was marked safe and delivered to the user's inbox because the sending IP address was marked safe in the Connection Filter policy.</span></span> <span data-ttu-id="8f770-104">لمراجعة النهج، يمكنك القيام بما يلي:</span><span class="sxs-lookup"><span data-stu-id="8f770-104">To review the policy, do the following:</span></span>

1. <span data-ttu-id="8f770-105">انتقل إلى مركز التوافق & الأمان في [Office 365،](https://go.microsoft.com/fwlink/p/?linkid=2077143)ثم انتقل إلى نهج إدارة المخاطر   >    >  [لمكافحة البريد العشوائي.](https://go.microsoft.com/fwlink/?linkid=2101518)</span><span class="sxs-lookup"><span data-stu-id="8f770-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143), and then go to **Threat management** > **Policy** > [Anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).</span></span>
2. <span data-ttu-id="8f770-106">على علامة **التبويب "مخصص"،** حدد نهج **تصفية الاتصال،** ثم حدد **"تحرير النهج".**</span><span class="sxs-lookup"><span data-stu-id="8f770-106">On the **Custom** tab, select the **Connection filter policy**, and then select **Edit policy**.</span></span>
3. <span data-ttu-id="8f770-107">راجع قائمة **السماح ب IP.**</span><span class="sxs-lookup"><span data-stu-id="8f770-107">Review the **IP Allow** list.</span></span> <span data-ttu-id="8f770-108">معرفة ما **إذا كانت القائمة الآمنة** تم تمكينها.</span><span class="sxs-lookup"><span data-stu-id="8f770-108">See if **Safe list** is enabled.</span></span>

    > [!NOTE]
    > <span data-ttu-id="8f770-109">تشترك Microsoft في مصادر جهة خارجية للمرسلين الموثوق بهم.</span><span class="sxs-lookup"><span data-stu-id="8f770-109">Microsoft subscribes to third-party sources of trusted senders.</span></span> <span data-ttu-id="8f770-110">إذا **تم تمكين "القائمة** الآمنة"، لا يتم وضع علامة عن طريق الخطأ على هؤلاء المرسلين الموثوق بهم على أنها بريد عشوائي.</span><span class="sxs-lookup"><span data-stu-id="8f770-110">If **Safe list** is enabled, these trusted senders aren't mistakenly marked as spam.</span></span> <span data-ttu-id="8f770-111">من المستحسن تحديد هذا الخيار، لأنه سيقلل عدد الإيجابيات الخاطئة (البريد الجيد المصنف كبريد عشوائي) التي تتلقاها.</span><span class="sxs-lookup"><span data-stu-id="8f770-111">I recommend selecting this option, because it will reduce the number of false positives (good mail that's classified as spam) that you receive.</span></span>
