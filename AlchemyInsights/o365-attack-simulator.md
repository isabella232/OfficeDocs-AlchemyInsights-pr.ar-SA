---
title: 2681 هجوم محاكي في مايكروسوفت 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: 3dae4768ca62757ce7f92dfc527078c963d72742
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506725"
---
# <a name="attack-simulator-in-microsoft-365"></a><span data-ttu-id="4ad85-102">محاكاة الهجوم في مايكروسوفت 365</span><span class="sxs-lookup"><span data-stu-id="4ad85-102">Attack Simulator in Microsoft 365</span></span>

- <span data-ttu-id="4ad85-103">هل تفتقد محاكي الهجوم؟</span><span class="sxs-lookup"><span data-stu-id="4ad85-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="4ad85-104">يتطلب محاكي الهجوم **Office 365 خطة متقدمة للحماية من التهديدات 2 (خطة ATP 2)** أو **Office 365 Enterprise E5**.</span><span class="sxs-lookup"><span data-stu-id="4ad85-104">Attack Simulator requires **Office 365 Advanced Threat Protection Plan 2 (ATP Plan 2)** or **Office 365 Enterprise E5**.</span></span> <span data-ttu-id="4ad85-105">**لا** يتم تضمين محاكي الهجوم في Office 365 خطة الحماية المتقدمة من التهديدات 1 (خطة ATP 1) أو Office 365 Enterprise E3 أو أي تطبيقات Microsoft 365 لاشتراكات الأعمال.</span><span class="sxs-lookup"><span data-stu-id="4ad85-105">Attack Simulator is **not** included in Office 365 Advanced Threat Protection Plan 1 (ATP Plan 1), Office 365 Enterprise E3, or any Microsoft 365 Apps for business subscriptions.</span></span>

- <span data-ttu-id="4ad85-106">يتطلب الحساب الذي تستخدمه لإطلاق هجمات محاكاة أذونات المسؤول أو مسؤول الأمان العمومية والمصادقة متعددة العوامل (MFA).</span><span class="sxs-lookup"><span data-stu-id="4ad85-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="4ad85-107">لمزيد من المعلومات حول متطلبات محاكي الهجوم، راجع [هذا الموضوع](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="4ad85-107">For more information about Attack Simulator requirements, see [this topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>

- <span data-ttu-id="4ad85-108">أشياء هامة لمعرفة عن محاكاة هجوم **كلمة مرور القوة الغاشمة:**</span><span class="sxs-lookup"><span data-stu-id="4ad85-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="4ad85-109">إذا تم تمكين حساب الهدف MFA وتم تخمين كلمة المرور بشكل صحيح، فلن يظهر الحساب كما تم اختراقه (سيكون عامل المصادقة الثاني غير مكتمل).</span><span class="sxs-lookup"><span data-stu-id="4ad85-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="4ad85-110">لا يمكن أن يكون ملف كلمة المرور أكبر من 10 ميغابايت.</span><span class="sxs-lookup"><span data-stu-id="4ad85-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="4ad85-111">استخدم كلمة مرور واحدة لكل سطر، وتضمين سطر فارغ (إرجاع النقل) بعد كلمة المرور الأخيرة في القائمة.</span><span class="sxs-lookup"><span data-stu-id="4ad85-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="4ad85-112">أشياء هامة يجب معرفتها عن محاكاة **ربط التصيد الاحتيالي بالرمح:**</span><span class="sxs-lookup"><span data-stu-id="4ad85-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="4ad85-113">حسب التصميم، لا يمكنك توفير قيمة مخصصة **لعنوان URL لخادم تسجيل الدخول التصيدي**.</span><span class="sxs-lookup"><span data-stu-id="4ad85-113">By design, you can't provide a custom value for **Phishing login server URL**.</span></span>

  - <span data-ttu-id="4ad85-114">إذا استخدم المستلم [الوظيفة الإضافية تمكين رسالة التقرير](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) للإبلاغ عن الرسالة كخداع، فقد لا تتلقى تنبيهات للرسالة (لأن هذا هجوم محاكاة).</span><span class="sxs-lookup"><span data-stu-id="4ad85-114">If a recipient uses the [Enable the Report Message add-in](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="4ad85-115">التقارير: بعد اكتمال الهجوم المحاكي، يمكنك النقر فوق **تفاصيل الهجوم** لمشاهدة التقرير.</span><span class="sxs-lookup"><span data-stu-id="4ad85-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="4ad85-116">للحصول على إرشادات مفصلة وميزات جديدة في محاكي الهجوم، راجع [محاكي الهجوم في Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="4ad85-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>
