---
title: لا تتم مزامنة Active Directory
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "1300023"
- "3754"
- "4531"
ms.openlocfilehash: 0da512379e5a2f6ccb773e18c465e545c0660560
ms.sourcegitcommit: e42bb24c9bae1d0df8c49c424d2aa5e7466703ac
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/14/2021
ms.locfileid: "52930962"
---
# <a name="active-directory-not-syncing"></a><span data-ttu-id="e965f-102">لا تتم مزامنة Active Directory</span><span class="sxs-lookup"><span data-stu-id="e965f-102">Active Directory not syncing</span></span>

<span data-ttu-id="e965f-103">إذا كنت تتلقى أخطاء في المزامنة، مثل "لا توجد مزامنة حديثة"، أو لاحظت حالة مزامنة الدليل في مدخل مسؤول Office، تقول "آخر مزامنة منذ أكثر من 3 أيام"، فقد يكون سبب ذلك أن AADConnect لديه إعدادات غير صحيحة أو أذونات غير كافية لتنفيذ المزامنة.</span><span class="sxs-lookup"><span data-stu-id="e965f-103">If you are receiving synchronization errors, such as "no recent synchronization," or notice the directory synchronization status in the Office admin portal says, "Last synced more than 3 days ago," it may be that AADConnect has incorrect settings or insufficient permissions to perform a synchronization.</span></span>  

<span data-ttu-id="e965f-104">قد يحل إعادة تثبيت AADConnect باستخدام الإعدادات المعبرة المشكلة بسرعة:</span><span class="sxs-lookup"><span data-stu-id="e965f-104">Reinstalling AADConnect by using express settings might resolve the issue quickly:</span></span>

1. <span data-ttu-id="e965f-105">[قم بتنزيل أحدث إصدار من AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span><span class="sxs-lookup"><span data-stu-id="e965f-105">[Download the latest version of AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span></span>

2. <span data-ttu-id="e965f-106">[اتبع إرشادات التثبيت السريع.](/azure/active-directory/hybrid/how-to-connect-install-express)</span><span class="sxs-lookup"><span data-stu-id="e965f-106">[Follow the instructions for express installation](/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

<span data-ttu-id="e965f-107">يجب تثبيت Azure AD Connect على نظام التشغيل Windows Server 2012 أو أحدث.</span><span class="sxs-lookup"><span data-stu-id="e965f-107">Azure AD Connect must be installed on Windows Server 2012 or later.</span></span> <span data-ttu-id="e965f-108">يجب أن يكون هذا الخادم مشتركاً وقد يكون عبارة عن وحدة تحكم بالمجال أو خادم عضو.</span><span class="sxs-lookup"><span data-stu-id="e965f-108">This server must be domain joined and may be a domain controller or a member server.</span></span> <span data-ttu-id="e965f-109">للحصول على قائمة كاملة بمتطلبات Azure AD الاتصال والمتطلبات الأساسية، راجع المتطلبات الأساسية ل [Azure AD الاتصال](/azure/active-directory/hybrid/how-to-connect-install-prerequisites).</span><span class="sxs-lookup"><span data-stu-id="e965f-109">For a full list of Azure AD Connect requirements and pre-requisites, review [Prerequisites for Azure AD Connect](/azure/active-directory/hybrid/how-to-connect-install-prerequisites).</span></span>

<span data-ttu-id="e965f-110">لمزيد من المعلومات حول حسابات خدمة AADConnect، راجع [Azure AD الاتصال: الحسابات والأذونات](/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span><span class="sxs-lookup"><span data-stu-id="e965f-110">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span></span>
