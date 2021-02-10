---
title: مشكلة في مجموعات الأمان
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8252"
- "9004397"
ms.openlocfilehash: 1198b79c3301bd2752a7385a6ba6746c8f0c2b5b
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177353"
---
# <a name="issue-with-security-groups"></a><span data-ttu-id="562fb-102">مشكلة في مجموعات الأمان</span><span class="sxs-lookup"><span data-stu-id="562fb-102">Issue with security groups</span></span>

<span data-ttu-id="562fb-103">**إذا كنت تحصل على خطأ في الشبكة AADDS104**</span><span class="sxs-lookup"><span data-stu-id="562fb-103">**If you are getting Network Error AADDS104**</span></span>

<span data-ttu-id="562fb-104">قواعد مجموعة أمان الشبكة غير الصالحة هي السبب الأكثر شيوعا لأخطاء الشبكة لخدمات مجال Azure Active Directory (AD DS).</span><span class="sxs-lookup"><span data-stu-id="562fb-104">Invalid network security group rules are the most common cause of network errors for Azure Active Directory Domain Services (AD DS).</span></span> <span data-ttu-id="562fb-105">يجب أن تسمح مجموعة أمان الشبكة للشبكة الظاهرية بالوصول إلى منافذ بروتوكولات وبروتوكولات معينة.</span><span class="sxs-lookup"><span data-stu-id="562fb-105">The network security group for the virtual network must allow access to specific ports and protocols.</span></span> <span data-ttu-id="562fb-106">إذا تم حظر هذه المنافذ، لا يمكن ل Azure مراقبة المجال المدار أو تحديثه.</span><span class="sxs-lookup"><span data-stu-id="562fb-106">If these ports are blocked, the Azure platform can't monitor or update the managed domain.</span></span> <span data-ttu-id="562fb-107">كما تؤثر المزامنة بين Azure AD و Azure AD DS.</span><span class="sxs-lookup"><span data-stu-id="562fb-107">The synchronization between the Azure AD and Azure AD DS is also impacted.</span></span> <span data-ttu-id="562fb-108">تأكد من الاحتفاظ بالمنافذ الافتراضية مفتوحة لتجنب انقطاع الخدمة.</span><span class="sxs-lookup"><span data-stu-id="562fb-108">Ensure you keep the default ports open to avoid interruption in service.</span></span>

<span data-ttu-id="562fb-109">لفهم التنبيهات الشائعة لحل مشاكل تكوين مجموعة أمان الشبكة، راجع [إضافة مجموعات الأمان والتحقق منها.](https://docs.microsoft.com/azure/active-directory-domain-services/alert-nsg#verify-and-edit-existing-security-rules)</span><span class="sxs-lookup"><span data-stu-id="562fb-109">To understand and to resolve common alerts for network security group configuration issues, see [Add and Verify Security Groups](https://docs.microsoft.com/azure/active-directory-domain-services/alert-nsg#verify-and-edit-existing-security-rules).</span></span>
