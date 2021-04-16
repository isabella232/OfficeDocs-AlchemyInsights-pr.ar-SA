---
title: رمز الطاقة أو البطارية مفقود في نظام التشغيل Windows 10
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002953"
- "5655"
ms.openlocfilehash: 95b68cee58f88d04f02e29477b139f7f583dc0b1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51790535"
---
# <a name="power-or-battery-icon-missing-in-windows-10"></a><span data-ttu-id="89ed5-102">رمز الطاقة أو البطارية مفقود في نظام التشغيل Windows 10</span><span class="sxs-lookup"><span data-stu-id="89ed5-102">Power or battery icon missing in Windows 10</span></span>

<span data-ttu-id="89ed5-103">إذا كان جهازك الذي يعمل بنظام التشغيل Windows 10 يحتوي على بطارية (على سبيل المثال، كمبيوتر محمول، أو كمبيوتر لوحي، أو كمبيوتر متصل عبر USB إلى UPS)، فعادة ما يظهر رمز الطاقة/البطارية في شريط المهام بالقرب من الساعة، على سبيل المثال:</span><span class="sxs-lookup"><span data-stu-id="89ed5-103">If your Windows 10 device has a battery (e.g., laptop or tablet, or a PC connected via USB to a UPS), normally a power/battery icon is shown in the taskbar near the clock, for example:</span></span>

![أيقونة البطارية](media/battery-icon.png)

<span data-ttu-id="89ed5-105">إذا كنت لا ترى هذا الرمز، فقد يكون مخفيًا:</span><span class="sxs-lookup"><span data-stu-id="89ed5-105">If you don't see this icon, it may be hidden:</span></span>

1. <span data-ttu-id="89ed5-106">انتقل إلى **[إعدادات > إضفاء الطابع الشخصي > شريط المهام](ms-settings:taskbar?activationSource=GetHelp)**.</span><span class="sxs-lookup"><span data-stu-id="89ed5-106">Go to **[Settings > Personalization > Taskbar](ms-settings:taskbar?activationSource=GetHelp)**.</span></span>

2. <span data-ttu-id="89ed5-107">في منطقة الإعلام، انقر فوق **تحديد الرموز التي تظهر على شريط المهام**.</span><span class="sxs-lookup"><span data-stu-id="89ed5-107">In the Notification area, click **Select which icons appear on the taskbar**.</span></span>

3. <span data-ttu-id="89ed5-108">ثم ابحث عن عنصر **الطاقة** في القائمة وقم بتبديل الإعداد إلى **تشغيل**.</span><span class="sxs-lookup"><span data-stu-id="89ed5-108">Then find the **Power** item in the list and toggle its setting to **On**.</span></span>

    ![إظهار أيقونه الطاقة في شريط المهام](media/power-icon-on.png)

<span data-ttu-id="89ed5-110">**استكشاف الأخطاء وإصلاحها**</span><span class="sxs-lookup"><span data-stu-id="89ed5-110">**Troubleshooting**</span></span>

<span data-ttu-id="89ed5-111">إذا اتبعت الإرشادات المذكورة أعلاه وكان مفتاح تبديل **الطاقة** معطلاً أو غير مرئي، في مربع البحث على شريط المهام، اكتب **مدير الجهاز**، ثم حدد **إدارة الأجهزة** في قائمة النتائج.</span><span class="sxs-lookup"><span data-stu-id="89ed5-111">If you followed the above instructions and the **Power** toggle is greyed out or not visible, in the search box on the taskbar, type **device manager**, and then select **Device Manager** in the list of results.</span></span> <span data-ttu-id="89ed5-112">ضمن **البطاريات**، انقر بزر الماوس الأيمن فوق بطارية جهازك، وانقر فوق **تعطيل**، ثم انقر فوق **نعم**.</span><span class="sxs-lookup"><span data-stu-id="89ed5-112">Under **Batteries**, right-click the battery for your device, click **Disable**, and click **Yes**.</span></span> <span data-ttu-id="89ed5-113">انتظر بضع ثوانٍ، ثم انقر بزر الماوس الأيمن فوق البطارية وانقر فوق **تمكين**.</span><span class="sxs-lookup"><span data-stu-id="89ed5-113">Wait a few seconds, and then right-click the battery and click **Enable**.</span></span> <span data-ttu-id="89ed5-114">ثم اعد تشغيل الجهاز.</span><span class="sxs-lookup"><span data-stu-id="89ed5-114">Then restart your device.</span></span>

<span data-ttu-id="89ed5-115">إذا اتبعت الإرشادات المذكورة أعلاه، ولكن رمز البطارية لا يظهر على شريط المهام، في مربع البحث على شريط المهام، اكتب **مدير المهام**، ثم انقر فوق **إدارة المهام** في قائمة النتائج.</span><span class="sxs-lookup"><span data-stu-id="89ed5-115">If you followed the above instructions, but the battery icon does not appear on the taskbar, in the search box on the taskbar, type **task manager**, and then click **Task Manager** in the list of results.</span></span> <span data-ttu-id="89ed5-116">على علامة التبويب **العمليات**، ضمن **اسم**، انقر بزر الماوس الأيمن فوق **Explorer**، ثم انقر فوق **إعادة تشغيل**.</span><span class="sxs-lookup"><span data-stu-id="89ed5-116">On the **Processes** tab, under **Name**, right-click **Explorer**, and then click **Restart**.</span></span>
