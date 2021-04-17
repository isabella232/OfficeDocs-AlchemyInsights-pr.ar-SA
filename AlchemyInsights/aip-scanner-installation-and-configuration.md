---
title: 'ماسح ضوئي AIP: التثبيت والتكوين'
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
- "5119"
ms.openlocfilehash: c32f3f10e2e17cf67e73ec8404be293eeefb68a3
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821650"
---
# <a name="aip-scanner-installation-and-configuration"></a><span data-ttu-id="eaeeb-102">ماسح ضوئي AIP: التثبيت والتكوين</span><span class="sxs-lookup"><span data-stu-id="eaeeb-102">AIP scanner: installation and configuration</span></span>

<span data-ttu-id="eaeeb-103">**لتثبيت ماسح AIP الضوئي، اتبع الإرشادات الموصى بها:**</span><span class="sxs-lookup"><span data-stu-id="eaeeb-103">**To install the AIP scanner, follow the recommended guidelines**:</span></span>

1. <span data-ttu-id="eaeeb-104">إذا كنت تقوم بالترقية ولا تقوم بإجراء تثبيت نظيف، فالرجاء التأكد من أنك اتبعت إرشادات ترقية ماسح حماية المعلومات [من Azure](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) ولعميل التسمية الموحد، راجع ترقية ماسح حماية المعلومات من [Azure](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).</span><span class="sxs-lookup"><span data-stu-id="eaeeb-104">If you are upgrading and not performing a clean installation, please make sure you have followed the guidelines for [upgrading the Azure Information Protection scanner](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) and for unified labeling client, see [upgrading the Azure Information Protection scanner](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).</span></span>
2. <span data-ttu-id="eaeeb-105">تحقق من امتثالك لجميع متطلبات إعدادات جدران الحماية والبنية الأساسية [للشبكة](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure).</span><span class="sxs-lookup"><span data-stu-id="eaeeb-105">Verify that you comply with all [Firewalls and network infrastructure settings requirements](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure).</span></span>
3. <span data-ttu-id="eaeeb-106">تأكد من [تعيين النهج إلى](https://docs.microsoft.com/azure/information-protection/configure-policy) تسمية تلقائية أو وضع تسمية افتراضية لها في النهج.</span><span class="sxs-lookup"><span data-stu-id="eaeeb-106">Make sure your [policies are set](https://docs.microsoft.com/azure/information-protection/configure-policy) to automatic labeling or have a default label in the policy.</span></span>
4. <span data-ttu-id="eaeeb-107">تأكد من تكوين نوع الملف ذي الصلة للتسمية/الحماية كما هو موضح في أنواع الملفات المعتمدة [بواسطة عميل Azure Information Protection](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection).</span><span class="sxs-lookup"><span data-stu-id="eaeeb-107">Make sure that the relevant file type is configured for label/protection as described in [File types supported by the Azure Information Protection client](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection).</span></span> <span data-ttu-id="eaeeb-108">بالإضافة إلى ذلك، إذا كنت تريد تغيير السلوك الافتراضي، فاتبع الإرشادات التالية: تغيير مستوى الحماية [الافتراضي للملفات](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).</span><span class="sxs-lookup"><span data-stu-id="eaeeb-108">In addition, if you want to change the default behavior, follow these guidelines: [Changing the default protection level of files](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).</span></span>
5. <span data-ttu-id="eaeeb-109">تحقق من أن حساب المستخدم الذي تم تكوينه لتشغيل خدمة الماسح الضوئي لديه أذونات للوصول إلى كل المستودعات التي تم تكوينها.</span><span class="sxs-lookup"><span data-stu-id="eaeeb-109">Verify that the user account configured to run the scanner service has permissions to access all the configured repositories.</span></span>
6. <span data-ttu-id="eaeeb-110">إذا ما زلت تواجه مشاكل، فيرجى تصدير سجلات الماسح الضوئي وإضافتها إلى تذكرة الدعم.</span><span class="sxs-lookup"><span data-stu-id="eaeeb-110">If you still experience issues, please export the scanner logs and add them to your support ticket.</span></span>

<span data-ttu-id="eaeeb-111">**تصدير سجلات ماسح حماية المعلومات في Azure**</span><span class="sxs-lookup"><span data-stu-id="eaeeb-111">**Export Azure Information Protection Scanner logs**</span></span>

1. <span data-ttu-id="eaeeb-112">انتقل إلى ٪localappdata٪\Microsoft\MSIP ضمن سياق المستخدم الذي يقوم بتشغيل خدمة الماسح الضوئي.</span><span class="sxs-lookup"><span data-stu-id="eaeeb-112">Navigate to %localappdata%\Microsoft\MSIP under the user context running the scanner service.</span></span>
2. <span data-ttu-id="eaeeb-113">اضغط على كل المحتويات ضمن مجلد MSIP.</span><span class="sxs-lookup"><span data-stu-id="eaeeb-113">Zip all the contents under the MSIP folder.</span></span>
3. <span data-ttu-id="eaeeb-114">احفظ السجلات إلى اختيارك للموقع، وأرفقها بطلب الخدمة.</span><span class="sxs-lookup"><span data-stu-id="eaeeb-114">Save the logs to your choice of location, and attach them to your service request.</span></span>
4. <span data-ttu-id="eaeeb-115">يمكنك أيضا استخدام [Export-AIPLogs -OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).</span><span class="sxs-lookup"><span data-stu-id="eaeeb-115">You can also use [Export-AIPLogs -OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).</span></span>

<span data-ttu-id="eaeeb-116">**لمزيد من المعلومات، راجع:**</span><span class="sxs-lookup"><span data-stu-id="eaeeb-116">**For additional information, see**:</span></span>
- [<span data-ttu-id="eaeeb-117">نشر ماسح حماية المعلومات من Azure لتصنيف الملفات وحمايتها تلقائيا</span><span class="sxs-lookup"><span data-stu-id="eaeeb-117">Deploying the Azure Information Protection scanner to automatically classify and protect files</span></span>](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [<span data-ttu-id="eaeeb-118">تحديد المعلمة Token ل Set-AIPAuthentication واستخدامها</span><span class="sxs-lookup"><span data-stu-id="eaeeb-118">Specify and use the Token parameter for Set-AIPAuthentication</span></span>](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [<span data-ttu-id="eaeeb-119">تشغيل دورة اكتشاف وعرض التقارير للماسح الضوئي</span><span class="sxs-lookup"><span data-stu-id="eaeeb-119">Run a discovery cycle and view reports for the scanner</span></span>](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [<span data-ttu-id="eaeeb-120">مراجعة وثائق Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="eaeeb-120">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="eaeeb-121">متطلبات حماية معلومات Azure</span><span class="sxs-lookup"><span data-stu-id="eaeeb-121">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [<span data-ttu-id="eaeeb-122">تنزيل عميل Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="eaeeb-122">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)
