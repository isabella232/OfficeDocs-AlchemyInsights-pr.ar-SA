---
title: تمكين مصادقة SMTP وإصلاحها
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "5652"
ms.openlocfilehash: 4695a2f111823739c4d87fa2b262a5e64e080955
ms.sourcegitcommit: 2103d706492ad7ee9596344714c0520569ebd6af
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/23/2021
ms.locfileid: "53077638"
---
# <a name="enable-smtp-authentication-and-troubleshooting"></a><span data-ttu-id="44498-102">تمكين مصادقة SMTP وإصلاحها</span><span class="sxs-lookup"><span data-stu-id="44498-102">Enable SMTP authentication and troubleshooting</span></span>

<span data-ttu-id="44498-103">إذا كنت تريد تمكين مصادقة SMTP لعلبة بريد أو إذا كنت تحصل على رسالة الخطأ "العميل غير مصدق عليه" أو "المصادقة غير ناجحة" أو "SmtpClientAuthentication" مع الرمز 5.7.57 أو 5.7.3 أو 5.7.139 عند محاولة ترحيل البريد الإلكتروني عن طريق مصادقة جهاز أو تطبيق باستخدام Microsoft 365، يمكنك تنفيذ هذه الإجراءات الثلاثة لحل المشكلة:</span><span class="sxs-lookup"><span data-stu-id="44498-103">If you want to enable SMTP authentication for a mailbox or you're getting a "Client not authenticated", "Authentication unsuccessful", or "SmtpClientAuthentication" error with code 5.7.57 or 5.7.3 or 5.7.139 when you try to relay email by authenticating a device or application with Microsoft 365, perform these three actions to resolve the issue:</span></span>

1. <span data-ttu-id="44498-104">قم [بتعطيل إعدادات أمان Azure الافتراضية](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) عن طريق تبديل **تمكين إعدادات الأمان الافتراضية** إلى **لا**.</span><span class="sxs-lookup"><span data-stu-id="44498-104">Disable the [Azure security defaults](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) by toggling **Enable security defaults** to **No**.</span></span>

    <span data-ttu-id="44498-105">أ.</span><span class="sxs-lookup"><span data-stu-id="44498-105">a.</span></span> <span data-ttu-id="44498-106">سجل دخولك إلى مدخل Azure كمسؤول أمان أو مسؤول وصول شرطي أو مسؤول عام.</span><span class="sxs-lookup"><span data-stu-id="44498-106">Sign in to the Azure portal as a Security administrator, Conditional Access administrator, or global administrator.</span></span><BR/>
    <span data-ttu-id="44498-107">ب.</span><span class="sxs-lookup"><span data-stu-id="44498-107">b.</span></span> <span data-ttu-id="44498-108">استعرض إلى Azure Active Directory > **خصائص .**</span><span class="sxs-lookup"><span data-stu-id="44498-108">Browse to Azure Active Directory > **Properties**.</span></span><BR/>
    <span data-ttu-id="44498-109">ج.</span><span class="sxs-lookup"><span data-stu-id="44498-109">c.</span></span> <span data-ttu-id="44498-110">حدد **إدارة إعدادات الأمان الافتراضية**.</span><span class="sxs-lookup"><span data-stu-id="44498-110">Select **Manage security defaults**.</span></span><BR/>
    <span data-ttu-id="44498-111">د.</span><span class="sxs-lookup"><span data-stu-id="44498-111">d.</span></span> <span data-ttu-id="44498-112">تعيين **تمكين إعدادات الأمان الافتراضية** إلى **لا**.</span><span class="sxs-lookup"><span data-stu-id="44498-112">Set **Enable security defaults** to **No**.</span></span><BR/>
    <span data-ttu-id="44498-113">ه.</span><span class="sxs-lookup"><span data-stu-id="44498-113">e.</span></span> <span data-ttu-id="44498-114">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="44498-114">Select **Save**.</span></span>

2. <span data-ttu-id="44498-115">[تمكين إرسال SMTP للعميل](/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) على علبة البريد المرخصة.</span><span class="sxs-lookup"><span data-stu-id="44498-115">[Enable Client SMTP submission](/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) on the licensed mailbox.</span></span>

    <span data-ttu-id="44498-116">أ.</span><span class="sxs-lookup"><span data-stu-id="44498-116">a.</span></span> <span data-ttu-id="44498-117">من مركز مسؤولي Microsoft 365، انتقل إلى **المستخدمون النشطون**، وحدد المستخدم.</span><span class="sxs-lookup"><span data-stu-id="44498-117">From the Microsoft 365 admin center, go to **Active Users**, and select the user.</span></span><BR/>
    <span data-ttu-id="44498-118">ب.</span><span class="sxs-lookup"><span data-stu-id="44498-118">b.</span></span> <span data-ttu-id="44498-119">انتقل إلى علامة التبويب البريد، و ضمن **تطبيقات البريد الإلكتروني،** حدد **إدارة تطبيقات البريد الإلكتروني**.</span><span class="sxs-lookup"><span data-stu-id="44498-119">Go to Mail tab, and under **Email apps**, select **Manage email apps**.</span></span><BR/>
    <span data-ttu-id="44498-120">د.</span><span class="sxs-lookup"><span data-stu-id="44498-120">d.</span></span> <span data-ttu-id="44498-121">تأكد من **أن SMTP المصادق** عليه محدد (تم تمكينه).</span><span class="sxs-lookup"><span data-stu-id="44498-121">Make sure **Authenticated SMTP** is checked (enabled).</span></span><BR/>
    <span data-ttu-id="44498-122">ه.</span><span class="sxs-lookup"><span data-stu-id="44498-122">e.</span></span> <span data-ttu-id="44498-123">حدد **حفظ التغييرات**.</span><span class="sxs-lookup"><span data-stu-id="44498-123">Select **Save changes**.</span></span><BR/>

3. <span data-ttu-id="44498-124">[قم بتعطيل المصادقة متعددة العوامل (MFA)](/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa) على علبة البريد المرخصة.</span><span class="sxs-lookup"><span data-stu-id="44498-124">[Disable Multi-Factor Authentication (MFA)](/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa) on the licensed mailbox.</span></span>

    <span data-ttu-id="44498-125">أ.</span><span class="sxs-lookup"><span data-stu-id="44498-125">a.</span></span> <span data-ttu-id="44498-126">انتقل إلى مركز مسؤولي Microsoft 365، وفي قائمة التنقل اليسرى حدد  >  **المستخدمون المستخدمون النشطون**.</span><span class="sxs-lookup"><span data-stu-id="44498-126">Go to the Microsoft 365 admin center, and in the left navigation menu select **Users** > **Active users**.</span></span><BR/>
    <span data-ttu-id="44498-127">ب.</span><span class="sxs-lookup"><span data-stu-id="44498-127">b.</span></span> <span data-ttu-id="44498-128">حدد **المصادقة متعددة العوامل**.</span><span class="sxs-lookup"><span data-stu-id="44498-128">Select **Multi-factor authentication**.</span></span><BR/>
    <span data-ttu-id="44498-129">ج.</span><span class="sxs-lookup"><span data-stu-id="44498-129">c.</span></span> <span data-ttu-id="44498-130">حدد المستخدم وعطل **وثة متعددة العوامل**.</span><span class="sxs-lookup"><span data-stu-id="44498-130">Select the user and disable **Multi-Factor auth**.</span></span><BR/>
