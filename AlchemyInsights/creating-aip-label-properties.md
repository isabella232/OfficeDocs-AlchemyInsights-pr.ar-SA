---
title: إنشاء نهج التسمية AIP
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "4539"
- "9002266"
ms.openlocfilehash: bef170d8e38dcc91094b95604aeb1968d5c57fca
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47732162"
---
# <a name="creating-aip-label-policies"></a><span data-ttu-id="579a7-102">إنشاء نهج التسمية AIP</span><span class="sxs-lookup"><span data-stu-id="579a7-102">Creating AIP Label Policies</span></span>

<span data-ttu-id="579a7-103">يمكن استخدام تسميات حماية معلومات Azure (AIP) مع نطاق كامل من البيانات التي تنشئها المؤسسة عاده وتخزنها ، من التصنيف الأدنى للبيانات الشخصية ، إلى اعلي تصنيف للبيانات السرية عاليه الجودة.</span><span class="sxs-lookup"><span data-stu-id="579a7-103">Azure Information Protection(AIP) labels can be used with the full range of data that an organization typically creates and stores, from the lowest classification of personal data, to the highest classification of highly confidential data.</span></span> <span data-ttu-id="579a7-104">تنطبق نهج حماية البيانات في azure علي عميل كلاسيكي لحماية معلومات Azure (AIP) وليس  [عميل التسمية الموحدة ل ip](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history).</span><span class="sxs-lookup"><span data-stu-id="579a7-104">Azure Information Protection Policies apply to the Azure Information Protection(AIP) classic client and not the  [AIP Unified Labeling client](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history).</span></span> <span data-ttu-id="579a7-105">يمكنك تكوين عده عناصر في نهج AIP ، بما في ذلك خيارات مثل:</span><span class="sxs-lookup"><span data-stu-id="579a7-105">You can configure multiple elements in an AIP policy, including options like:</span></span>

- <span data-ttu-id="579a7-106">خيار التسمية التي ستسمح للمسؤولين أو تصنيف المستخدمين والمستندات والبريد الكتروني وحمايتها (اختياري)</span><span class="sxs-lookup"><span data-stu-id="579a7-106">Option for which label will let administrators or user classify and protection(optional) documents and emails</span></span>
- <span data-ttu-id="579a7-107">خيار فرض التصنيف عندما يقوم المستخدمون بحفظ المستندات وإرسال البريد الكتروني</span><span class="sxs-lookup"><span data-stu-id="579a7-107">Option to enforce classification when users save documents and send email</span></span>
- <span data-ttu-id="579a7-108">خيار لتسميه رسالة بريد الكتروني تلقائيا ، استنادا إلى مرفقاتها.</span><span class="sxs-lookup"><span data-stu-id="579a7-108">Option to automatically label an email message, based on its attachments.</span></span>
- <span data-ttu-id="579a7-109">خيار للتحكم في ما إذا كان شريط حماية المعلومات معروضا في تطبيقات Office</span><span class="sxs-lookup"><span data-stu-id="579a7-109">Option to control whether the Information Protection bar is displayed in Office applications</span></span>

<span data-ttu-id="579a7-110">للحصول علي خيارات ومعلومات اضافيه حول نهج حماية البيانات في Azure ، راجع: [نظره عامه حول نهج حماية البيانات في azure](https://docs.microsoft.com/azure/information-protection/overview-policy).</span><span class="sxs-lookup"><span data-stu-id="579a7-110">For additional options and information on Azure Information Protection policies, see: [Overview of the Azure Information Protection policy](https://docs.microsoft.com/azure/information-protection/overview-policy).</span></span>  

<span data-ttu-id="579a7-111">للحصول علي موارد مفيده أخرى بخصوص نهج AIP ، راجع:</span><span class="sxs-lookup"><span data-stu-id="579a7-111">For other helpful resources regarding AIP policies, see:</span></span>

- [<span data-ttu-id="579a7-112">برنامج تعليمي: تكوين إعدادات نهج حماية البيانات في Azure وإنشاء تسميه جديده</span><span class="sxs-lookup"><span data-stu-id="579a7-112">Tutorial: Configure Azure Information Protection policy settings and create a new label</span></span>](https://docs.microsoft.com/azure/information-protection/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="579a7-113">تكوين نهج حماية البيانات في Azure</span><span class="sxs-lookup"><span data-stu-id="579a7-113">Configuring the Azure Information Protection policy</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy)  
- [<span data-ttu-id="579a7-114">إنشاء تسميات الحساسية ونهجها وتكوينها</span><span class="sxs-lookup"><span data-stu-id="579a7-114">Create and configure sensitivity labels and their policies</span></span>](https://docs.microsoft.com/microsoft-365/compliance/create-sensitivity-labels)  
- [<span data-ttu-id="579a7-115">إرشادات ارشاديه للسيناريوهات الشائعة التي تستخدم حماية البيانات في Azure</span><span class="sxs-lookup"><span data-stu-id="579a7-115">How-to guides for common scenarios that use Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/how-to-guides)  
- [<span data-ttu-id="579a7-116">مراجعه وثائق حماية البيانات في Azure</span><span class="sxs-lookup"><span data-stu-id="579a7-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)  
- [<span data-ttu-id="579a7-117">متطلبات حماية البيانات في Azure</span><span class="sxs-lookup"><span data-stu-id="579a7-117">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)  
- [<span data-ttu-id="579a7-118">البرنامج التعليمي لبدء التشغيل السريع لحماية البيانات في Azure</span><span class="sxs-lookup"><span data-stu-id="579a7-118">Quick start tutorial for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="579a7-119">تنزيل عميل حماية المعلومات في Azure</span><span class="sxs-lookup"><span data-stu-id="579a7-119">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)