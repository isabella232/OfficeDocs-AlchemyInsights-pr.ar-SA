---
title: بدء استخدام أحداث Teams المباشرة
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000208"
- "3436"
ms.openlocfilehash: 979555a6fba46437adaf7e8c201cb9d6c4a8e965
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47677266"
---
# <a name="getting-started-with-teams-live-events"></a><span data-ttu-id="e245f-102">بدء استخدام أحداث Teams المباشرة</span><span class="sxs-lookup"><span data-stu-id="e245f-102">Getting started with Teams live events</span></span>

<span data-ttu-id="e245f-103">الأحداث المباشرة في Microsoft Teams هي ملحق اجتماعات Teams الذي يمكّنك من عقد أحداث تُنقل إلى مجموعة كبيرة من الحضور عبر الإنترنت وجدولتها.</span><span class="sxs-lookup"><span data-stu-id="e245f-103">Microsoft Teams live events are an extension of Teams meetings that enable you to schedule and produce events that stream to large online audiences.</span></span>

<span data-ttu-id="e245f-104">لعقد حدث مباشر، ستحتاج لما يلي:</span><span class="sxs-lookup"><span data-stu-id="e245f-104">To create a live event, you will need the following:</span></span>

- <span data-ttu-id="e245f-105">أولا ، تاكد من توفر احداث الفرق المباشرة [في بلدك وإقليمك](https://docs.microsoft.com/microsoftteams/teams-live-events/plan-for-teams-live-events#regional-availability)؛ لم يتم دعم الاحداث المباشرة بعد في بعض الدول.</span><span class="sxs-lookup"><span data-stu-id="e245f-105">First, confirm that Teams Live Events are [available in your Country and Region](https://docs.microsoft.com/microsoftteams/teams-live-events/plan-for-teams-live-events#regional-availability); Live Events are not yet supported in some countries.</span></span>  <span data-ttu-id="e245f-106">إذا قمت بتعيين تراخيص وتعيين نهج ، ولكن لا يزال يتعذر عليك إنشاء حدث فرق مباشر ، فمن المحتمل ان تكون في بلدك أو في منطقه حيث لا تتوفر الاحداث الحية بعد.</span><span class="sxs-lookup"><span data-stu-id="e245f-106">If you’ve assigned licenses and set policies, but still cannot create a Teams Live Event, it is likely you are in a Country or Region where Live Events is not yet available.</span></span>

- <span data-ttu-id="e245f-107">[ترخيص Office 365 Enterprise E1 أو E3 أو E5 أو Office 365 A3 أوA5](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#step-2-get-and-assign-licenses).</span><span class="sxs-lookup"><span data-stu-id="e245f-107">An [Office 365 Enterprise E1, E3, or E5 license or an Office 365 A3 or A5 license](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#step-2-get-and-assign-licenses).</span></span> <span data-ttu-id="e245f-108">**ملاحظة**: بسبب الزيادة الحالية في استخدام Teams، قد يستغرق تعيين ترخيص Teams إلى مستخدم حوالي 24 ساعة قبل أن يتم إعداده بشكل كامل.</span><span class="sxs-lookup"><span data-stu-id="e245f-108">**Note**: Due to a recent increase in Teams usage, when you assign a Teams license to a user, it may take around 24 hours before they'll be fully set up.</span></span> <span data-ttu-id="e245f-109">إلا أن يتم ذلك، لن تتمكن من تعيين نُهج Teams إليه وقد لا يتوفر له إمكانية الوصول إلى ميزات مثل إجراء مكالمات أو عقد مؤتمرات صوتية.</span><span class="sxs-lookup"><span data-stu-id="e245f-109">Until then, you won't be able to assign Teams policies to them, and they might not have access to some Teams features like calling and audio conferencing.</span></span>

- <span data-ttu-id="e245f-110">إذن [لعقد أحداث مباشرة في مركز إدارة Microsoft Teams](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#create-or-edit-a-live-events-policy).</span><span class="sxs-lookup"><span data-stu-id="e245f-110">Permission to [create live events in Microsoft Teams admin center](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#create-or-edit-a-live-events-policy).</span></span>

- <span data-ttu-id="e245f-111">إذن [لعقد أحداث مباشرة في Microsoft Stream](https://docs.microsoft.com/microsoftteams/teams-live-events/what-are-teams-live-events) (للأحداث التي يتم عقدها باستخدام تطبيق أو جهاز بث خارجي).</span><span class="sxs-lookup"><span data-stu-id="e245f-111">Permission to [create live events in Microsoft Stream](https://docs.microsoft.com/microsoftteams/teams-live-events/what-are-teams-live-events) (for events produced using an external broadcasting app or device).</span></span>

- <span data-ttu-id="e245f-112">عضوية فريق كاملة في المؤسسة (غير مسموح بعضوية ضيف أو مؤسسة أخرى).</span><span class="sxs-lookup"><span data-stu-id="e245f-112">Full team membership in the org (can't be a guest or from another org).</span></span>
<span data-ttu-id="e245f-113">تمكين جدولة اجتماع خاص ومشاركة الشاشة ومشاركة الفيديو عبر IP في نهج اجتماع Team.</span><span class="sxs-lookup"><span data-stu-id="e245f-113">Private meeting scheduling, screensharing, and IP video sharing, turned on in Team meeting policy.</span></span>

- <span data-ttu-id="e245f-114">[أفضل ممارسات](https://support.office.com/article/Best-practices-for-producing-a-Teams-live-event-e500370e-4dd1-4187-8b48-af10ef02cf42) أحداث Teams المباشرة.</span><span class="sxs-lookup"><span data-stu-id="e245f-114">[Best practices](https://support.office.com/article/Best-practices-for-producing-a-Teams-live-event-e500370e-4dd1-4187-8b48-af10ef02cf42) for Teams Live Events.</span></span>

<span data-ttu-id="e245f-115">للحصول على مزيد من المعلومات، الرجاء الاطلاع على [بدء استخدام أحداث Microsoft Teams المباشرة](https://support.office.com/article/get-started-with-microsoft-teams-live-events-d077fec2-a058-483e-9ab5-1494afda578a).</span><span class="sxs-lookup"><span data-stu-id="e245f-115">For more information, please see [Get started with Microsoft Teams live events](https://support.office.com/article/get-started-with-microsoft-teams-live-events-d077fec2-a058-483e-9ab5-1494afda578a).</span></span>