---
title: 'الماسح الضوئي ل IP: التثبيت والتكوين'
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
- "5119"
ms.openlocfilehash: be5b63ffccd5bbd83e7802e4ef5aa657ed921ae6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47686629"
---
# <a name="aip-scanner-installation-and-configuration"></a><span data-ttu-id="7ab77-102">الماسح الضوئي ل IP: التثبيت والتكوين</span><span class="sxs-lookup"><span data-stu-id="7ab77-102">AIP scanner: installation and configuration</span></span>

<span data-ttu-id="7ab77-103">**لتثبيت الماسح الضوئي AIP ، اتبع الإرشادات المستحسنة**:</span><span class="sxs-lookup"><span data-stu-id="7ab77-103">**To install the AIP scanner, follow the recommended guidelines**:</span></span>

1. <span data-ttu-id="7ab77-104">إذا كنت تقوم بالترقية ولا تجري التثبيت النظيف ، فالرجاء التاكد من اتباع الإرشادات المتعلقة [بترقيه الماسح الضوئي لحماية البيانات في azure](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) ولعميل التسمية الموحد ، راجع [ترقيه الماسح الضوئي لحماية البيانات في azure](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).</span><span class="sxs-lookup"><span data-stu-id="7ab77-104">If you are upgrading and not performing a clean installation, please make sure you have followed the guidelines for [upgrading the Azure Information Protection scanner](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) and for unified labeling client, see [upgrading the Azure Information Protection scanner](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).</span></span>
2. <span data-ttu-id="7ab77-105">تاكد من انك تلتزم بكل [متطلبات إعدادات الشبكات الاساسيه وجدران الحماية](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure).</span><span class="sxs-lookup"><span data-stu-id="7ab77-105">Verify that you comply with all [Firewalls and network infrastructure settings requirements](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure).</span></span>
3. <span data-ttu-id="7ab77-106">تاكد من تعيين التسمية التلقائية [للنهج الخاصة](https://docs.microsoft.com/azure/information-protection/configure-policy) بك أو الحصول علي تسميات افتراضيه في النهج.</span><span class="sxs-lookup"><span data-stu-id="7ab77-106">Make sure your [policies are set](https://docs.microsoft.com/azure/information-protection/configure-policy) to automatic labeling or have a default label in the policy.</span></span>
4. <span data-ttu-id="7ab77-107">تاكد من تكوين نوع الملف ذي الصلة للتسمية/الحماية كما هو موضح في [أنواع الملفات التي يعتمدها عميل حماية البيانات في Azure](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection).</span><span class="sxs-lookup"><span data-stu-id="7ab77-107">Make sure that the relevant file type is configured for label/protection as described in [File types supported by the Azure Information Protection client](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection).</span></span> <span data-ttu-id="7ab77-108">بالاضافه إلى ذلك ، إذا كنت تريد تغيير السلوك الافتراضي ، فاتبع الإرشادات التالية: [تغيير مستوي الحماية الافتراضي للملفات](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).</span><span class="sxs-lookup"><span data-stu-id="7ab77-108">In addition, if you want to change the default behavior, follow these guidelines: [Changing the default protection level of files](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).</span></span>
5. <span data-ttu-id="7ab77-109">تاكد من ان حساب المستخدم الذي تم تكوينه لتشغيل خدمه الماسح الضوئي يملك أذونات للوصول إلى كل المستودعات التي تم تكوينها.</span><span class="sxs-lookup"><span data-stu-id="7ab77-109">Verify that the user account configured to run the scanner service has permissions to access all the configured repositories.</span></span>
6. <span data-ttu-id="7ab77-110">إذا كنت لا تزال تواجه مشاكل ، يرجى تصدير سجلات الماسح الضوئي وأضافها إلى تذكره الدعم.</span><span class="sxs-lookup"><span data-stu-id="7ab77-110">If you still experience issues, please export the scanner logs and add them to your support ticket.</span></span>

<span data-ttu-id="7ab77-111">**تصدير سجلات الماسح الخاصة بحماية البيانات في Azure**</span><span class="sxs-lookup"><span data-stu-id="7ab77-111">**Export Azure Information Protection Scanner logs**</span></span>

1. <span data-ttu-id="7ab77-112">انتقل إلى%localappdata%\Microsoft\MSIP تحت سياق المستخدم الذي يقوم بتشغيل خدمه الماسح الضوئي.</span><span class="sxs-lookup"><span data-stu-id="7ab77-112">Navigate to %localappdata%\Microsoft\MSIP under the user context running the scanner service.</span></span>
2. <span data-ttu-id="7ab77-113">الكل المحتويات أسفل المجلد مسيب.</span><span class="sxs-lookup"><span data-stu-id="7ab77-113">Zip all the contents under the MSIP folder.</span></span>
3. <span data-ttu-id="7ab77-114">احفظ السجلات في اختيار الموقع ، وقم بإرفاقها بطلب الخدمة.</span><span class="sxs-lookup"><span data-stu-id="7ab77-114">Save the logs to your choice of location, and attach them to your service request.</span></span>
4. <span data-ttu-id="7ab77-115">يمكنك أيضا استخدام [التصدير-أيبلوجس-أونبيهالفوف](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).</span><span class="sxs-lookup"><span data-stu-id="7ab77-115">You can also use [Export-AIPLogs -OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).</span></span>

<span data-ttu-id="7ab77-116">**للحصول علي مزيد من المعلومات ، راجع**:</span><span class="sxs-lookup"><span data-stu-id="7ab77-116">**For additional information, see**:</span></span>
- [<span data-ttu-id="7ab77-117">نشر الماسح الضوئي لحماية البيانات في Azure لتصنيف الملفات وحمايتها تلقائيا</span><span class="sxs-lookup"><span data-stu-id="7ab77-117">Deploying the Azure Information Protection scanner to automatically classify and protect files</span></span>](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [<span data-ttu-id="7ab77-118">تحديد معلمه الرمز المميز لأيباوثينتيكيشن واستخدامها</span><span class="sxs-lookup"><span data-stu-id="7ab77-118">Specify and use the Token parameter for Set-AIPAuthentication</span></span>](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [<span data-ttu-id="7ab77-119">تشغيل دوره اكتشاف وعرض التقارير الخاصة بالماسح الضوئي</span><span class="sxs-lookup"><span data-stu-id="7ab77-119">Run a discovery cycle and view reports for the scanner</span></span>](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [<span data-ttu-id="7ab77-120">مراجعه وثائق حماية البيانات في Azure</span><span class="sxs-lookup"><span data-stu-id="7ab77-120">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="7ab77-121">متطلبات حماية البيانات في Azure</span><span class="sxs-lookup"><span data-stu-id="7ab77-121">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [<span data-ttu-id="7ab77-122">تنزيل عميل حماية المعلومات في Azure</span><span class="sxs-lookup"><span data-stu-id="7ab77-122">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)
