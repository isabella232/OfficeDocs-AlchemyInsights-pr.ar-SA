---
title: مثال على نهج مكافحة التصيد الاحتيالي ل Microsoft Defender ل Office 365
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: eabff70c22b641627d3ab6c0b2f8846a0be2f49e
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/08/2021
ms.locfileid: "50692493"
---
# <a name="example-microsoft-defender-for-office-365-anti-phishing-policy"></a><span data-ttu-id="ce0dc-102">مثال على نهج مكافحة التصيد الاحتيالي ل Microsoft Defender ل Office 365</span><span class="sxs-lookup"><span data-stu-id="ce0dc-102">Example Microsoft Defender for Office 365 anti-phishing policy</span></span>

<span data-ttu-id="ce0dc-103">تمكن هذه الإعدادات نهج يسمى *المجال والمدير التنفيذي.*</span><span class="sxs-lookup"><span data-stu-id="ce0dc-103">These settings enable a policy called *Domain and CEO*.</span></span> <span data-ttu-id="ce0dc-104">يوفر هذا النهج حماية لكل من المستخدم والمجال من انتحال الشخصية، ثم يطبق النهج على كل رسائل البريد الإلكتروني التي يتلقاها المستخدمون ضمن المجال.</span><span class="sxs-lookup"><span data-stu-id="ce0dc-104">This policy provides both user and domain protection from impersonation and then applies the policy to all email received by users within the domain.</span></span> <span data-ttu-id="ce0dc-105">أولا، أضف المعلومات التالية لإنشاء النهج:</span><span class="sxs-lookup"><span data-stu-id="ce0dc-105">First, add the following information to create the policy:</span></span>

- <span data-ttu-id="ce0dc-106">**الاسم**: وصف المجال **والمدير التنفيذي:** يضمن عدم انتحال منصب المدير التنفيذي ومجالك.</span><span class="sxs-lookup"><span data-stu-id="ce0dc-106">**Name**: Domain and CEO **Description**: Ensures that the CEO and your domain are not being impersonated.</span></span>
  <span data-ttu-id="ce0dc-107">**مطبق على:** **تحديد مجال المستلم هو**.</span><span class="sxs-lookup"><span data-stu-id="ce0dc-107">**Applied to**: Select **The recipient domain is**.</span></span> <span data-ttu-id="ce0dc-108">ضمن **أي من هذه،** حدد **"اختيار"،** ثم حدد مجالا.</span><span class="sxs-lookup"><span data-stu-id="ce0dc-108">Under **Any of these**, select **Choose**, and then select a domain.</span></span> <span data-ttu-id="ce0dc-109">حدد **+ إضافة.**</span><span class="sxs-lookup"><span data-stu-id="ce0dc-109">Select **+ Add**.</span></span> <span data-ttu-id="ce0dc-110">حدد خانة الاختيار إلى جانب اسم المجال في القائمة (على سبيل المثال، *contoso.com)،* ثم حدد **"إضافة".**</span><span class="sxs-lookup"><span data-stu-id="ce0dc-110">Select the check box next to the name of the domain in the list (for example, *contoso.com*), and then select **Add**.</span></span> <span data-ttu-id="ce0dc-111">حدد **"تم".**</span><span class="sxs-lookup"><span data-stu-id="ce0dc-111">Select **Done**.</span></span>
- <span data-ttu-id="ce0dc-112">بعد إنشاء النهج، يمكنك ضبط النهج باستخدام الخيارات التالية:</span><span class="sxs-lookup"><span data-stu-id="ce0dc-112">After the policy is created, you can fine-tune the policy by using the following options:</span></span>
  - <span data-ttu-id="ce0dc-113">**إضافة مستخدمين لحمايتها:** في هذا المثال، أضف عنوان البريد الإلكتروني الخاص للمدير التنفيذي، كحد أدنى.</span><span class="sxs-lookup"><span data-stu-id="ce0dc-113">**Add users to protect:** For this example, add the CEO's email address, at a minimum.</span></span>
  - <span data-ttu-id="ce0dc-114">**إضافة مجالات لحمايتها:** أضف مجال المؤسسة الذي يتضمن مكتب المدير التنفيذي.</span><span class="sxs-lookup"><span data-stu-id="ce0dc-114">**Add domains to protect**: Add the organizational domain that includes the office of the CEO.</span></span>
  - <span data-ttu-id="ce0dc-115">**اختر الإجراءات:** إذا تم إرسال البريد الإلكتروني بواسطة مستخدم منتحل، فحدد "إعادة توجيه الرسالة" إلى عنوان بريد إلكتروني آخر، ثم أدخل عنوان البريد الإلكتروني الخاص بمسؤول الأمان (على سبيل المثال،  *securityadmin@contoso.com).*</span><span class="sxs-lookup"><span data-stu-id="ce0dc-115">**Choose actions**: For **If email is sent by an impersonated user**, select **Redirect message to another email address**, and then enter the email address of the security administrator (for example, *securityadmin@contoso.com*).</span></span> <span data-ttu-id="ce0dc-116">إذا **تم إرسال البريد الإلكتروني بواسطة مجال منتحل،** فحدد **"عزل" الرسالة.**</span><span class="sxs-lookup"><span data-stu-id="ce0dc-116">For **If email is sent by an impersonated domain**, select **Quarantine the message**.</span></span>
  - <span data-ttu-id="ce0dc-117">**معلومات علبة** البريد: يتم تحديد هذا الخيار بشكل افتراضي عند إنشاء نهج جديد لمكافحة التصيد الاحتيالي.</span><span class="sxs-lookup"><span data-stu-id="ce0dc-117">**Mailbox intelligence**: By default, this option is selected when you create a new anti-phishing policy.</span></span> <span data-ttu-id="ce0dc-118">اترك هذا الإعداد **في وضع "العمل"** للحصول على أفضل النتائج.</span><span class="sxs-lookup"><span data-stu-id="ce0dc-118">Leave this setting **On** for best results.</span></span>
  - <span data-ttu-id="ce0dc-119">**إضافة مرسلين ومجالات موثوق بها:** في هذا المثال، لا تحدد أي تجاوزات.</span><span class="sxs-lookup"><span data-stu-id="ce0dc-119">**Add trusted senders and domains:** For this example, don't define any overrides.</span></span>
- <span data-ttu-id="ce0dc-120">بعد مراجعة الإعدادات، حدد **"إنشاء هذا النهج"** أو **"حفظ"،** حسب الاقتضاء.</span><span class="sxs-lookup"><span data-stu-id="ce0dc-120">Once you've reviewed your settings, select **Create this policy** or **Save**, as appropriate.</span></span>

<span data-ttu-id="ce0dc-121">لمعرفة المزيد، راجع سياسات مكافحة [التصيد الاحتيالي في Microsoft 365.](https://go.microsoft.com/fwlink/?linkid=2092235)</span><span class="sxs-lookup"><span data-stu-id="ce0dc-121">To learn more, see [Anti-phishing policies in Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2092235).</span></span>
