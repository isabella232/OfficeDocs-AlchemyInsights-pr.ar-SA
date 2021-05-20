---
title: 2681 Attack Simulator في Microsoft 365
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
ms.openlocfilehash: e7d71fdb77b4a047c1998e9aba75cdd469a936a8
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/19/2021
ms.locfileid: "52545713"
---
# <a name="attack-simulator-in-microsoft-365"></a><span data-ttu-id="5ec10-102">محاكي الهجوم في Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="5ec10-102">Attack Simulator in Microsoft 365</span></span>

- <span data-ttu-id="5ec10-103">هل تفتقد "محاكي الهجوم"؟</span><span class="sxs-lookup"><span data-stu-id="5ec10-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="5ec10-104">يتطلب محاكي الهجوم **وجود Microsoft Defender Office 365 2** أو Office 365 Enterprise **E5**.</span><span class="sxs-lookup"><span data-stu-id="5ec10-104">Attack Simulator requires **Microsoft Defender for Office 365 Plan 2** or **Office 365 Enterprise E5**.</span></span> <span data-ttu-id="5ec10-105">لا يتم **تضمين** محاكي الهجوم في Microsoft Defender Office 365 1 أو Office 365 Enterprise E3 أو أي اشتراكات Microsoft 365 Apps for business اشتراكات.</span><span class="sxs-lookup"><span data-stu-id="5ec10-105">Attack Simulator is **not** included in Microsoft Defender for Office 365 Plan 1, Office 365 Enterprise E3, or any Microsoft 365 Apps for business subscriptions.</span></span>

- <span data-ttu-id="5ec10-106">يتطلب الحساب الذي تستخدمه لشن هجمات محاكاة أذونات المسؤول العام أو مسؤول الأمان والمصادقة متعددة العوامل (MFA).</span><span class="sxs-lookup"><span data-stu-id="5ec10-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="5ec10-107">لمزيد من المعلومات حول متطلبات "محاكي الهجمات"، راجع [هذا الموضوع](/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="5ec10-107">For more information about Attack Simulator requirements, see [this topic](/microsoft-365/security/office-365-security/attack-simulator).</span></span>

- <span data-ttu-id="5ec10-108">أشياء مهمة يجب معرفتها حول عمليات محاكاة هجوم **"القوة الغاشمة لكلمة** المرور":</span><span class="sxs-lookup"><span data-stu-id="5ec10-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="5ec10-109">إذا تم تمكين المصادقة MFA للحساب الهدف وكان تخمين كلمة المرور صحيحا، لن يظهر الحساب كمعرض للخطر (سيكون عامل المصادقة الثاني غير مكتمل).</span><span class="sxs-lookup"><span data-stu-id="5ec10-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="5ec10-110">لا يمكن أن يزيد حجم ملف كلمة المرور عن 10 مبايت.</span><span class="sxs-lookup"><span data-stu-id="5ec10-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="5ec10-111">استخدم كلمة مرور واحدة لكل سطر، ثم قم بتضمين سطر فارغ (إرجاع السطر) بعد كلمة المرور الأخيرة في القائمة.</span><span class="sxs-lookup"><span data-stu-id="5ec10-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="5ec10-112">أشياء مهمة يجب معرفتها حول عمليات محاكاة **"التصيد الاحتيالي من أجل** التصيد الاحتيالي":</span><span class="sxs-lookup"><span data-stu-id="5ec10-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="5ec10-113">حسب التصميم، لا يمكنك توفير قيمة مخصصة ل URL خادم تسجيل الدخول إلى التصيد **الاحتيالي**.</span><span class="sxs-lookup"><span data-stu-id="5ec10-113">By design, you can't provide a custom value for **Phishing login server URL**.</span></span>

  - <span data-ttu-id="5ec10-114">إذا استخدم المستلم [](/microsoft-365/security/office-365-security/enable-the-report-message-add-in) الميزة الإضافية تمكين رسالة التقرير للتقارير حول الرسالة على أنها تصيد احتيالي، فقد لا تتلقى تنبيهات للرسالة (لأن هذا هجوم محاكاة).</span><span class="sxs-lookup"><span data-stu-id="5ec10-114">If a recipient uses the [Enable the Report Message add-in](/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="5ec10-115">التقارير: بعد اكتمال الهجوم المحاكاة، يمكنك النقر **فوق** تفاصيل الهجوم لرؤية التقرير.</span><span class="sxs-lookup"><span data-stu-id="5ec10-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="5ec10-116">للحصول على إرشادات مفصلة وميزات جديدة في "محاكي الهجوم"، راجع [محاكي](/microsoft-365/security/office-365-security/attack-simulator)الهجوم في Microsoft 365 .</span><span class="sxs-lookup"><span data-stu-id="5ec10-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Microsoft 365](/microsoft-365/security/office-365-security/attack-simulator).</span></span>
