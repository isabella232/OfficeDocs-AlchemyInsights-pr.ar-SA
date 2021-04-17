---
title: الترحيل من AIP إلى تسمية MIP/الموحدة في مركز التوافق
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
- "9002278"
- "5114"
ms.openlocfilehash: 12f5f5c46edd7918618c55a8a1905f3b28643092
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825358"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a><span data-ttu-id="a719f-102">الترحيل من AIP إلى تسمية MIP/الموحدة في مركز التوافق</span><span class="sxs-lookup"><span data-stu-id="a719f-102">Migration from AIP to MIP/Unified Labeling in the Compliance Center</span></span>

<span data-ttu-id="a719f-103">للترحيل من تسميات AIP إلى التسمية الموحدة في مركز الأمان والتوافق، يمكنك القيام بما يلي:</span><span class="sxs-lookup"><span data-stu-id="a719f-103">To migrate from AIP labels to Unified Labeling in the Security and Compliance center, do the following:</span></span>

<span data-ttu-id="a719f-104">**تنشيط الحماية من مدخل Azure**</span><span class="sxs-lookup"><span data-stu-id="a719f-104">**Activate protection from the Azure portal**</span></span>

1. <span data-ttu-id="a719f-105">إذا لم تكن قد فعلت ذلك بعد، فافتح نافذة مستعرض جديدة ثم [سجل الدخول إلى مدخل Azure](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal).</span><span class="sxs-lookup"><span data-stu-id="a719f-105">If you haven't already done so, open a new browser window and [sign in to the Azure portal](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal).</span></span> <span data-ttu-id="a719f-106">انتقل إلى **شفرة Azure Information Protection.**</span><span class="sxs-lookup"><span data-stu-id="a719f-106">Navigate to the **Azure Information Protection** blade.</span></span> <span data-ttu-id="a719f-107">على سبيل المثال، في قائمة الموزع، انقر فوق **كافة الخدمات** وابدأ بكتابة **المعلومات** في المربع عامل التصفية.</span><span class="sxs-lookup"><span data-stu-id="a719f-107">For example, on the hub menu, click **All services** and start typing **Information** in the Filter box.</span></span> <span data-ttu-id="a719f-108">حدد **Azure Information Protection**.</span><span class="sxs-lookup"><span data-stu-id="a719f-108">Select **Azure Information Protection**.</span></span> <span data-ttu-id="a719f-109">إذا لم تكن قد قمت بالوصول إلى شفرة Azure Information [](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) Protection من قبل، فشاهد الخطوات الإضافية مرة واحدة لإضافة هذا النصل إلى المدخل.</span><span class="sxs-lookup"><span data-stu-id="a719f-109">If you haven't accessed the Azure Information Protection blade before, see the one-time [additional steps](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) to add this blade to the portal.</span></span> <span data-ttu-id="a719f-110">لفتح شفرة Azure Information Protection، يجب أن يكون لديك خطة [Azure Information Protection Premium](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) أو خطة Office 365 التي تتضمن إدارة الحقوق.</span><span class="sxs-lookup"><span data-stu-id="a719f-110">To open the Azure Information Protection blade, you must have either an [Azure Information Protection Premium plan](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) or an Office 365 plan that includes Rights Management.</span></span> <span data-ttu-id="a719f-111">إذا كان لديك أحد هذه الاشتراكات ولكنك رأيت رسالة بأنه يتعذر العثور على اشتراك صالح، فاتصل ب [دعم Microsoft](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) أو استخدم قنوات الدعم القياسية.</span><span class="sxs-lookup"><span data-stu-id="a719f-111">If you have one of these subscriptions but see a message that a valid subscription cannot be found, [contact Microsoft Support](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) or use your standard support channels.</span></span>

2. <span data-ttu-id="a719f-112">حدد خيارات **القائمة إدارة،** وحدد **تنشيط الحماية**.</span><span class="sxs-lookup"><span data-stu-id="a719f-112">Locate the **Manage** menu options, and select **Protection activation**.</span></span> <span data-ttu-id="a719f-113">انقر **فوق** تنشيط ، ثم قم بتأكيد الإجراء.</span><span class="sxs-lookup"><span data-stu-id="a719f-113">Click **Activate**, and then confirm your action.</span></span> <span data-ttu-id="a719f-114">عند اكتمال التنشيط، يعرض شريط المعلومات انتهاء **التنشيط بنجاح**.</span><span class="sxs-lookup"><span data-stu-id="a719f-114">When activation is complete, the information bar displays **Activation finished successfully**.</span></span>

<span data-ttu-id="a719f-115">**ترحيل تسميات Azure Information Protection إلى مركز & أمان Office 365**</span><span class="sxs-lookup"><span data-stu-id="a719f-115">**Migrate Azure Information Protection labels to Office 365 Security & Compliance Center**</span></span>

1. <span data-ttu-id="a719f-116">تأكد من تسجيل دخولك كمستخدم بإذن المسؤول العام.</span><span class="sxs-lookup"><span data-stu-id="a719f-116">Make sure you are logged in as a user with Global Administrator permission.</span></span>

2. <span data-ttu-id="a719f-117">انتقل إلى **شفرة Azure Information Protection.**</span><span class="sxs-lookup"><span data-stu-id="a719f-117">Navigate to the **Azure Information Protection** blade.</span></span>

3. <span data-ttu-id="a719f-118">من خيار **القائمة إدارة،** حدد **تسمية موحدة**.</span><span class="sxs-lookup"><span data-stu-id="a719f-118">From the **Manage** menu option, select **Unified labeling**.</span></span>

4. <span data-ttu-id="a719f-119">على **شفرة حماية معلومات Azure - تسمية** موحدة، انقر فوق **تنشيط** واتبع الإرشادات عبر الإنترنت.</span><span class="sxs-lookup"><span data-stu-id="a719f-119">On the **Azure Information Protection - Unified labeling** blade, click **Activate** and follow the online instructions.</span></span>

<span data-ttu-id="a719f-120">**ملاحظة:** تحقق من أن لديك الأذونات المناسبة قبل تنشيط & مركز التوافق.</span><span class="sxs-lookup"><span data-stu-id="a719f-120">**Note**: Verify that you have the appropriate permissions before activating the Security & Compliance Center Migration.</span></span> <span data-ttu-id="a719f-121">لمزيد من المعلومات، راجع هذه المقالات:</span><span class="sxs-lookup"><span data-stu-id="a719f-121">See these articles for more info:</span></span>

1. [<span data-ttu-id="a719f-122">هل تحتاج إلى أن تكون مسؤولا عاما لتكوين Azure Information Protection، أو هل يمكنني التفويض إلى مسؤولي آخرين؟</span><span class="sxs-lookup"><span data-stu-id="a719f-122">Do you need to be a global admin to configure Azure Information Protection, or can I delegate to other administrators?</span></span>](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [<span data-ttu-id="a719f-123">معلومات مهمة حول الأدوار الإدارية بعد عملية إعادة & مركز التوافق.</span><span class="sxs-lookup"><span data-stu-id="a719f-123">Important information about administrative roles after migrating to Security & Compliance Center.</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

<span data-ttu-id="a719f-124">لمزيد من المعلومات حول ترحيل AIP إلى التسميات الموحدة إلى مركز الأمان والتوافق، راجع [ترحيل التسميات](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).</span><span class="sxs-lookup"><span data-stu-id="a719f-124">For more information on the AIP to Unified Labeling migration to Security and Compliance Center, see [Migrate labels](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).</span></span>
