---
title: حول الهوية في Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6039"
- "9003111"
ms.openlocfilehash: f417117acac4c3040932fc0a35e5d0b1c3709cd5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664157"
---
# <a name="about-identity-in-yammer"></a><span data-ttu-id="4dab5-102">حول الهوية في Yammer</span><span class="sxs-lookup"><span data-stu-id="4dab5-102">About identity in Yammer</span></span>

<span data-ttu-id="4dab5-103">من المستحسن تنفيذ كل الشبكات علي الخطوات التالية لتجنب المشاكل ذات الصلة بالهوية:</span><span class="sxs-lookup"><span data-stu-id="4dab5-103">It is recommended that all networks take the following steps to avoid identity-related issues:</span></span>

1. <span data-ttu-id="4dab5-104">فرض هويه Office 365 بعد توفير حسابات Microsoft 365 للمستخدمين في Azure AD للتاكد من ان كل المستخدمين يقومون بتسجيل الدخول باستخدام حساب Microsoft 365 الأساسي الخاص بهم.</span><span class="sxs-lookup"><span data-stu-id="4dab5-104">Enforce Office 365 identity after provisioning Microsoft 365 accounts for users in Azure AD to ensure that all users sign in by using their primary Microsoft 365 account.</span></span> <span data-ttu-id="4dab5-105">للحصول علي مزيد من المعلومات ، راجع [فرض هويه Office 365 لمستخدمي Yammer](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).</span><span class="sxs-lookup"><span data-stu-id="4dab5-105">For more info, see [Enforce Office 365 identity for Yammer users](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).</span></span>
2. <span data-ttu-id="4dab5-106">دمج عده شبكات Yammer.</span><span class="sxs-lookup"><span data-stu-id="4dab5-106">Consolidate multiple Yammer networks.</span></span> <span data-ttu-id="4dab5-107">تسمح تكوينات Yammer القديمة بتوصيل شبكات Yammer بمستاجر واحد.</span><span class="sxs-lookup"><span data-stu-id="4dab5-107">Legacy Yammer configurations permit multiple Yammer networks to be connected to one tenant.</span></span> <span data-ttu-id="4dab5-108">للحصول علي مزيد من المعلومات ، راجع [ترحيل الشبكة-دمج شبكات Yammer متعددة](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span><span class="sxs-lookup"><span data-stu-id="4dab5-108">For more info, see [Network migration - Consolidate multiple Yammer networks](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span></span>
3. <span data-ttu-id="4dab5-109">بشكل اختياري ، قم بفرض الترخيص ل Yammer لحظر المستخدمين من Yammer إذا لم يكن لديهم ترخيص.</span><span class="sxs-lookup"><span data-stu-id="4dab5-109">Optionally, enforce licensing for Yammer to block users from Yammer if they don't have a license.</span></span> <span data-ttu-id="4dab5-110">للحصول علي مزيد من المعلومات ، راجع [أداره تراخيص مستخدمي Yammer في Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="4dab5-110">For more info, see [Manage Yammer user licenses in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).</span></span>
4. <span data-ttu-id="4dab5-111">أخيرا ، قم بتدوين قائمه المستخدمين لشبكات Yammer القديمة وتوقف المستخدمون القديمون.</span><span class="sxs-lookup"><span data-stu-id="4dab5-111">Finally, audit the user list for older Yammer networks and suspend legacy users.</span></span> <span data-ttu-id="4dab5-112">من المستحسن ان تقوم بإيقاف (إلغاء تنشيط) المستخدمين بدلا من حذفها ، لان الحذف غير مقبول.</span><span class="sxs-lookup"><span data-stu-id="4dab5-112">It is recommended that you suspend (deactivate) users instead of deleting them, because deletion is irreversible.</span></span> <span data-ttu-id="4dab5-113">للحصول علي مزيد من المعلومات ، راجع [تدوين مستخدمي Yammer في الشبكات المتصلة ب Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) [وأزاله المستخدمين](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).</span><span class="sxs-lookup"><span data-stu-id="4dab5-113">For more info, see [Audit Yammer users in networks connected to Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) and [Remove users](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).</span></span>

<span data-ttu-id="4dab5-114">بتكوين Yammer باستخدام هذه الخطوات ، ستكون جاهزا أيضا لتكوين شبكه Yammer للوضع الأصلي ل Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="4dab5-114">By configuring Yammer using these steps, you'll also be ready to configure your Yammer network for Native Mode for Microsoft 365.</span></span> <span data-ttu-id="4dab5-115">لمزيد من المعلومات ، راجع [تكوين شبكه Yammer للوضع الأصلي ل Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).</span><span class="sxs-lookup"><span data-stu-id="4dab5-115">For more info, see [Configure your Yammer network for Native Mode for Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).</span></span>