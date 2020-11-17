---
title: إنشاء مجموعه
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
- "9003234"
- "7230"
ms.openlocfilehash: b8cb3f1de991bfe7197607d5e8964a018e31c122
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 11/17/2020
ms.locfileid: "49088487"
---
# <a name="create-a-group"></a><span data-ttu-id="e6ec5-102">إنشاء مجموعه</span><span class="sxs-lookup"><span data-stu-id="e6ec5-102">Create a group</span></span>

<span data-ttu-id="e6ec5-103">يصف هذا الموضوع إنشاء المجموعة.</span><span class="sxs-lookup"><span data-stu-id="e6ec5-103">This topic describes group creation.</span></span>

<span data-ttu-id="e6ec5-104">**اذن إنشاء مجموعه**</span><span class="sxs-lookup"><span data-stu-id="e6ec5-104">**Permission to Create a Group**</span></span>

<span data-ttu-id="e6ec5-105">تاكد من انك مصرحت لك بإنشاء مجموعه جديده.</span><span class="sxs-lookup"><span data-stu-id="e6ec5-105">Ensure you are authorized to create a new group.</span></span> <span data-ttu-id="e6ec5-106">يمكن للمسؤولين العموميين تعطيل إنشاء المجموعة في مدخل Azure أو لوحه الوصول.</span><span class="sxs-lookup"><span data-stu-id="e6ec5-106">Global administrators can disable group creation in the Azure portal or Access Panel.</span></span> <span data-ttu-id="e6ec5-107">قد تحتاج إلى مسؤول لإنشاء المجموعة الجديدة لك ، أو لمنحك الأذونات المناسبة.</span><span class="sxs-lookup"><span data-stu-id="e6ec5-107">You may need an administrator to create the new group for you, or to give you appropriate permissions.</span></span>

<span data-ttu-id="e6ec5-108">**أداره أذونات إنشاء المجموعة**</span><span class="sxs-lookup"><span data-stu-id="e6ec5-108">**Manage Group creation permissions**</span></span>

1. <span data-ttu-id="e6ec5-109">بإمكان المسؤولين العموميين أداره أذونات إنشاء المجموعة (لأسباب تتعلق بالأمان) أو مجموعات Office 365 التي تم إنشاؤها في مدخل azure أو لوحه الوصول ، عن طريق اختيار "يمكن للمستخدمين إنشاء مجموعات الأمان في azure مداخل" أو "يمكن للمستخدمين إنشاء مجموعات من office **365 في azure** portal  >  **General (Settings)**.</span><span class="sxs-lookup"><span data-stu-id="e6ec5-109">Global administrators can manage group creation permissions (for security-related reasons) or Office 365 groups created in the Azure portal or Access Panel, by choosing "Users can create security groups in Azure portals" or "Users can create Office 365 groups in Azure portals" options in **All groups** > **General (Settings)**.</span></span>
2. <span data-ttu-id="e6ec5-110">يمكنك أيضا تقييد إنشاء المجموعة لتحديد مجموعه من المستخدمين إذا كان لديك ترخيص Azure Active directory P1.</span><span class="sxs-lookup"><span data-stu-id="e6ec5-110">You can also restrict group creation to select a group of users if you have an Azure Active Directory P1 Premium license.</span></span>

<span data-ttu-id="e6ec5-111">**تعطيل الاعلامات الخاصة بأعضاء مجموعه Office 365 الجديدة**</span><span class="sxs-lookup"><span data-stu-id="e6ec5-111">**Disabling welcome notification for new Office 365 group members**</span></span>

<span data-ttu-id="e6ec5-112">يمكن تعطيل الاعلام بالترحيب المرسل إلى المستخدمين الذين تمت اضافتهم إلى مجموعات Office 365 عن طريق اعداد **أونيفيدجروبويلكوميميساجينابليد** to False في Powershell.</span><span class="sxs-lookup"><span data-stu-id="e6ec5-112">The welcome notification sent to users who are added to Office 365 groups can be disabled by setting **UnifiedGroupWelcomeMessageEnabled** to False in Powershell.</span></span> <span data-ttu-id="e6ec5-113">تعرف علي هذا الاعداد [هنا](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="e6ec5-113">Learn about this setting [here](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).</span></span>

