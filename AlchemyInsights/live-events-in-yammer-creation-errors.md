---
title: الأحداث المباشرة في أخطاء إنشاء Yammer
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002495"
- "5112"
ms.openlocfilehash: 35cddfee1a78fd6e1e502871bd5b56d786bf300a
ms.sourcegitcommit: fbaa2ce2cfb4d56d8c4cf2fa2d95489bdfcb7ff0
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/30/2020
ms.locfileid: "43947762"
---
# <a name="live-events-in-yammer-creation-errors"></a><span data-ttu-id="5dea2-102">الأحداث المباشرة في أخطاء إنشاء Yammer</span><span class="sxs-lookup"><span data-stu-id="5dea2-102">Live events in Yammer creation errors</span></span>

<span data-ttu-id="5dea2-103">**إنشاء حدث Yammer Live**</span><span class="sxs-lookup"><span data-stu-id="5dea2-103">**Yammer Live Event creation**</span></span>

<span data-ttu-id="5dea2-104">سيعرض Yammer خيار إنشاء حدث مباشر في كل الأوقات.</span><span class="sxs-lookup"><span data-stu-id="5dea2-104">Yammer will show the option to create a live event at all times.</span></span> <span data-ttu-id="5dea2-105">في بعض الحالات، قد لا يفي المستخدم بالمتطلبات الأساسية لإنشاء حدث مباشر وتتلقي رسالة خطا عند محاولة إنشائه.</span><span class="sxs-lookup"><span data-stu-id="5dea2-105">In some cases, a user may not meet the prerequisites for creating a live event and receive an error when they attempt to create it.</span></span> <span data-ttu-id="5dea2-106">تغطي العناصر أدناه الأسباب الشائعة لهذه المشكلة وتوفر طرقًا لحلها للمستخدمين النهائيين.</span><span class="sxs-lookup"><span data-stu-id="5dea2-106">The items below cover common reasons for this problem and provide ways to resolve it for end users.</span></span>

<span data-ttu-id="5dea2-107">**الأشخاص الذين يمكنهم إنشاء أحداث مباشرة**</span><span class="sxs-lookup"><span data-stu-id="5dea2-107">**Who can create live events**</span></span>
- <span data-ttu-id="5dea2-108">ترخيص Office 365 Enterprise E1 أو E3 أو E5 أو Office 365 A3 أوA5.</span><span class="sxs-lookup"><span data-stu-id="5dea2-108">An Office 365 Enterprise E1, E3, or E5 license or an Office 365 A3 or A5 license.</span></span>
- <span data-ttu-id="5dea2-109">إذن إنشاء أحداث مباشرة في مركز إدارة Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="5dea2-109">Permission to create live events in Microsoft Teams admin center.</span></span>
- <span data-ttu-id="5dea2-110">إذن إنشاء أحداث مباشرة في Microsoft Stream (للأحداث التي يتم إنشاؤها باستخدام تطبيق أو جهاز بث خارجي).</span><span class="sxs-lookup"><span data-stu-id="5dea2-110">Permission to create live events in Microsoft Stream (for events produced using an external broadcasting app or device).</span></span>
- <span data-ttu-id="5dea2-111">عضوية فريق كاملة في المؤسسة (لا يمكن أن يكون ضيفاً أو من مؤسسة أخرى).</span><span class="sxs-lookup"><span data-stu-id="5dea2-111">Full team membership in the org (can’t be a guest or from another org).</span></span>
- <span data-ttu-id="5dea2-112">تمكين جدولة اجتماع خاص ومشاركة الشاشة ومشاركة الفيديو عبر IP في نهج اجتماع Team.</span><span class="sxs-lookup"><span data-stu-id="5dea2-112">Private meeting scheduling, screensharing, and IP video sharing, turned on in Team meeting policy.</span></span>

<span data-ttu-id="5dea2-113">**نهج إنشاء الأحداث المباشرة**</span><span class="sxs-lookup"><span data-stu-id="5dea2-113">**Live event creation policies**</span></span>

<span data-ttu-id="5dea2-114">يتبع Yammer سياسات الأحداث المباشرة المحددة في مستأجر Office 365 الخاص بـ Stream.</span><span class="sxs-lookup"><span data-stu-id="5dea2-114">Yammer follows the Live Event policies set in your Office 365 tenant for Stream.</span></span> <span data-ttu-id="5dea2-115">بشكل افتراضي، يمكن لكل شخص في مؤسستك إنشاء الأحداث المباشرة.</span><span class="sxs-lookup"><span data-stu-id="5dea2-115">By default, everyone in your organization can create a live event.</span></span> <span data-ttu-id="5dea2-116">يمكن للمسؤولين [إجراء تغييرات علي هذا الإعداد مما قد يمنع المستخدمين من إنشاء حدث مباشر](https://docs.microsoft.com/stream/live-event-administration#enabling-and-restricting-users-to-creating).</span><span class="sxs-lookup"><span data-stu-id="5dea2-116">Administrators may [make changes to this setting which may prevent users from creating a live event](https://docs.microsoft.com/stream/live-event-administration#enabling-and-restricting-users-to-creating).</span></span> <span data-ttu-id="5dea2-117">من المهم التحقق من أن المستخدمين لديهم أذونات لإنشاء إحداث مباشره إذا تلقيت رسالة خطا في النهج.</span><span class="sxs-lookup"><span data-stu-id="5dea2-117">It is important to check that users have permissions to create live events if they receive a policy error.</span></span>
