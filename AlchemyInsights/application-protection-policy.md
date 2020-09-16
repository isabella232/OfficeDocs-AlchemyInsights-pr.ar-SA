---
title: نهج حماية التطبيقات
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/22/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1073"
- "6700006"
ms.openlocfilehash: 929400dcf0ca18ce8f52cb11e5c907064449480e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47716880"
---
# <a name="application-protection-policy"></a><span data-ttu-id="8686b-102">نهج حماية التطبيقات</span><span class="sxs-lookup"><span data-stu-id="8686b-102">Application protection policy</span></span>

<span data-ttu-id="8686b-103">إذا كنت جديدا في نهج حماية التطبيقات (التطبيق) ، فراجع [نظره عامه حول نهج حماية التطبيق](https://docs.microsoft.com/intune/apps/app-protection-policy).</span><span class="sxs-lookup"><span data-stu-id="8686b-103">If you're new to Application protection policy (APP), check out the [App protection policies overview](https://docs.microsoft.com/intune/apps/app-protection-policy).</span></span>

<span data-ttu-id="8686b-104">لبدء استخدام التطبيق ، راجع [كيفيه إنشاء نهج حماية التطبيق وتعيينها](https://docs.microsoft.com/intune/app-protection-policies).</span><span class="sxs-lookup"><span data-stu-id="8686b-104">To start using APP, see [How to create and assign app protection policies](https://docs.microsoft.com/intune/app-protection-policies).</span></span>

<span data-ttu-id="8686b-105">متطلبات نهج حماية التطبيق:</span><span class="sxs-lookup"><span data-stu-id="8686b-105">Application protection policy requirements:</span></span>

- <span data-ttu-id="8686b-106">يملك المستخدم ترخيص Intune أو EMS.</span><span class="sxs-lookup"><span data-stu-id="8686b-106">User has an Intune or EMS license.</span></span>
- <span data-ttu-id="8686b-107">ينتمي المستخدم إلى مجموعه مستهدفه بواسطة نهج حماية التطبيق.</span><span class="sxs-lookup"><span data-stu-id="8686b-107">User belongs to a group targeted by application protection policies.</span></span>
- <span data-ttu-id="8686b-108">يتم تسجيل دخول مستخدم واحد فقط للشركات إلى تطبيقات محمية علي جهاز.</span><span class="sxs-lookup"><span data-stu-id="8686b-108">Only one corporate user is signed into protected apps on a device.</span></span>
- <span data-ttu-id="8686b-109">قام التطبيق بتنفيذ [INTUNE SDK](https://docs.microsoft.com/intune/app-sdk-get-started).</span><span class="sxs-lookup"><span data-stu-id="8686b-109">The application has implemented the [Intune SDK](https://docs.microsoft.com/intune/app-sdk-get-started).</span></span> <span data-ttu-id="8686b-110">للحصول علي قائمه بالتطبيقات التي تدعم SDK ، راجع [التطبيقات المحمية في Microsoft Intune](https://docs.microsoft.com/intune/apps-supported-intune-apps).</span><span class="sxs-lookup"><span data-stu-id="8686b-110">For a list of apps that support the SDK, see [Microsoft Intune protected apps](https://docs.microsoft.com/intune/apps-supported-intune-apps).</span></span>

<span data-ttu-id="8686b-111">يتم تطبيق النهج بعد قيام المستخدم الذي يلبي المتطلبات أعلاه بتسجيل الدخول إلى تطبيق تم تمكينه في Intune SDK.</span><span class="sxs-lookup"><span data-stu-id="8686b-111">Policies apply after a user who meets the above requirements signs into an Intune SDK enabled app.</span></span> <span data-ttu-id="8686b-112">تتمثل أسهل طريقه لتحديد ما إذا كان النهج مطبقا بالطلب ان يقوم المستخدم بتعيين رقم pin في النهج.</span><span class="sxs-lookup"><span data-stu-id="8686b-112">The easiest way to determine if a policy is applied is by requiring that the user set a pin in the policy.</span></span> 

<span data-ttu-id="8686b-113">لمزيد من المعلومات، اطلع على:</span><span class="sxs-lookup"><span data-stu-id="8686b-113">For more information, see:</span></span>

[<span data-ttu-id="8686b-114">الاسئله المتداولة حول التطبيق/الMAM</span><span class="sxs-lookup"><span data-stu-id="8686b-114">APP/MAM troubleshooting FAQ</span></span>](https://docs.microsoft.com/intune/apps/troubleshoot-mam)  

[<span data-ttu-id="8686b-115">كيفيه التحقق من صحة اعداد نهج حماية التطبيق</span><span class="sxs-lookup"><span data-stu-id="8686b-115">How to validate your app protection policy setup</span></span>](https://docs.microsoft.com/intune/app-protection-policies-validate)

[<span data-ttu-id="8686b-116">فهم توقيت تسليم نهج حماية التطبيق</span><span class="sxs-lookup"><span data-stu-id="8686b-116">Understand App Protection Policy delivery timing</span></span>](https://docs.microsoft.com/intune/app-protection-policy-delivery)  

[<span data-ttu-id="8686b-117">كيفيه مراقبه نهج حماية التطبيق</span><span class="sxs-lookup"><span data-stu-id="8686b-117">How to monitor app protection policies</span></span>](https://docs.microsoft.com/intune/app-protection-policies-monitor)