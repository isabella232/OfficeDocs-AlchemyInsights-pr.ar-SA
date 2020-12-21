---
title: أداره مجموعات التطبيقات باستخدام مدخل Azure لسطح مكتب Windows الظاهري
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003956"
- "7013"
ms.openlocfilehash: 0dd08d04ad6328e7afa158b36517839fc31a8566
ms.sourcegitcommit: 2ffdf6096de5608b117c6677d3cd7dd4c23ea024
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/18/2020
ms.locfileid: "49721743"
---
# <a name="manage-app-groups-by-using-the-azure-portal-for-windows-virtual-desktop"></a><span data-ttu-id="8471e-102">أداره مجموعات التطبيقات باستخدام مدخل Azure لسطح مكتب Windows الظاهري</span><span class="sxs-lookup"><span data-stu-id="8471e-102">Manage app groups by using the Azure portal for Windows Virtual Desktop</span></span>

<span data-ttu-id="8471e-103">تقوم مجموعه التطبيقات الافتراضية التي تم إنشاؤها لتجمع مضيف سطح مكتب Windows ظاهري جديد بنشر سطح المكتب بالبالكامل.</span><span class="sxs-lookup"><span data-stu-id="8471e-103">The default app group created for a new Windows Virtual Desktop host pool also publishes the full desktop.</span></span> <span data-ttu-id="8471e-104">بالاضافه إلى ذلك ، فان استخدام مدخل Azure يسمح لك بإنشاء مجموعه تطبيق RemoteApp واحده أو أكثر لتجمع المضيف.</span><span class="sxs-lookup"><span data-stu-id="8471e-104">In addition, using the Azure portal lets you create one or more RemoteApp app groups for the host pool.</span></span>

<span data-ttu-id="8471e-105">ستقوم عمليه النشر بما يلي:</span><span class="sxs-lookup"><span data-stu-id="8471e-105">The deployment process will do the following:</span></span>

1. <span data-ttu-id="8471e-106">إنشاء مجموعه تطبيق RemoteApp.</span><span class="sxs-lookup"><span data-stu-id="8471e-106">Create the RemoteApp app group.</span></span>
2. <span data-ttu-id="8471e-107">أضف التطبيقات المحددة إلى مجموعه التطبيقات.</span><span class="sxs-lookup"><span data-stu-id="8471e-107">Add your selected apps to the app group.</span></span>
3. <span data-ttu-id="8471e-108">نشر مستخدمين فرديين أو مجموعات مستخدمين إلى مجموعه التطبيقات.</span><span class="sxs-lookup"><span data-stu-id="8471e-108">Publish individual users or user groups to the app group.</span></span>
4. <span data-ttu-id="8471e-109">سجل مجموعه التطبيقات ، إذا اخترت القيام بذلك.</span><span class="sxs-lookup"><span data-stu-id="8471e-109">Register the app group, if you choose to do so.</span></span>
5. <span data-ttu-id="8471e-110">يمكنك إنشاء ارتباط إلى قالب أداره موارد Azure وفقا للتكوين ، الذي يمكنك تنزيله وحفظه.</span><span class="sxs-lookup"><span data-stu-id="8471e-110">Create a link to an Azure Resource Manager template according to your configuration, which you can download and save.</span></span>

<span data-ttu-id="8471e-111">لإنشاء مجموعه RemoteApp ل Windows Virtual Desktop ، اتبع الإرشادات الموجودة في [أداره مجموعات التطبيقات باستخدام مدخل Azure](https://go.microsoft.com/fwlink/?linkid=2129550).</span><span class="sxs-lookup"><span data-stu-id="8471e-111">To create a RemoteApp group for Windows Virtual Desktop, follow the instructions in [Manage app groups with the Azure portal](https://go.microsoft.com/fwlink/?linkid=2129550).</span></span>
