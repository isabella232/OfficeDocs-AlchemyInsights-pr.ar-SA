---
title: إنشاء نُهج تسمية AIP
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "4539"
- "9002266"
ms.openlocfilehash: de7d76564cabb0a5dd1a836984df6b1a63b2b218
ms.sourcegitcommit: 8fdcd2acd31e8a4b9a8a0b91674f397d2f7889c1
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/03/2020
ms.locfileid: "44568886"
---
# <a name="creating-aip-label-policies"></a><span data-ttu-id="6c558-102">إنشاء نُهج تسمية AIP</span><span class="sxs-lookup"><span data-stu-id="6c558-102">Creating AIP Label Policies</span></span>

<span data-ttu-id="6c558-103">يمكن استخدام تسميات حماية المعلومات Azure (AIP) مع المجموعة الكاملة من البيانات التي تقوم المؤسسة عادة بإنشائها وتخزينها، من أدنى تصنيف للبيانات الشخصية، إلى أعلى تصنيف للبيانات السرية للغاية.</span><span class="sxs-lookup"><span data-stu-id="6c558-103">Azure Information Protection(AIP) labels can be used with the full range of data that an organization typically creates and stores, from the lowest classification of personal data, to the highest classification of highly confidential data.</span></span> <span data-ttu-id="6c558-104">تنطبق سياسات حماية المعلومات Azure على العميل الكلاسيكي لحماية المعلومات Azure (AIP) وليس [على عميل العلامات الموحدة AIP](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history).</span><span class="sxs-lookup"><span data-stu-id="6c558-104">Azure Information Protection Policies apply to the Azure Information Protection(AIP) classic client and not the  [AIP Unified Labeling client](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history).</span></span> <span data-ttu-id="6c558-105">يمكنك تكوين عناصر متعددة في نهج AIP، بما في ذلك خيارات مثل:</span><span class="sxs-lookup"><span data-stu-id="6c558-105">You can configure multiple elements in an AIP policy, including options like:</span></span>

- <span data-ttu-id="6c558-106">الخيار الذي سيسمح للعلامة للمسؤولين أو المستخدم بتصنيف وحماية (اختياري) المستندات ورسائل البريد الإلكتروني</span><span class="sxs-lookup"><span data-stu-id="6c558-106">Option for which label will let administrators or user classify and protection(optional) documents and emails</span></span>
- <span data-ttu-id="6c558-107">خيار فرض التصنيف عندما يقوم المستخدمون بحفظ المستندات وإرسال البريد الإلكتروني</span><span class="sxs-lookup"><span data-stu-id="6c558-107">Option to enforce classification when users save documents and send email</span></span>
- <span data-ttu-id="6c558-108">خيار تسمية رسالة بريد إلكتروني تلقائيًا، استنادًا إلى مرفقاتها.</span><span class="sxs-lookup"><span data-stu-id="6c558-108">Option to automatically label an email message, based on its attachments.</span></span>
- <span data-ttu-id="6c558-109">خيار التحكم في ما إذا كان يتم عرض شريط حماية المعلومات في تطبيقات Office</span><span class="sxs-lookup"><span data-stu-id="6c558-109">Option to control whether the Information Protection bar is displayed in Office applications</span></span>

<span data-ttu-id="6c558-110">للحصول على خيارات ومعلومات إضافية حول سياسات حماية المعلومات Azure، راجع: [نظرة عامة على سياسة حماية المعلومات Azure](https://docs.microsoft.com/azure/information-protection/overview-policy).</span><span class="sxs-lookup"><span data-stu-id="6c558-110">For additional options and information on Azure Information Protection policies, see: [Overview of the Azure Information Protection policy](https://docs.microsoft.com/azure/information-protection/overview-policy).</span></span>  

<span data-ttu-id="6c558-111">للحصول على موارد مفيدة أخرى فيما يتعلق بسياسات AIP، راجع:</span><span class="sxs-lookup"><span data-stu-id="6c558-111">For other helpful resources regarding AIP policies, see:</span></span>

- [<span data-ttu-id="6c558-112">البرنامج التعليمي: تكوين إعدادات نهج حماية المعلومات Azure وإنشاء تسمية جديدة</span><span class="sxs-lookup"><span data-stu-id="6c558-112">Tutorial: Configure Azure Information Protection policy settings and create a new label</span></span>](https://docs.microsoft.com/azure/information-protection/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="6c558-113">تكوين نهج حماية المعلومات Azure</span><span class="sxs-lookup"><span data-stu-id="6c558-113">Configuring the Azure Information Protection policy</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy)  
- [<span data-ttu-id="6c558-114">إنشاء وتكوين تسميات الحساسية وسياساتها</span><span class="sxs-lookup"><span data-stu-id="6c558-114">Create and configure sensitivity labels and their policies</span></span>](https://docs.microsoft.com/microsoft-365/compliance/create-sensitivity-labels)  
- [<span data-ttu-id="6c558-115">أدلة إرشادية للسيناريوهات الشائعة التي تستخدم حماية معلومات Azure</span><span class="sxs-lookup"><span data-stu-id="6c558-115">How-to guides for common scenarios that use Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/how-to-guides)  
- [<span data-ttu-id="6c558-116">مراجعة وثائق حماية المعلومات Azure</span><span class="sxs-lookup"><span data-stu-id="6c558-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)  
- [<span data-ttu-id="6c558-117">متطلبات حماية المعلومات اللازوردية</span><span class="sxs-lookup"><span data-stu-id="6c558-117">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)  
- [<span data-ttu-id="6c558-118">بدء سريع تعليمي لحماية المعلومات أزور</span><span class="sxs-lookup"><span data-stu-id="6c558-118">Quick start tutorial for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="6c558-119">تحميل عميل حماية المعلومات Azure</span><span class="sxs-lookup"><span data-stu-id="6c558-119">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)