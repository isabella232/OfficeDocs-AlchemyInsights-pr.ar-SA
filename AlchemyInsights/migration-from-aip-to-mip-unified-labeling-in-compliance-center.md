---
title: الترحيل من AIP إلى ميب/التسمية الموحدة في مركز التوافق
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5114"
ms.openlocfilehash: 7157eada10db2443f64fb7925f408359275d75eb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47674313"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a><span data-ttu-id="bb647-102">الترحيل من AIP إلى ميب/التسمية الموحدة في مركز التوافق</span><span class="sxs-lookup"><span data-stu-id="bb647-102">Migration from AIP to MIP/Unified Labeling in the Compliance Center</span></span>

<span data-ttu-id="bb647-103">للترحيل من AIPات IP إلى التسمية الموحدة في مركز الأمان والتوافق ، قم بما يلي:</span><span class="sxs-lookup"><span data-stu-id="bb647-103">To migrate from AIP labels to Unified Labeling in the Security and Compliance center, do the following:</span></span>

<span data-ttu-id="bb647-104">**تنشيط الحماية من مدخل Azure**</span><span class="sxs-lookup"><span data-stu-id="bb647-104">**Activate protection from the Azure portal**</span></span>

1. <span data-ttu-id="bb647-105">إذا لم تكن قد فعلت ذلك بعد ، فافتح نافذه مستعرض جديده وقم [بتسجيل الدخول إلى مدخل Azure](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal).</span><span class="sxs-lookup"><span data-stu-id="bb647-105">If you haven't already done so, open a new browser window and [sign in to the Azure portal](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal).</span></span> <span data-ttu-id="bb647-106">انتقل إلى ريش **حماية البيانات في Azure** .</span><span class="sxs-lookup"><span data-stu-id="bb647-106">Navigate to the **Azure Information Protection** blade.</span></span> <span data-ttu-id="bb647-107">علي سبيل المثال ، في قائمه الموزع ، انقر فوق **كافة الخدمات** وأبدا بكتابه **المعلومات** في المربع عامل التصفية.</span><span class="sxs-lookup"><span data-stu-id="bb647-107">For example, on the hub menu, click **All services** and start typing **Information** in the Filter box.</span></span> <span data-ttu-id="bb647-108">حدد **حماية البيانات في Azure**.</span><span class="sxs-lookup"><span data-stu-id="bb647-108">Select **Azure Information Protection**.</span></span> <span data-ttu-id="bb647-109">إذا لم تكن قد قمت بالوصول إلى ريش حماية البيانات في Azure قبل ذلك ، فراجع [الخطوات الاضافيه لمره واحده](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) لأضافه هذا الريش إلى المدخل.</span><span class="sxs-lookup"><span data-stu-id="bb647-109">If you haven't accessed the Azure Information Protection blade before, see the one-time [additional steps](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) to add this blade to the portal.</span></span> <span data-ttu-id="bb647-110">لفتح ريش حماية البيانات في Azure ، يجب ان يتوفر لديك [خطه Premium لحماية البيانات في azure](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) أو خطه Office 365 التي تتضمن أداره الحقوق.</span><span class="sxs-lookup"><span data-stu-id="bb647-110">To open the Azure Information Protection blade, you must have either an [Azure Information Protection Premium plan](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) or an Office 365 plan that includes Rights Management.</span></span> <span data-ttu-id="bb647-111">إذا كان لديك أحد هذه الاشتراكات ولكنك تري رسالة تفيد بتعذر العثور علي اشتراك صحيح ، [فاتصل بدعم Microsoft](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) أو استخدم قنوات الدعم القياسية الخاصة بك.</span><span class="sxs-lookup"><span data-stu-id="bb647-111">If you have one of these subscriptions but see a message that a valid subscription cannot be found, [contact Microsoft Support](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) or use your standard support channels.</span></span>

2. <span data-ttu-id="bb647-112">حدد موقع خيارات القائمة **أداره** ، وحدد **تنشيط الحماية**.</span><span class="sxs-lookup"><span data-stu-id="bb647-112">Locate the **Manage** menu options, and select **Protection activation**.</span></span> <span data-ttu-id="bb647-113">انقر فوق **تنشيط**، ثم قم بتاكيد الاجراء.</span><span class="sxs-lookup"><span data-stu-id="bb647-113">Click **Activate**, and then confirm your action.</span></span> <span data-ttu-id="bb647-114">عند اكتمال عمليه التنشيط ، يعرض شريط المعلومات **انتهاء التنشيط بنجاح**.</span><span class="sxs-lookup"><span data-stu-id="bb647-114">When activation is complete, the information bar displays **Activation finished successfully**.</span></span>

<span data-ttu-id="bb647-115">**ترحيل تسميات حماية البيانات في Azure إلى مركز توافق & أمان Office 365**</span><span class="sxs-lookup"><span data-stu-id="bb647-115">**Migrate Azure Information Protection labels to Office 365 Security & Compliance Center**</span></span>

1. <span data-ttu-id="bb647-116">تاكد من انك قمت بتسجيل الدخول كمستخدم لديه اذن المسؤول العام.</span><span class="sxs-lookup"><span data-stu-id="bb647-116">Make sure you are logged in as a user with Global Administrator permission.</span></span>

2. <span data-ttu-id="bb647-117">انتقل إلى ريش **حماية البيانات في Azure** .</span><span class="sxs-lookup"><span data-stu-id="bb647-117">Navigate to the **Azure Information Protection** blade.</span></span>

3. <span data-ttu-id="bb647-118">من خيار القائمة **أداره** ، حدد **التسمية الموحدة**.</span><span class="sxs-lookup"><span data-stu-id="bb647-118">From the **Manage** menu option, select **Unified labeling**.</span></span>

4. <span data-ttu-id="bb647-119">في **حماية البيانات في Azure-النصليه التسمية الموحدة** ، انقر فوق **تنشيط** واتبع الإرشادات الموجودة علي الإنترنت.</span><span class="sxs-lookup"><span data-stu-id="bb647-119">On the **Azure Information Protection - Unified labeling** blade, click **Activate** and follow the online instructions.</span></span>

<span data-ttu-id="bb647-120">**ملاحظه**: تحقق من ان لديك الأذونات المناسبة قبل تنشيط ترحيل مركز توافق & الأمان.</span><span class="sxs-lookup"><span data-stu-id="bb647-120">**Note**: Verify that you have the appropriate permissions before activating the Security & Compliance Center Migration.</span></span> <span data-ttu-id="bb647-121">راجع هذه المقالات للحصول علي مزيد من المعلومات:</span><span class="sxs-lookup"><span data-stu-id="bb647-121">See these articles for more info:</span></span>

1. [<span data-ttu-id="bb647-122">هل تحتاج إلى ان تكون مسؤولا عاما لتكوين حماية البيانات في Azure ، ام يمكنني التفويض بالمسؤولين الآخرين ؟</span><span class="sxs-lookup"><span data-stu-id="bb647-122">Do you need to be a global admin to configure Azure Information Protection, or can I delegate to other administrators?</span></span>](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [<span data-ttu-id="bb647-123">معلومات مهمة حول الأدوار الاداريه بعد الترحيل إلى مركز توافق & الأمان.</span><span class="sxs-lookup"><span data-stu-id="bb647-123">Important information about administrative roles after migrating to Security & Compliance Center.</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

<span data-ttu-id="bb647-124">للحصول علي مزيد من المعلومات حول ترحيل التسمية الموحدة إلى مركز الأمان والتوافق ، راجع [ترحيل التسميات](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).</span><span class="sxs-lookup"><span data-stu-id="bb647-124">For more information on the AIP to Unified Labeling migration to Security and Compliance Center, see [Migrate labels](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).</span></span>
