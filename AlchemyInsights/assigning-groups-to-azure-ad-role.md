---
title: تعيين مجموعات إلى دور Azure AD
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7898"
- "9003230"
ms.openlocfilehash: feca81fe785bc45e47f6faa876230b5c7701713d
ms.sourcegitcommit: 6dc6f999e840c90694a246b90062950205679420
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/15/2021
ms.locfileid: "49884761"
---
# <a name="assigning-groups-to-azure-ad-role"></a><span data-ttu-id="60723-102">تعيين مجموعات إلى دور Azure AD</span><span class="sxs-lookup"><span data-stu-id="60723-102">Assigning groups to Azure AD role</span></span>

<span data-ttu-id="60723-103">لتعيين مجموعه Azure AD مع مصدر التخويل في Azure AD إلى دور Azure AD ، نفذ الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="60723-103">To assign an Azure AD group with source of authority in Azure AD to an Azure AD role, perform the following steps:</span></span>

1. <span data-ttu-id="60723-104">إنشاء مجموعه جديده-لإنشاء مجموعه جديده:</span><span class="sxs-lookup"><span data-stu-id="60723-104">Create a new group - To create a new group:</span></span>

    <span data-ttu-id="60723-105">علي.</span><span class="sxs-lookup"><span data-stu-id="60723-105">a.</span></span> <span data-ttu-id="60723-106">سجل دخولك إلى مركز أداره Azure AD باستخدام **مسؤول دور مميز** أو أذونات **المسؤول العام** .</span><span class="sxs-lookup"><span data-stu-id="60723-106">Sign in to the Azure AD admin center with **privileged role administrator** or **global administrator** permissions.</span></span>
    <span data-ttu-id="60723-107">ب.</span><span class="sxs-lookup"><span data-stu-id="60723-107">b.</span></span> <span data-ttu-id="60723-108">حدد **مجموعات Azure Active directory > > كل المجموعات > المجموعة الجديدة**.</span><span class="sxs-lookup"><span data-stu-id="60723-108">Select **Azure Active Directory > Groups > All groups > New group**.</span></span>
    <span data-ttu-id="60723-109">ن.</span><span class="sxs-lookup"><span data-stu-id="60723-109">c.</span></span> <span data-ttu-id="60723-110">إنشاء المجموعة.</span><span class="sxs-lookup"><span data-stu-id="60723-110">Create the group.</span></span>

2. <span data-ttu-id="60723-111">تعيين الدور إلى المجموعة اما اثناء إنشاء المجموعة أو بعد إنشاء المجموعة.</span><span class="sxs-lookup"><span data-stu-id="60723-111">Assign the role to the group either during group creation or after the group is created.</span></span>

    <span data-ttu-id="60723-112">علي.</span><span class="sxs-lookup"><span data-stu-id="60723-112">a.</span></span> <span data-ttu-id="60723-113">لتعيين دور إلى المجموعة في وقت إنشاء المجموعة ، يمكنك التبديل علي ادوار التبديل في **AZURE AD للمجموعة** وإنشاء المجموعة.</span><span class="sxs-lookup"><span data-stu-id="60723-113">To assign a role to the group at the time of group creation, switch on the toggle **Azure AD roles can be assigned to the group** and create the group.</span></span>
    <span data-ttu-id="60723-114">ب.</span><span class="sxs-lookup"><span data-stu-id="60723-114">b.</span></span> <span data-ttu-id="60723-115">لتعيين دور إلى المجموعة بعد إنشائه ، انتقل إلى علامة التبويب **الأدوار المعينة** للمجموعة التي تم إنشاؤها حديثا ، وقم بتعيين الدور إلى المجموعة.</span><span class="sxs-lookup"><span data-stu-id="60723-115">To assign a role to the group after it has been created, navigate to the **Assigned roles** tab for the newly created group, and assign the role to the group.</span></span>  

<span data-ttu-id="60723-116">**أداره عضويه مجموعه تم تعيينها إلى دور Azure AD**</span><span class="sxs-lookup"><span data-stu-id="60723-116">**Manage membership of a group that is assigned to Azure AD role**</span></span>

<span data-ttu-id="60723-117">لمنع رفع الامتيازات ، بشكل افتراضي ، يمكن لمسؤولي الأدوار المسموحين والمسؤولين العموميين فقط تعديل عضويه مجموعه تم تعيينها لأحد الأدوار.</span><span class="sxs-lookup"><span data-stu-id="60723-117">To prevent elevation of privileges, by default, only privileged role administrators and global administrators can modify the membership of a group that is assigned to a role.</span></span> <span data-ttu-id="60723-118">ومع ذلك ، يمكنك اختيار تعيين مالك لهذه المجموعة وتفويض هذه المهمة.</span><span class="sxs-lookup"><span data-stu-id="60723-118">They can, however, choose to assign an owner for such a group and delegate this task.</span></span>

<span data-ttu-id="60723-119">للحصول علي مزيد من التفاصيل حول تعيين مجموعات السحابة إلى ادوار Azure AD ، راجع [تعيين ادوار إعلانات إلى مجموعه السحابة](https://docs.microsoft.com/azure/active-directory/roles/groups-concept).</span><span class="sxs-lookup"><span data-stu-id="60723-119">For more details on assigning cloud groups to Azure AD roles, see [Assign a AD roles to Cloud Group](https://docs.microsoft.com/azure/active-directory/roles/groups-concept).</span></span> <span data-ttu-id="60723-120">للحصول علي مزيد من التفاصيل حول استكشاف الأخطاء وإصلاحها للأدوار المعينة إلى مجموعات السحابة ، راجع [استكشاف أخطاء الأدوار المعينة لمجموعات السحابة](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting)</span><span class="sxs-lookup"><span data-stu-id="60723-120">For more details on troubleshooting roles assigned to cloud groups, see [Troubleshoot roles assigned to cloud groups](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).</span></span>





