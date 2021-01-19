---
title: وحدة التحكم في المجال
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7909"
- "9003233"
ms.openlocfilehash: d4cbe80c3e8f0ce32fcbe89e852f24efd6f50575
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/18/2021
ms.locfileid: "49900732"
---
# <a name="domain-controller"></a><span data-ttu-id="8c8c9-102">وحدة التحكم في المجال</span><span class="sxs-lookup"><span data-stu-id="8c8c9-102">Domain controller</span></span>

<span data-ttu-id="8c8c9-103">**تعذر تمكين AAD أو فشل النشر**</span><span class="sxs-lookup"><span data-stu-id="8c8c9-103">**Unable to enable AAD-DS or deployment is failing**</span></span>

<span data-ttu-id="8c8c9-104">لحل مشكله خدمه مجال Azure AD (AAD-DS) غير ممكنة أو فشل نشرها ، قم بتنفيذ الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="8c8c9-104">To solve the issue of Azure AD domain service (AAD-DS) not being enabled or failing to be deployed, perform the following steps:</span></span>

1. <span data-ttu-id="8c8c9-105">إذا كنت تستخدم شبكه ظاهريه موجودة بالفعل ، فتحقق من نسجك عن القواعد التي تحظر المنافذ المطلوبة للمزامنة في AAD في المدخل https://aka.ms/aadds-networking .</span><span class="sxs-lookup"><span data-stu-id="8c8c9-105">If you are using an already existing virtual network, check your NSG for rules that block ports needed to synchronize in AAD-DS in the portal https://aka.ms/aadds-networking.</span></span>
2. <span data-ttu-id="8c8c9-106">تحقق لمعرفه ما إذا تم الرد علي رسالة الخطا الخاصة بك في دليل استكشاف الأخطاء وإصلاحها المتوفر في  https://aka.ms/aadds-troubleshoot-enable .</span><span class="sxs-lookup"><span data-stu-id="8c8c9-106">Check to see if your error message is answered in this troubleshooting guide that is available in  https://aka.ms/aadds-troubleshoot-enable.</span></span>
3. <span data-ttu-id="8c8c9-107">جرب نشر خدمات مجالات Azure AD في شبكه ظاهريه جديده.</span><span class="sxs-lookup"><span data-stu-id="8c8c9-107">Try deploying Azure AD Domain Services in a new virtual network.</span></span>
4. <span data-ttu-id="8c8c9-108">اتبع دليل بدء الاستخدام حول كيفيه نشر AAD-DS ، والمتوفرة في [البرنامج التعليمي لإنشاء خدمات مجال AZURE AD](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).</span><span class="sxs-lookup"><span data-stu-id="8c8c9-108">Follow the Getting Started guide on how to deploy AAD-DS, which is available at [Tutorial to Create Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).</span></span>
5. <span data-ttu-id="8c8c9-109">إذا واجهتك مشاكل في نشر خدمات مجالات Azure AD ، فراجع [استكشاف أخطاء خدمات مجال AZURE ad وإصلاحها](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot)</span><span class="sxs-lookup"><span data-stu-id="8c8c9-109">If you are having issues with Deploying Azure AD Domain Services, see [Troubleshoot Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) to resolve common errors to help you get things working again.</span></span> 

<span data-ttu-id="8c8c9-110">**تعذر تعطيل AAD-DS**</span><span class="sxs-lookup"><span data-stu-id="8c8c9-110">**Unable to disable AAD-DS**</span></span>

<span data-ttu-id="8c8c9-111">تعذر إيقاف AAD-DS مؤقتا.</span><span class="sxs-lookup"><span data-stu-id="8c8c9-111">AAD-DS is unable to be paused.</span></span> <span data-ttu-id="8c8c9-112">إذا كنت ترغب في التوقف عن استخدام مجالك المدار ، فيجب حذفه.</span><span class="sxs-lookup"><span data-stu-id="8c8c9-112">If you wish to stop using your managed domain, it must be deleted.</span></span>

<span data-ttu-id="8c8c9-113">إذا واجهت مشاكل ، لحل رسائل الخطا الشائعة والخطوات المتعلقة باستكشاف الأخطاء وإصلاحها لمساعدتك علي تنفيذ المهام مره أخرى ، راجع [استكشاف الأخطاء وإصلاحها ل Azure active Directory Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot).</span><span class="sxs-lookup"><span data-stu-id="8c8c9-113">If you run into issues, to resolve common error messages and for associated troubleshooting steps to help you get things running again, see [Troubleshoot Azure Active Directory Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot).</span></span>
