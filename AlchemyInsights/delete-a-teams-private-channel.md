---
title: حذف القناة الخاصة بالفرق
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3781"
- "9001223"
ms.openlocfilehash: 56021a335c64810700913cf08519b95f24a7a17d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47730902"
---
# <a name="delete-a-teams-private-channel"></a><span data-ttu-id="4b754-102">حذف القناة الخاصة بالفرق</span><span class="sxs-lookup"><span data-stu-id="4b754-102">Delete a Teams private channel</span></span>

<span data-ttu-id="4b754-103">ان Microsoft علي علم بوجود مشكله في حذف القناة الخاصة بفرق العمل الخاصة إذا كان لديك نهج استبقاء SharePoint ممكنة لموقع SharePoint الأساسي.</span><span class="sxs-lookup"><span data-stu-id="4b754-103">Microsoft is aware of an issue deleting a Teams private channel if you have SharePoint Retention Policies enabled for the underlying SharePoint site.</span></span> <span data-ttu-id="4b754-104">تعمل Microsoft علي تصحيح.</span><span class="sxs-lookup"><span data-stu-id="4b754-104">Microsoft is working on a fix.</span></span> <span data-ttu-id="4b754-105">في الوقت نفسه ، يمكنك استخدام الحلول البديلة التالية لحذف القناة الخاصة.</span><span class="sxs-lookup"><span data-stu-id="4b754-105">In the meantime, you can use the following workarounds to delete the private channel.</span></span>

<span data-ttu-id="4b754-106">**استبعاد الفريق/مجموعه المواقع المشتركة من نهج الاستبقاء في Sharepoint.**</span><span class="sxs-lookup"><span data-stu-id="4b754-106">**Exclude the Team/site collection from the Sharepoint retention policy.**</span></span>

1. <span data-ttu-id="4b754-107">انتقل إلى مدخل أداره Office 365 ، وحدد **إظهار الكل** في جزء التنقل الأيمن.</span><span class="sxs-lookup"><span data-stu-id="4b754-107">Go to the Office 365 admin portal, and select **Show all** in the left navigation pane.</span></span>
2. <span data-ttu-id="4b754-108">ضمن **مراكز الاداره**، انتقل إلى نهج تفادي فقدان بيانات **التوافق في & الأمان**  >  **Data Loss Prevention**  >  **Policy**.</span><span class="sxs-lookup"><span data-stu-id="4b754-108">Under **Admin centers**, go to **Security & Compliance** > **Data Loss Prevention** > **Policy**.</span></span>
3. <span data-ttu-id="4b754-109">حدد اي نهج ينطبق علي مواقع Sharepoint ، وقم بتعديل النهج بحيث لا يتم تضمين موقع Sharepoint للفريق الذي يحتوي علي القناة الخاصة ضمن نهج الاستبقاء.</span><span class="sxs-lookup"><span data-stu-id="4b754-109">Identify any policy that applies to Sharepoint sites, and modify the policy so the Sharepoint site for the Team containing the private channel is NOT included under the retention policy.</span></span>
4. <span data-ttu-id="4b754-110">احفظ النهج.</span><span class="sxs-lookup"><span data-stu-id="4b754-110">Save the policy.</span></span>
    <span data-ttu-id="4b754-111">قد يستغرق الأمر مده تصل إلى 24 ساعة لكي تدخل إعدادات النهج حيز التنفيذ.</span><span class="sxs-lookup"><span data-stu-id="4b754-111">It can take up to 24 hours for policy settings to take effect.</span></span>
    <span data-ttu-id="4b754-112">بعد استبعاد الموقع ، يمكنك حذف القناة الخاصة.</span><span class="sxs-lookup"><span data-stu-id="4b754-112">After the site has been excluded, you can delete the private channel.</span></span>  
    
<span data-ttu-id="4b754-113">***قد*** تتمكن من حذف القناة الخاصة باستخدام فرق Microsoft علي جهازك الذي يعمل بنظام Android.</span><span class="sxs-lookup"><span data-stu-id="4b754-113">You  ***might*** be able to delete the private channel by using Microsoft Teams on your Android device.</span></span> 

<span data-ttu-id="4b754-114">للحصول علي معلومات SharePoint ذات الصلة ، راجع [تعذر حذف العناصر في SharePoint Online أو OneDrive For business](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold).</span><span class="sxs-lookup"><span data-stu-id="4b754-114">For related SharePoint information, see [Unable to delete items in SharePoint Online or OneDrive for Business](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold).</span></span>