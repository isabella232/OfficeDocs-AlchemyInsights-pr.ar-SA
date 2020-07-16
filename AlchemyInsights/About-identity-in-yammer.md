---
title: حول الهوية في Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6039"
- "9003111"
ms.openlocfilehash: 2c4c2c836d18d2ab45e2368e778c793277b18aa0
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148165"
---
# <a name="about-identity-in-yammer"></a><span data-ttu-id="f3a19-102">حول الهوية في Yammer</span><span class="sxs-lookup"><span data-stu-id="f3a19-102">About identity in Yammer</span></span>

<span data-ttu-id="f3a19-103">من المستحسن أن كافة الشبكات اتخاذ الخطوات التالية لتجنب المشاكل المتعلقة بالهوية:</span><span class="sxs-lookup"><span data-stu-id="f3a19-103">It is recommended that all networks take the following steps to avoid identity-related issues:</span></span>

1. <span data-ttu-id="f3a19-104">فرض هوية Office 365 بعد توفير حسابات Microsoft 365 للمستخدمين في إعلان Azure للتأكد من أن كافة المستخدمين تسجيل الدخول باستخدام حساب Microsoft 365 الأساسي الخاص بهم.</span><span class="sxs-lookup"><span data-stu-id="f3a19-104">Enforce Office 365 identity after provisioning Microsoft 365 accounts for users in Azure AD to ensure that all users sign in by using their primary Microsoft 365 account.</span></span> <span data-ttu-id="f3a19-105">لمزيد من المعلومات، راجع [فرض هوية Office 365 لمستخدمي Yammer](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).</span><span class="sxs-lookup"><span data-stu-id="f3a19-105">For more info, see [Enforce Office 365 identity for Yammer users](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).</span></span>
2. <span data-ttu-id="f3a19-106">دمج شبكات Yammer متعددة.</span><span class="sxs-lookup"><span data-stu-id="f3a19-106">Consolidate multiple Yammer networks.</span></span> <span data-ttu-id="f3a19-107">تسمح التكوينات Yammer القديمة لعدة شبكات Yammer أن تكون متصلاً بمستأجر واحد.</span><span class="sxs-lookup"><span data-stu-id="f3a19-107">Legacy Yammer configurations permit multiple Yammer networks to be connected to one tenant.</span></span> <span data-ttu-id="f3a19-108">لمزيد من المعلومات، راجع [ترحيل الشبكة - دمج شبكات Yammer المتعددة](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span><span class="sxs-lookup"><span data-stu-id="f3a19-108">For more info, see [Network migration - Consolidate multiple Yammer networks](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span></span>
3. <span data-ttu-id="f3a19-109">اختيارياً، فرض الترخيص لـ Yammer لحظر المستخدمين من Yammer إذا لم يكن لديهم ترخيص.</span><span class="sxs-lookup"><span data-stu-id="f3a19-109">Optionally, enforce licensing for Yammer to block users from Yammer if they don't have a license.</span></span> <span data-ttu-id="f3a19-110">لمزيد من المعلومات، راجع [إدارة تراخيص المستخدمين Yammer في Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="f3a19-110">For more info, see [Manage Yammer user licenses in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).</span></span>
4. <span data-ttu-id="f3a19-111">وأخيراً، تدوين قائمة المستخدمين لشبكات Yammer القديمة وتعليق المستخدمين القديمة.</span><span class="sxs-lookup"><span data-stu-id="f3a19-111">Finally, audit the user list for older Yammer networks and suspend legacy users.</span></span> <span data-ttu-id="f3a19-112">من المستحسن أن تقوم بإيقاف (إلغاء تنشيط) المستخدمين بدلاً من حذفهم، لأن الحذف لا رجعة فيه.</span><span class="sxs-lookup"><span data-stu-id="f3a19-112">It is recommended that you suspend (deactivate) users instead of deleting them, because deletion is irreversible.</span></span> <span data-ttu-id="f3a19-113">لمزيد من المعلومات، راجع [تدقيق المستخدمين Yammer في الشبكات المتصلة بـ Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) [وإزالة المستخدمين](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).</span><span class="sxs-lookup"><span data-stu-id="f3a19-113">For more info, see [Audit Yammer users in networks connected to Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) and [Remove users](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).</span></span>

<span data-ttu-id="f3a19-114">بتكوين Yammer باستخدام هذه الخطوات، ستكون أيضاً جاهزاً لتكوين شبكة Yammer لـ الوضع الأصلي لـ Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="f3a19-114">By configuring Yammer using these steps, you'll also be ready to configure your Yammer network for Native Mode for Microsoft 365.</span></span> <span data-ttu-id="f3a19-115">لمزيد من المعلومات، راجع [تكوين شبكة Yammer الخاصة بك لـ الوضع الأصلي لـ Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).</span><span class="sxs-lookup"><span data-stu-id="f3a19-115">For more info, see [Configure your Yammer network for Native Mode for Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).</span></span>