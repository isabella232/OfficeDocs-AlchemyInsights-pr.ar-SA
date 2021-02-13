---
title: نشر Microsoft Edge على iOS وiPadOS وAndroid
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/10/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8241"
- "9004604"
ms.openlocfilehash: 524e87ab57e29823361053093708c83831f19687
ms.sourcegitcommit: 03378c78eadac5d950802dcbacc328bca3314032
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/10/2021
ms.locfileid: "50194447"
---
# <a name="deploy-microsoft-edge-to-ios-ipados-and-android"></a><span data-ttu-id="275a6-102">نشر Microsoft Edge على iOS وiPadOS وAndroid</span><span class="sxs-lookup"><span data-stu-id="275a6-102">Deploy Microsoft Edge to iOS, iPadOS, and Android</span></span>

<span data-ttu-id="275a6-103">سيساعدك السيناريو الإرشادي الملخص أدناه في تعيين Microsoft Edge لمستخدمي أجهزة iOS وiPadOS وAndroid.</span><span class="sxs-lookup"><span data-stu-id="275a6-103">The guided scenario summarized below will help you assign Microsoft Edge to users of iOS, iPadOS, and Android devices.</span></span>

> [!NOTE]
> <span data-ttu-id="275a6-104">إذا قمت بحظر المستخدمين من تسجيل الأجهزة المحمولة، فلن يعمل هذا السيناريو الإرشادي وسيحتاج المستخدمون إلى تثبيت Microsoft Edge بمفردهم.</span><span class="sxs-lookup"><span data-stu-id="275a6-104">If you blocked users from enrolling mobile devices, this guided scenario won't work and the users will need to install Microsoft Edge on their own.</span></span>

<span data-ttu-id="275a6-105">يتضمن السيناريو الإرشادي الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="275a6-105">The guided scenario involves the following steps:</span></span>

1. [<span data-ttu-id="275a6-106">المتطلبات الأساسية</span><span class="sxs-lookup"><span data-stu-id="275a6-106">Prerequisites</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#prerequisites)
2. [<span data-ttu-id="275a6-107">مقدمة</span><span class="sxs-lookup"><span data-stu-id="275a6-107">Introduction</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-1---introduction)
3. [<span data-ttu-id="275a6-108">الأساسيات</span><span class="sxs-lookup"><span data-stu-id="275a6-108">Basics</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-2---basics)
4. [<span data-ttu-id="275a6-109">تكوين</span><span class="sxs-lookup"><span data-stu-id="275a6-109">Configuration</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-3---configuration)
5. [<span data-ttu-id="275a6-110">الواجبات</span><span class="sxs-lookup"><span data-stu-id="275a6-110">Assignments</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-4---assignments)
6. [<span data-ttu-id="275a6-111">المراجعة والخلق</span><span class="sxs-lookup"><span data-stu-id="275a6-111">Review and creation</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-5---review--create)

<span data-ttu-id="275a6-112">بعد إكمال الخطوات في السيناريو الإرشادي، ستمكن سياسات Microsoft Intune الميزات التالية في Microsoft Edge للأعمال:</span><span class="sxs-lookup"><span data-stu-id="275a6-112">After you complete the steps in the guided scenario, Microsoft Intune policies will enable the following features of Microsoft Edge for business:</span></span>

- <span data-ttu-id="275a6-113">هوية مزدوجة</span><span class="sxs-lookup"><span data-stu-id="275a6-113">Dual identity</span></span>
- <span data-ttu-id="275a6-114">التكامل مع نهج حماية تطبيق Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="275a6-114">Integration with Microsoft Intune app protection policy</span></span>
- <span data-ttu-id="275a6-115">التكامل مع وكيل تطبيق Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="275a6-115">Integration with Azure Active Directory Application Proxy</span></span>
- <span data-ttu-id="275a6-116">المفضلة المدارة واختصارات الصفحة الرئيسية</span><span class="sxs-lookup"><span data-stu-id="275a6-116">Managed favorites and home page shortcuts</span></span>
