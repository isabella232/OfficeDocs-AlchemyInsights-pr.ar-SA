---
title: تأجيل ترقية Teams
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2737"
- "4000006"
ms.openlocfilehash: abbf696b1554743bda188704272bfd85fe6f94e2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51801218"
---
# <a name="how-to-postpone-the-microsoft-driven-teams-upgrade"></a><span data-ttu-id="23025-102">كيفية تأجيل ترقية Teams التي تعمل ب Microsoft</span><span class="sxs-lookup"><span data-stu-id="23025-102">How to postpone the Microsoft-driven Teams upgrade</span></span>

<span data-ttu-id="23025-103">**هام:** يمكننا مساعدتك في إصلاح هذا الأمر باستخدام تشخيص الدعم، ولكن يبدو أنك لا تستخدم "مركز الإدارة الجديد".</span><span class="sxs-lookup"><span data-stu-id="23025-103">**Important**: We can help fix this for you using a support diagnostic, but it looks like you are not using the New Admin Center.</span></span> <span data-ttu-id="23025-104">لاستخدام "مركز الإدارة الجديد"، مرر تبديل في الجزء العلوي الأيمن الذي يقول **مركز إدارة جديد** إلى اليمين.</span><span class="sxs-lookup"><span data-stu-id="23025-104">To use the New Admin Center, slide the toggle in the top right that says **new admin center** to the right.</span></span> <span data-ttu-id="23025-105">باستخدام مركز الإدارة الجديد، انقر فوق عنصر واجهة مستخدم هل تحتاج إلى **مساعدة؟،** وا اكتب "تأجيل ترقية Teams"، ثم اتبع المطالبات لتشغيل التشخيص.</span><span class="sxs-lookup"><span data-stu-id="23025-105">Using the New Admin Center, click the **Need Help?** widget, type "Postpone Teams Upgrade", then follow the prompts to run the diagnostic.</span></span>

<span data-ttu-id="23025-106">إذا تلقيت اتصالا حول ترقية تلقائية مدفوعة من Microsoft من Skype for Business إلى Microsoft Teams، وترغب في تأجيل الترقية التلقائية إلى تاريخ  لاحق، يمكن للمسؤول العام تسجيل  الدخول إلى مدخل مسؤول [Teams،](https://admin.teams.microsoft.com/dashboard) وبعد تحديد الزر تحديث الحالة ضمن ترقية Microsoft Teams، حدد الزر تأجيل.</span><span class="sxs-lookup"><span data-stu-id="23025-106">If you received communication about a Microsoft-driven automated upgrade from Skype for Business to Microsoft Teams, and you wish to postpone the automated upgrade to a later date, your Global Admin can log in to the [Teams Admin portal](https://admin.teams.microsoft.com/dashboard) and, after selecting the **Refresh Status** button under Microsoft Teams Upgrade, select the **Postpone** button.</span></span> <span data-ttu-id="23025-107">لمشاهدة التاريخ الجديد للترقية التلقائية للمستأجر إلى Microsoft Teams، قم بتحديث صفحة مدخل مسؤول الفرق.</span><span class="sxs-lookup"><span data-stu-id="23025-107">To see the new date for your tenant's automated upgrade to Microsoft Teams, refresh the Teams Admin portal page.</span></span>

<span data-ttu-id="23025-108">**ملاحظة:** لن **يتوفر الزر** تأجيل إلا إذا تلقيت إعلام مركز الرسائل بشأن الترقية التلقائية.</span><span class="sxs-lookup"><span data-stu-id="23025-108">**Note:** The **Postpone** button will only be available if you have received the message center notification regarding the automated upgrade.</span></span> 

<span data-ttu-id="23025-109">يمكن للمسؤولين العامين أيضا تشغيل [Get-CsTeamsUpgradeStatus](https://docs.microsoft.com/powershell/module/skype/get-csteamsupgradestatus?view=skype-ps) لمعرفة المزيد حول حالة الترقية الحالية.</span><span class="sxs-lookup"><span data-stu-id="23025-109">Global Admins can also run [Get-CsTeamsUpgradeStatus](https://docs.microsoft.com/powershell/module/skype/get-csteamsupgradestatus?view=skype-ps) to learn more about their current upgrade status.</span></span>
