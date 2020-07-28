---
title: حذف قناة خاصة للفرق
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3781"
- "9001223"
ms.openlocfilehash: 2ee998f0c70973645c273a2a6609af2420a4f74b
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 07/28/2020
ms.locfileid: "45438691"
---
# <a name="delete-a-teams-private-channel"></a><span data-ttu-id="a4b5e-102">حذف قناة خاصة للفرق</span><span class="sxs-lookup"><span data-stu-id="a4b5e-102">Delete a Teams private channel</span></span>

<span data-ttu-id="a4b5e-103">Microsoft على علم مشكلة حذف قناة خاصة الفرق إذا كان لديك نهج الاحتفاظ SharePoint تمكين موقع SharePoint.</span><span class="sxs-lookup"><span data-stu-id="a4b5e-103">Microsoft is aware of an issue deleting a Teams private channel if you have SharePoint Retention Policies enabled for the underlying SharePoint site.</span></span> <span data-ttu-id="a4b5e-104">تعمل Microsoft على إصلاح.</span><span class="sxs-lookup"><span data-stu-id="a4b5e-104">Microsoft is working on a fix.</span></span> <span data-ttu-id="a4b5e-105">في غضون ذلك، يمكنك استخدام الحلول التالية لحذف القناة الخاصة.</span><span class="sxs-lookup"><span data-stu-id="a4b5e-105">In the meantime, you can use the following workarounds to delete the private channel.</span></span>

<span data-ttu-id="a4b5e-106">**استبعاد مجموعة الفريق/الموقع من نهج الاحتفاظ Sharepoint.**</span><span class="sxs-lookup"><span data-stu-id="a4b5e-106">**Exclude the Team/site collection from the Sharepoint retention policy.**</span></span>

1. <span data-ttu-id="a4b5e-107">انتقل إلى مدخل مسؤول Office 365، وحدد **إظهار الكل** في جزء التنقل الأيمن.</span><span class="sxs-lookup"><span data-stu-id="a4b5e-107">Go to the Office 365 admin portal, and select **Show all** in the left navigation pane.</span></span>
2. <span data-ttu-id="a4b5e-108">تحت **مراكز الإدارة**، انتقل إلى سياسة منع فقدان البيانات & التوافق **مع**  >  **Data Loss Prevention**  >  **الأمان.**</span><span class="sxs-lookup"><span data-stu-id="a4b5e-108">Under **Admin centers**, go to **Security & Compliance** > **Data Loss Prevention** > **Policy**.</span></span>
3. <span data-ttu-id="a4b5e-109">تحديد أي نهج ينطبق على مواقع Sharepoint، وتعديل النهج بحيث موقع Sharepoint للفريق الذي يحتوي على قناة خاصة غير مضمن ضمن نهج الاستبقاء.</span><span class="sxs-lookup"><span data-stu-id="a4b5e-109">Identify any policy that applies to Sharepoint sites, and modify the policy so the Sharepoint site for the Team containing the private channel is NOT included under the retention policy.</span></span>
4. <span data-ttu-id="a4b5e-110">حفظ النهج.</span><span class="sxs-lookup"><span data-stu-id="a4b5e-110">Save the policy.</span></span>
    <span data-ttu-id="a4b5e-111">قد يستغرق الأمر ما يصل إلى 24 ساعة حتى يتم تنفيذ إعدادات النهج.</span><span class="sxs-lookup"><span data-stu-id="a4b5e-111">It can take up to 24 hours for policy settings to take effect.</span></span>
    <span data-ttu-id="a4b5e-112">بعد استبعاد الموقع، يمكنك حذف القناة الخاصة.</span><span class="sxs-lookup"><span data-stu-id="a4b5e-112">After the site has been excluded, you can delete the private channel.</span></span>  
    
<span data-ttu-id="a4b5e-113">***قد*** تتمكن من حذف القناة الخاصة باستخدام Microsoft Teams على جهاز Android.</span><span class="sxs-lookup"><span data-stu-id="a4b5e-113">You  ***might*** be able to delete the private channel by using Microsoft Teams on your Android device.</span></span> 

<span data-ttu-id="a4b5e-114">للحصول على معلومات SharePoint ذات الصلة، راجع [غير قادر على حذف العناصر في SharePoint Online أو أندريف للعمل](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold).</span><span class="sxs-lookup"><span data-stu-id="a4b5e-114">For related SharePoint information, see [Unable to delete items in SharePoint Online or OneDrive for Business](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold).</span></span>