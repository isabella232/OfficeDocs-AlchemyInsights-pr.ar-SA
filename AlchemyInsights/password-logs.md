---
title: سجلات كلمات المرور
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9361"
- "9003259"
ms.openlocfilehash: ed151b436fa2043c610931deeb74a202af88fcf4
ms.sourcegitcommit: 226fe97678b6be215eda0c278399f8be9be525c1
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/08/2021
ms.locfileid: "50523354"
---
# <a name="password-logs"></a><span data-ttu-id="4c448-102">سجلات كلمات المرور</span><span class="sxs-lookup"><span data-stu-id="4c448-102">Password logs</span></span>

<span data-ttu-id="4c448-103">**أواجه مشاكل في الوصول إلى سجلات تدقيق إعادة تعيين كلمة المرور**</span><span class="sxs-lookup"><span data-stu-id="4c448-103">**I'm having problems accessing password reset audit logs**</span></span>

<span data-ttu-id="4c448-104">استكشاف المشاكل المتعلقة بالوصول إلى سجلات تدقيق إعادة تعيين كلمة المرور وإصلاحها، قم بتنفيذ الخطوة التالية:</span><span class="sxs-lookup"><span data-stu-id="4c448-104">To troubleshoot issues regarding access to password reset audit logs, perform the following step:</span></span>

<span data-ttu-id="4c448-105">تأكد من أنك مفوض لعرض سجلات التدقيق.</span><span class="sxs-lookup"><span data-stu-id="4c448-105">Ensure you are authorized to view audit logs.</span></span> 

<span data-ttu-id="4c448-106">الأدوار التالية هي فقط المعتمدة:</span><span class="sxs-lookup"><span data-stu-id="4c448-106">Only the following roles are authorized:</span></span>
 - <span data-ttu-id="4c448-107">المسؤول العام</span><span class="sxs-lookup"><span data-stu-id="4c448-107">Global administrator</span></span>
 - <span data-ttu-id="4c448-108">مسؤول الأمان</span><span class="sxs-lookup"><span data-stu-id="4c448-108">Security administrator</span></span>
 - <span data-ttu-id="4c448-109">قارئ الأمان</span><span class="sxs-lookup"><span data-stu-id="4c448-109">Security reader</span></span>

<span data-ttu-id="4c448-110">**أريد رؤية كل أحداث إعادة تعيين كلمة المرور للتدقيق من وقت نشر كلمة المرور**</span><span class="sxs-lookup"><span data-stu-id="4c448-110">**I want to see all password reset audit events from the time I initially deployed**</span></span>

<span data-ttu-id="4c448-111">يتم تخزين ما يصل إلى 120000 من أحداث إعادة تعيين/تسجيل كلمات المرور في تقارير آخر 30 يوما.</span><span class="sxs-lookup"><span data-stu-id="4c448-111">Up to 120,000 password reset/registration events are stored in the reports of the last 30 days.</span></span> <span data-ttu-id="4c448-112">ينطبق هذا الحد الأقصى على واجهة المستخدم عند تنزيل CSV.</span><span class="sxs-lookup"><span data-stu-id="4c448-112">This maximum limit applies to the UI when downloading the CSV.</span></span> <span data-ttu-id="4c448-113">يتوفر 1 مليون حدث من خلال PowerShell.</span><span class="sxs-lookup"><span data-stu-id="4c448-113">1 million events are available through PowerShell.</span></span>
<span data-ttu-id="4c448-114">لمزيد من المعلومات، راجع الارتباطات أدناه:</span><span class="sxs-lookup"><span data-stu-id="4c448-114">For more information, see the links below:</span></span>

- [<span data-ttu-id="4c448-115">إعادة تعيين أحداث كلمة المرور للخدمة الذاتية من Azure AD Reports and Events API</span><span class="sxs-lookup"><span data-stu-id="4c448-115">Self-service password reset events from the Azure AD Reports and Events API</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="4c448-116">كيفية تنزيل أحداث إعادة تعيين تسجيل كلمات المرور بسرعة باستخدام PowerShell</span><span class="sxs-lookup"><span data-stu-id="4c448-116">How to download password reset registration events quickly with PowerShell</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)

<span data-ttu-id="4c448-117">**أريد فهم المزيد حول قدرات إعادة تعيين التقارير بكلمة مرور**</span><span class="sxs-lookup"><span data-stu-id="4c448-117">**I want to understand more about password reset reporting capabilities**</span></span>

<span data-ttu-id="4c448-118">تحقق من الأشخاص الذين يسجلون كلمات المرور أو يعيدون تعيينها باستخدام Azure AD كلمة مرور إعادة تعيين سجلات التدقيق في مدخل Azure ضمن المستخدمين **والمجموعات.**</span><span class="sxs-lookup"><span data-stu-id="4c448-118">Check who is registering for or resetting passwords with Azure AD password reset audit logs in the Azure portal under **Users and groups**.</span></span>
<span data-ttu-id="4c448-119">لمزيد من المعلومات، راجع الارتباطات التالية:</span><span class="sxs-lookup"><span data-stu-id="4c448-119">For more information, see the following links:</span></span>

- [<span data-ttu-id="4c448-120">نظرة عامة حول إعادة تعيين كلمة المرور للتقارير</span><span class="sxs-lookup"><span data-stu-id="4c448-120">Password reset reports overview</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="4c448-121">كيفية عرض تقارير إعادة تعيين كلمة المرور في مدخل Azure</span><span class="sxs-lookup"><span data-stu-id="4c448-121">How to view password reset reports in the Azure portal</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="4c448-122">إعادة تعيين أحداث كلمة المرور للخدمة الذاتية من Azure AD Reports and Events API</span><span class="sxs-lookup"><span data-stu-id="4c448-122">Self-service password reset events from the Azure AD Reports and Events API</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="4c448-123">كيفية تنزيل أحداث إعادة تعيين تسجيل كلمات المرور بسرعة باستخدام PowerShell</span><span class="sxs-lookup"><span data-stu-id="4c448-123">How to download password reset registration events quickly with PowerShell</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)


