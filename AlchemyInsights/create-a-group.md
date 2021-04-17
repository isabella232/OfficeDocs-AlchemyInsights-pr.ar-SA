---
title: إنشاء مجموعة
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
- "9003234"
- "7230"
ms.openlocfilehash: ec74b7c098d302d3bdeb5a412fad41efe7b82b98
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816331"
---
# <a name="create-a-group"></a><span data-ttu-id="bde07-102">إنشاء مجموعة</span><span class="sxs-lookup"><span data-stu-id="bde07-102">Create a group</span></span>

<span data-ttu-id="bde07-103">يصف هذا الموضوع إنشاء المجموعة.</span><span class="sxs-lookup"><span data-stu-id="bde07-103">This topic describes group creation.</span></span>

<span data-ttu-id="bde07-104">**الإذن لإنشاء مجموعة**</span><span class="sxs-lookup"><span data-stu-id="bde07-104">**Permission to Create a Group**</span></span>

<span data-ttu-id="bde07-105">تأكد من أنك م مخولا لإنشاء مجموعة جديدة.</span><span class="sxs-lookup"><span data-stu-id="bde07-105">Ensure you are authorized to create a new group.</span></span> <span data-ttu-id="bde07-106">يمكن للمسؤولين العامين تعطيل إنشاء المجموعة في مدخل Azure أو لوحة Access.</span><span class="sxs-lookup"><span data-stu-id="bde07-106">Global administrators can disable group creation in the Azure portal or Access Panel.</span></span> <span data-ttu-id="bde07-107">قد تحتاج إلى مسؤول لإنشاء المجموعة الجديدة لك، أو من أجل من يعطيك الأذونات المناسبة.</span><span class="sxs-lookup"><span data-stu-id="bde07-107">You may need an administrator to create the new group for you, or to give you appropriate permissions.</span></span>

<span data-ttu-id="bde07-108">**إدارة أذونات إنشاء المجموعة**</span><span class="sxs-lookup"><span data-stu-id="bde07-108">**Manage Group creation permissions**</span></span>

1. <span data-ttu-id="bde07-109">يمكن للمسؤولين العامين إدارة أذونات إنشاء المجموعات (لأسباب متعلقة والأمان) أو مجموعات Office 365 التي تم إنشاؤها في مدخل Azure أو لوحة Access، باختيار "يمكن للمستخدمين إنشاء مجموعات أمان في مداخل Azure" أو خيارات "يمكن للمستخدمين إنشاء مجموعات Office 365 في مداخل Azure" في كافة المجموعات عام  >  **(إعدادات)**.</span><span class="sxs-lookup"><span data-stu-id="bde07-109">Global administrators can manage group creation permissions (for security-related reasons) or Office 365 groups created in the Azure portal or Access Panel, by choosing "Users can create security groups in Azure portals" or "Users can create Office 365 groups in Azure portals" options in **All groups** > **General (Settings)**.</span></span>
2. <span data-ttu-id="bde07-110">يمكنك أيضا تقييد إنشاء المجموعة لتحديد مجموعة من المستخدمين إذا كان لديك ترخيص Azure Active Directory P1 Premium.</span><span class="sxs-lookup"><span data-stu-id="bde07-110">You can also restrict group creation to select a group of users if you have an Azure Active Directory P1 Premium license.</span></span>

<span data-ttu-id="bde07-111">**تعطيل إعلام الترحيب لأعضاء مجموعة Office 365 الجدد**</span><span class="sxs-lookup"><span data-stu-id="bde07-111">**Disabling welcome notification for new Office 365 group members**</span></span>

<span data-ttu-id="bde07-112">يمكن تعطيل إعلام الترحيب الذي يتم إرساله إلى المستخدمين الذين تم إضافتهم إلى مجموعات Office 365 عن طريق تعيين **UnifiedGroupWelcomeMessageEnabled** إلى False في Powershell.</span><span class="sxs-lookup"><span data-stu-id="bde07-112">The welcome notification sent to users who are added to Office 365 groups can be disabled by setting **UnifiedGroupWelcomeMessageEnabled** to False in Powershell.</span></span> <span data-ttu-id="bde07-113">تعرف على هذا الإعداد [هنا](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="bde07-113">Learn about this setting [here](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).</span></span>

