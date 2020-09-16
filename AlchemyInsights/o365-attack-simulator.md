---
title: محاكي الهجوم في 2681 في Microsoft 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: dec96238c8438dcf9df176e3e3f20bd8a985b2cc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47759206"
---
# <a name="attack-simulator-in-microsoft-365"></a><span data-ttu-id="f1e62-102">محاكي الهجوم في Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="f1e62-102">Attack Simulator in Microsoft 365</span></span>

- <span data-ttu-id="f1e62-103">هل أنت تفتقد إلى محاكي الهجوم ؟</span><span class="sxs-lookup"><span data-stu-id="f1e62-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="f1e62-104">المحاكي يتطلب **الحماية من المخاطر المتقدمة في office 365 (خطه ATP 2)** أو **Office 365 Enterprise E5**.</span><span class="sxs-lookup"><span data-stu-id="f1e62-104">Attack Simulator requires **Office 365 Advanced Threat Protection Plan 2 (ATP Plan 2)** or **Office 365 Enterprise E5**.</span></span> <span data-ttu-id="f1e62-105">**لم** يتم تضمين محاكي الهجوم في خطه الحماية المتقدمة من المخاطر في Office 365 (خطه ATP 1) أو Office 365 Enterprise E3 أو اي تطبيقات Microsoft 365 للاشتراكات التجارية.</span><span class="sxs-lookup"><span data-stu-id="f1e62-105">Attack Simulator is **not** included in Office 365 Advanced Threat Protection Plan 1 (ATP Plan 1), Office 365 Enterprise E3, or any Microsoft 365 Apps for business subscriptions.</span></span>

- <span data-ttu-id="f1e62-106">يتطلب الحساب الذي تستخدمه لبدء الهجمات المحاكية أذونات المسؤول العام أو مسؤول الأمان ومصادقه متعددة العوامل (MFA).</span><span class="sxs-lookup"><span data-stu-id="f1e62-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="f1e62-107">لمزيد من المعلومات حول متطلبات محاكي الهجوم ، راجع [هذا الموضوع](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="f1e62-107">For more information about Attack Simulator requirements, see [this topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>

- <span data-ttu-id="f1e62-108">الأمور الهامه التي يجب معرفتها حول عمليات محاكاة هجوم **كلمه المرور بروتي**</span><span class="sxs-lookup"><span data-stu-id="f1e62-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="f1e62-109">إذا كان الحساب الهدف تم تمكين MFA عليه وكانت كلمه المرور جويسيده بشكل صحيح ، فلن يظهر الحساب كتم اختراقه (سيكتمل عامل المصادقة الثاني).</span><span class="sxs-lookup"><span data-stu-id="f1e62-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="f1e62-110">لا يمكن ان يكون ملف كلمه المرور أكبر من 10 ميغابايت.</span><span class="sxs-lookup"><span data-stu-id="f1e62-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="f1e62-111">استخدم كلمه مرور واحده لكل سطر ، وقم بتضمين سطر فارغ (حرف إرجاع) بعد كلمه المرور الاخيره في القائمة.</span><span class="sxs-lookup"><span data-stu-id="f1e62-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="f1e62-112">الأمور الهامه التي يجب معرفتها حول عمليات محاكاة **الشبير في التصيد الاحتيالي** :</span><span class="sxs-lookup"><span data-stu-id="f1e62-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="f1e62-113">بحسب التصميم ، لا يمكنك توفير قيمه مخصصه **لعنوان URL لخادم تسجيل الدخول إلى التصيد الاحتيالي**.</span><span class="sxs-lookup"><span data-stu-id="f1e62-113">By design, you can't provide a custom value for **Phishing login server URL**.</span></span>

  - <span data-ttu-id="f1e62-114">إذا كان أحد المستلمين يستخدم [الوظيفة الاضافيه الخاصة برسائل التقرير](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) للإبلاغ عن الرسالة كتصيد احتيالي ، فقد لا تتلقي تنبيات للرسالة (لان هذا الهجوم تمت محاكاته).</span><span class="sxs-lookup"><span data-stu-id="f1e62-114">If a recipient uses the [Enable the Report Message add-in](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="f1e62-115">التقارير: بعد اكتمال الهجوم الذي تمت محاكاته ، يمكنك النقر فوق **تفاصيل الهجوم** لعرض التقرير.</span><span class="sxs-lookup"><span data-stu-id="f1e62-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="f1e62-116">للحصول علي الإرشادات التفصيلية والميزات الجديدة في محاكي الهجوم ، راجع [محاكي الهجوم في Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="f1e62-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>
