---
title: تكوين خدمه المجالات
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
- "7931"
- "9004400"
ms.openlocfilehash: 51e0bd78240627876721cbce654188afac1ee365
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/18/2021
ms.locfileid: "49884806"
---
# <a name="unable-to-enable-aad-ds-or-deployment-is-failing"></a><span data-ttu-id="d7252-102">تعذر تمكين AAD أو فشل النشر</span><span class="sxs-lookup"><span data-stu-id="d7252-102">Unable to enable AAD-DS or deployment is failing</span></span>

<span data-ttu-id="d7252-103">لحل مشكله خدمه مجال Azure AD (AAD-DS) غير ممكنة أو فشل نشرها ، قم بتنفيذ الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="d7252-103">To solve the issue of Azure AD domain service (AAD-DS) not being enabled or failing to be deployed, perform the following steps:</span></span>

1. <span data-ttu-id="d7252-104">إذا كنت تستخدم شبكه ظاهريه موجودة بالفعل ، فتحقق من نسجك عن القواعد التي تحظر المنافذ المطلوبة للمزامنة في AAD في المدخل https://aka.ms/aadds-networking .</span><span class="sxs-lookup"><span data-stu-id="d7252-104">If you are using an already existing virtual network, check your NSG for rules that block ports needed to synchronize in AAD-DS in the portal https://aka.ms/aadds-networking.</span></span>
2. <span data-ttu-id="d7252-105">تحقق لمعرفه ما إذا تم الرد علي رسالة الخطا الخاصة بك في دليل استكشاف الأخطاء وإصلاحها المتوفر في  https://aka.ms/aadds-troubleshoot-enable .</span><span class="sxs-lookup"><span data-stu-id="d7252-105">Check to see if your error message is answered in this troubleshooting guide that is available in  https://aka.ms/aadds-troubleshoot-enable.</span></span>
3. <span data-ttu-id="d7252-106">جرب نشر خدمات مجالات Azure AD في شبكه ظاهريه جديده.</span><span class="sxs-lookup"><span data-stu-id="d7252-106">Try deploying Azure AD Domain Services in a new virtual network.</span></span>
4. <span data-ttu-id="d7252-107">اتبع دليل بدء الاستخدام حول كيفيه نشر AAD-DS: [إنشاء خدمات مجال AAD وتكوينها](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).</span><span class="sxs-lookup"><span data-stu-id="d7252-107">Follow the Getting Started guide on how to deploy AAD-DS: [Create and Configure AAD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).</span></span>
5. <span data-ttu-id="d7252-108">إذا واجهتك مشاكل في نشر خدمات مجالات Azure AD ، فراجع [استكشاف أخطاء خدمات مجال AZURE ad وإصلاحها](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot)</span><span class="sxs-lookup"><span data-stu-id="d7252-108">If you are having issues with Deploying Azure AD Domain Services, see [Troubleshoot Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) to resolve common errors to help you get things working again.</span></span> 

<span data-ttu-id="d7252-109">**تعذر تعطيل AAD-DS**</span><span class="sxs-lookup"><span data-stu-id="d7252-109">**Unable to disable AAD-DS**</span></span>

<span data-ttu-id="d7252-110">تعذر إيقاف AAD-DS مؤقتا.</span><span class="sxs-lookup"><span data-stu-id="d7252-110">AAD-DS is unable to be paused.</span></span> <span data-ttu-id="d7252-111">إذا كنت ترغب في التوقف عن استخدام مجالك المدار ، فيجب حذفه.</span><span class="sxs-lookup"><span data-stu-id="d7252-111">If you wish to stop using your managed domain, it must be deleted.</span></span>
<span data-ttu-id="d7252-112">لحذف مجالك المدار ، راجع [حذف خدمه مجال AAD](https://docs.microsoft.com/azure/active-directory-domain-services/delete-aadds).</span><span class="sxs-lookup"><span data-stu-id="d7252-112">To delete your Managed domain, see [Delete AAD Domain Service](https://docs.microsoft.com/azure/active-directory-domain-services/delete-aadds).</span></span>



