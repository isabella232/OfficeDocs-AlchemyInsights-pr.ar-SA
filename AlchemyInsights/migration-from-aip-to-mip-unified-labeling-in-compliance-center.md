---
title: الترحيل من AIP إلى MIP /وضع العلامات الموحدة في مركز الامتثال
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5114"
ms.openlocfilehash: 7ce9c387fc94f59674a922c5fe071fc0fb030344
ms.sourcegitcommit: e6d73d240669342fde9d4d25b0ee2838b7e43965
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/14/2020
ms.locfileid: "44236294"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a><span data-ttu-id="4ef66-102">الترحيل من AIP إلى MIP /وضع العلامات الموحدة في مركز الامتثال</span><span class="sxs-lookup"><span data-stu-id="4ef66-102">Migration from AIP to MIP/Unified Labeling in the Compliance Center</span></span>

<span data-ttu-id="4ef66-103">للترحيل من تسميات AIP إلى وضع العلامات الموحدة في مركز الأمان والامتثال، قم بما يلي:</span><span class="sxs-lookup"><span data-stu-id="4ef66-103">To migrate from AIP labels to Unified Labeling in the Security and Compliance center, do the following:</span></span>

<span data-ttu-id="4ef66-104">**تفعيل الحماية من بوابة Azure**</span><span class="sxs-lookup"><span data-stu-id="4ef66-104">**Activate protection from the Azure portal**</span></span>

1. <span data-ttu-id="4ef66-105">إذا لم تكن قد فعلت ذلك بالفعل، افتح نافذة متصفح جديدة [وسجّل الدخول إلى بوابة Azure](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal).</span><span class="sxs-lookup"><span data-stu-id="4ef66-105">If you haven't already done so, open a new browser window and [sign in to the Azure portal](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal).</span></span> <span data-ttu-id="4ef66-106">انتقل إلى شفرة **حماية المعلومات Azure.**</span><span class="sxs-lookup"><span data-stu-id="4ef66-106">Navigate to the **Azure Information Protection** blade.</span></span> <span data-ttu-id="4ef66-107">على سبيل المثال، في قائمة لوحة الوصل، انقر فوق **كافة الخدمات** وابدأ في كتابة **المعلومات** في مربع عامل التصفية.</span><span class="sxs-lookup"><span data-stu-id="4ef66-107">For example, on the hub menu, click **All services** and start typing **Information** in the Filter box.</span></span> <span data-ttu-id="4ef66-108">حدد **حماية معلومات Azure**.</span><span class="sxs-lookup"><span data-stu-id="4ef66-108">Select **Azure Information Protection**.</span></span> <span data-ttu-id="4ef66-109">إذا لم تكن قد قمت بالوصول إلى شفرة حماية المعلومات Azure من قبل، فراجع [الخطوات الإضافية](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) لمرة واحدة لإضافة هذا النصل إلى المدخل.</span><span class="sxs-lookup"><span data-stu-id="4ef66-109">If you haven't accessed the Azure Information Protection blade before, see the one-time [additional steps](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) to add this blade to the portal.</span></span> <span data-ttu-id="4ef66-110">لفتح شفرة حماية المعلومات Azure، يجب أن يكون لديك [إما خطة Azure لحماية المعلومات أو](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) خطة Office 365 التي تتضمن إدارة الحقوق.</span><span class="sxs-lookup"><span data-stu-id="4ef66-110">To open the Azure Information Protection blade, you must have either an [Azure Information Protection Premium plan](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) or an Office 365 plan that includes Rights Management.</span></span> <span data-ttu-id="4ef66-111">إذا كان لديك أحد هذه الاشتراكات ولكن راجع رسالة تفيد بأنه لا يمكن العثور على اشتراك صالح، [فاتصل بدعم Microsoft](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) أو استخدم قنوات الدعم القياسية.</span><span class="sxs-lookup"><span data-stu-id="4ef66-111">If you have one of these subscriptions but see a message that a valid subscription cannot be found, [contact Microsoft Support](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) or use your standard support channels.</span></span>

2. <span data-ttu-id="4ef66-112">تحديد موقع خيارات القائمة **إدارة،** وحدد **تنشيط الحماية**.</span><span class="sxs-lookup"><span data-stu-id="4ef66-112">Locate the **Manage** menu options, and select **Protection activation**.</span></span> <span data-ttu-id="4ef66-113">انقر فوق **تنشيط**، ثم تأكيد الإجراء الخاص بك.</span><span class="sxs-lookup"><span data-stu-id="4ef66-113">Click **Activate**, and then confirm your action.</span></span> <span data-ttu-id="4ef66-114">عند اكتمال التنشيط، يعرض شريط المعلومات **التنشيط الذي تم الانتهاء منه بنجاح**.</span><span class="sxs-lookup"><span data-stu-id="4ef66-114">When activation is complete, the information bar displays **Activation finished successfully**.</span></span>

<span data-ttu-id="4ef66-115">**ترحيل تسميات حماية معلومات Azure إلى مركز التوافق & الأمان في Office 365**</span><span class="sxs-lookup"><span data-stu-id="4ef66-115">**Migrate Azure Information Protection labels to Office 365 Security & Compliance Center**</span></span>

1. <span data-ttu-id="4ef66-116">تأكد من تسجيل الدخول كمستخدم بإذن المسؤول العمومي.</span><span class="sxs-lookup"><span data-stu-id="4ef66-116">Make sure you are logged in as a user with Global Administrator permission.</span></span>

2. <span data-ttu-id="4ef66-117">انتقل إلى شفرة **حماية المعلومات Azure.**</span><span class="sxs-lookup"><span data-stu-id="4ef66-117">Navigate to the **Azure Information Protection** blade.</span></span>

3. <span data-ttu-id="4ef66-118">من خيار **إدارة** القائمة، حدد **وضع العلامات الموحدة**.</span><span class="sxs-lookup"><span data-stu-id="4ef66-118">From the **Manage** menu option, select **Unified labeling**.</span></span>

4. <span data-ttu-id="4ef66-119">على حماية المعلومات Azure - شفرة **وضع العلامات الموحدة،** انقر فوق **تنشيط** واتبع الإرشادات عبر الإنترنت.</span><span class="sxs-lookup"><span data-stu-id="4ef66-119">On the **Azure Information Protection - Unified labeling** blade, click **Activate** and follow the online instructions.</span></span>

<span data-ttu-id="4ef66-120">**ملاحظة:** تحقق من أن لديك الأذونات المناسبة قبل تنشيط ترحيل مركز التوافق & الأمان.</span><span class="sxs-lookup"><span data-stu-id="4ef66-120">**Note**: Verify that you have the appropriate permissions before activating the Security & Compliance Center Migration.</span></span> <span data-ttu-id="4ef66-121">راجع هذه المقالات لمزيد من المعلومات:</span><span class="sxs-lookup"><span data-stu-id="4ef66-121">See these articles for more info:</span></span>

1. [<span data-ttu-id="4ef66-122">هل تحتاج إلى أن تكون مسؤولًا عالميًا لتكوين حماية معلومات Azure، أم يمكنني التفويض إلى مسؤولين آخرين؟</span><span class="sxs-lookup"><span data-stu-id="4ef66-122">Do you need to be a global admin to configure Azure Information Protection, or can I delegate to other administrators?</span></span>](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [<span data-ttu-id="4ef66-123">معلومات هامة حول الأدوار الإدارية بعد الترحيل إلى مركز التوافق & الأمان.</span><span class="sxs-lookup"><span data-stu-id="4ef66-123">Important information about administrative roles after migrating to Security & Compliance Center.</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

<span data-ttu-id="4ef66-124">لمزيد من المعلومات حول ترحيل AIP إلى وضع العلامات الموحدة إلى مركز الأمان والامتثال، راجع [ترحيل التسميات](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).</span><span class="sxs-lookup"><span data-stu-id="4ef66-124">For more information on the AIP to Unified Labeling migration to Security and Compliance Center, see [Migrate labels](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).</span></span>
