---
title: سياسة حماية التطبيقات
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/22/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1073"
- "6700006"
ms.openlocfilehash: 7fed65e6749f72e6264070b360a52e72968fc8da
ms.sourcegitcommit: 6f7cbf1dc28c0693009ddf03d9768c1c65018964
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 07/22/2020
ms.locfileid: "45423265"
---
# <a name="application-protection-policy"></a><span data-ttu-id="e16d8-102">سياسة حماية التطبيقات</span><span class="sxs-lookup"><span data-stu-id="e16d8-102">Application protection policy</span></span>

<span data-ttu-id="e16d8-103">إذا كنت حديث العهد بسياسة حماية التطبيقات (APP)، فراجع [نظرة عامة على سياسات حماية التطبيقات](https://docs.microsoft.com/intune/apps/app-protection-policy).</span><span class="sxs-lookup"><span data-stu-id="e16d8-103">If you're new to Application protection policy (APP), check out the [App protection policies overview](https://docs.microsoft.com/intune/apps/app-protection-policy).</span></span>

<span data-ttu-id="e16d8-104">لبدء استخدام APP، راجع [كيفية إنشاء سياسات حماية التطبيق وتعيينها](https://docs.microsoft.com/intune/app-protection-policies).</span><span class="sxs-lookup"><span data-stu-id="e16d8-104">To start using APP, see [How to create and assign app protection policies](https://docs.microsoft.com/intune/app-protection-policies).</span></span>

<span data-ttu-id="e16d8-105">متطلبات سياسة حماية التطبيقات:</span><span class="sxs-lookup"><span data-stu-id="e16d8-105">Application protection policy requirements:</span></span>

- <span data-ttu-id="e16d8-106">المستخدم لديه ترخيص إينتوني أو EMS.</span><span class="sxs-lookup"><span data-stu-id="e16d8-106">User has an Intune or EMS license.</span></span>
- <span data-ttu-id="e16d8-107">ينتمي المستخدم إلى مجموعة مستهدفة من قبل نُهج حماية التطبيقات.</span><span class="sxs-lookup"><span data-stu-id="e16d8-107">User belongs to a group targeted by application protection policies.</span></span>
- <span data-ttu-id="e16d8-108">يتم تسجيل دخول مستخدم واحد فقط إلى تطبيقات محمية على جهاز.</span><span class="sxs-lookup"><span data-stu-id="e16d8-108">Only one corporate user is signed into protected apps on a device.</span></span>
- <span data-ttu-id="e16d8-109">التطبيق قد قام بتطبيق [SDK Intune](https://docs.microsoft.com/intune/app-sdk-get-started).</span><span class="sxs-lookup"><span data-stu-id="e16d8-109">The application has implemented the [Intune SDK](https://docs.microsoft.com/intune/app-sdk-get-started).</span></span> <span data-ttu-id="e16d8-110">للحصول على قائمة بالتطبيقات التي تدعم SDK، راجع [تطبيقات Microsoft Intune المحمية](https://docs.microsoft.com/intune/apps-supported-intune-apps).</span><span class="sxs-lookup"><span data-stu-id="e16d8-110">For a list of apps that support the SDK, see [Microsoft Intune protected apps](https://docs.microsoft.com/intune/apps-supported-intune-apps).</span></span>

<span data-ttu-id="e16d8-111">يتم تطبيق السياسات بعد أن يقوم المستخدم الذي يستوفي علامات المتطلبات المذكورة أعلاه في تطبيق تمكين Intune SDK.</span><span class="sxs-lookup"><span data-stu-id="e16d8-111">Policies apply after a user who meets the above requirements signs into an Intune SDK enabled app.</span></span> <span data-ttu-id="e16d8-112">أسهل طريقة لتحديد ما إذا كان يتم تطبيق نهج هو عن طريق مطالبة المستخدم بتعيين دبوس في النهج.</span><span class="sxs-lookup"><span data-stu-id="e16d8-112">The easiest way to determine if a policy is applied is by requiring that the user set a pin in the policy.</span></span> 

<span data-ttu-id="e16d8-113">لمزيد من المعلومات، اطلع على:</span><span class="sxs-lookup"><span data-stu-id="e16d8-113">For more information, see:</span></span>

[<span data-ttu-id="e16d8-114">الأسئلة الشائعة حول استكشاف أخطاء APP/MAM</span><span class="sxs-lookup"><span data-stu-id="e16d8-114">APP/MAM troubleshooting FAQ</span></span>](https://docs.microsoft.com/intune/apps/troubleshoot-mam)  

[<span data-ttu-id="e16d8-115">كيفية التحقق من صحة إعداد سياسة حماية التطبيق</span><span class="sxs-lookup"><span data-stu-id="e16d8-115">How to validate your app protection policy setup</span></span>](https://docs.microsoft.com/intune/app-protection-policies-validate)

[<span data-ttu-id="e16d8-116">فهم توقيت تسليم سياسة حماية التطبيقات</span><span class="sxs-lookup"><span data-stu-id="e16d8-116">Understand App Protection Policy delivery timing</span></span>](https://docs.microsoft.com/intune/app-protection-policy-delivery)  

[<span data-ttu-id="e16d8-117">كيفية مراقبة سياسات حماية التطبيقات</span><span class="sxs-lookup"><span data-stu-id="e16d8-117">How to monitor app protection policies</span></span>](https://docs.microsoft.com/intune/app-protection-policies-monitor)