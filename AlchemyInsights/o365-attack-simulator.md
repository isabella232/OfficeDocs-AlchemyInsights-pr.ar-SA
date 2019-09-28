---
title: 2681 محاكاة الهجوم في مكتب 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: 07d7622c00074f7bd0d567185824db448f1eeef3
ms.sourcegitcommit: 7232b48bcd8bb9867d52a2f055a46ce76a58b8da
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/27/2019
ms.locfileid: "37305319"
---
# <a name="attack-simulator-in-office-365"></a><span data-ttu-id="009bf-102">هجوم محاكي في مكتب 365</span><span class="sxs-lookup"><span data-stu-id="009bf-102">Attack Simulator in Office 365</span></span>

- <span data-ttu-id="009bf-103">هل أنت في عداد المفقودين محاكي الهجوم ؟</span><span class="sxs-lookup"><span data-stu-id="009bf-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="009bf-104">هجوم محاكي يتطلب **مكتب 365 متقدمة التهديد خطه الحماية 2 (ATP خطه 2)** أو **مكتب 365 المؤسسة E5**.</span><span class="sxs-lookup"><span data-stu-id="009bf-104">Attack Simulator requires **Office 365 Advanced Threat Protection Plan 2 (ATP Plan 2)** or **Office 365 Enterprise E5**.</span></span> <span data-ttu-id="009bf-105">**لا** يتم تضمين محاكي الهجوم في office 365 المتقدمة خطه حماية التهديد 1 (ATP خطه 1) ، مكتب 365 المؤسسة E3 ، أو اي مكتب 365 الاشتراكات التجارية.</span><span class="sxs-lookup"><span data-stu-id="009bf-105">Attack Simulator is **not** included in Office 365 Advanced Threat Protection Plan 1 (ATP Plan 1), Office 365 Enterprise E3, or any Office 365 Business subscriptions.</span></span>

- <span data-ttu-id="009bf-106">يتطلب الحساب الذي تستخدمه لتشغيل الهجمات المحاكية المسؤول العمومي أو أذونات مسؤول الأمان والمصادقة متعددة العوامل (وزاره الخارجية).</span><span class="sxs-lookup"><span data-stu-id="009bf-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="009bf-107">لمزيد من المعلومات حول متطلبات محاكي الهجوم ، راجع [هذا الموضوع](https://docs.microsoft.com/office365/securitycompliance/attack-simulator#before-you-begin).</span><span class="sxs-lookup"><span data-stu-id="009bf-107">For more information about Attack Simulator requirements, see [this topic](https://docs.microsoft.com/office365/securitycompliance/attack-simulator#before-you-begin).</span></span>

- <span data-ttu-id="009bf-108">الأشياء الهامه التي يجب معرفتها عن محاكاة الهجوم **الغاشمة القوه كلمه المرور** :</span><span class="sxs-lookup"><span data-stu-id="009bf-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="009bf-109">إذا كان الحساب الهدف لديه تمكين وزاره الخارجية وخمنت كلمه المرور بشكل صحيح ، لن تظهر الحساب كما للخطر (سيكون عامل المصادقة الثاني غير مكتملة).</span><span class="sxs-lookup"><span data-stu-id="009bf-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="009bf-110">لا يمكن ان يكون ملف كلمه المرور أكبر من 10 ميغابايت.</span><span class="sxs-lookup"><span data-stu-id="009bf-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="009bf-111">استخدم كلمه مرور واحده لكل سطر ، وتضمين سطر فارغ (إرجاع الحرف) بعد كلمه المرور الاخيره في القائمة.</span><span class="sxs-lookup"><span data-stu-id="009bf-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="009bf-112">الأشياء الهامه التي يجب معرفتها حول **الخداع الرمح** إرفاق المحاكاة:</span><span class="sxs-lookup"><span data-stu-id="009bf-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="009bf-113">حسب التصميم ، لا يمكنك توفير قيمه مخصصه **لعنوان URL لخادم تسجيل الدخول الاحتيالي**.</span><span class="sxs-lookup"><span data-stu-id="009bf-113">By design, you can't provide a custom value for **Phishing login server URL**.</span></span>

  - <span data-ttu-id="009bf-114">إذا كان المستلم يستخدم [تمكين الوظيفة الاضافيه "رسالة التقرير](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) " للإبلاغ عن الرسالة كتصيد احتيالي ، قد لا تتلقي تنبيات للرسالة (لان هذا هو هجوم محاكاة).</span><span class="sxs-lookup"><span data-stu-id="009bf-114">If a recipient uses the [Enable the Report Message add-in](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="009bf-115">التقارير: بعد اكتمال الهجوم المحاكي ، يمكنك النقر فوق **تفاصيل الهجوم** لمشاهده التقرير.</span><span class="sxs-lookup"><span data-stu-id="009bf-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="009bf-116">للحصول علي تعليمات مفصله وميزات جديده في هجوم محاكي ، انظر [هجوم محاكي في مكتب 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="009bf-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>
