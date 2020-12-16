---
title: نقل الخدمات-نقل كل خدمات ردفي إلى اشتراك آخر
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004116"
- "7196"
ms.openlocfilehash: d6744484fe42f09f03de562a00fd56712607d418
ms.sourcegitcommit: ec88047d550006a1df4b6f10a3f513218113b9a5
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/15/2020
ms.locfileid: "49691915"
---
# <a name="transfer-services---move-all-rdfe-services-to-another-subscription"></a><span data-ttu-id="3d756-102">نقل الخدمات-نقل كل خدمات ردفي إلى اشتراك آخر</span><span class="sxs-lookup"><span data-stu-id="3d756-102">Transfer Services - Move all RDFE services to another subscription</span></span>

<span data-ttu-id="3d756-103">**نقل الموارد**</span><span class="sxs-lookup"><span data-stu-id="3d756-103">**Move resources**</span></span>

<span data-ttu-id="3d756-104">يمكن نقل موارد azure إلى اشتراك آخر في Azure أو مجموعه موارد ضمن الاشتراك نفسه باستخدام Azure portal أو Azure PowerShell أو Azure CLI أو REST API لنقل الموارد.</span><span class="sxs-lookup"><span data-stu-id="3d756-104">Azure resources can be moved to either another Azure subscription or resource group under the same subscription using Azure portal, Azure PowerShell, Azure CLI, or the REST API to move resources.</span></span>

<span data-ttu-id="3d756-105">قبل ان تتمكن من نقل الموارد ، راجع:</span><span class="sxs-lookup"><span data-stu-id="3d756-105">Before you can move resources, see:</span></span>

- [<span data-ttu-id="3d756-106">قائمه الاختيار قبل نقل الموارد</span><span class="sxs-lookup"><span data-stu-id="3d756-106">Checklist before moving resources</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#checklist-before-moving-resources)
- [<span data-ttu-id="3d756-107">الخدمات التي يمكن نقلها</span><span class="sxs-lookup"><span data-stu-id="3d756-107">Services that can be moved</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/move-support-resources?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="3d756-108">كيفيه التحقق من صحة النقل</span><span class="sxs-lookup"><span data-stu-id="3d756-108">How to validate the move</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#validate-move)
- [<span data-ttu-id="3d756-109">نقل إرشادات للخدمات</span><span class="sxs-lookup"><span data-stu-id="3d756-109">Move guidance for services</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/move-limitations/app-service-move-limitations?WT.mc_id=Portal-Microsoft_Azure_Support)

<span data-ttu-id="3d756-110">لنقل الموارد الموجودة إلى مجموعه موارد أو اشتراك آخر ، يمكنك استخدام:</span><span class="sxs-lookup"><span data-stu-id="3d756-110">To move existing resources to another resource group or subscription, you can use:</span></span>

- [<span data-ttu-id="3d756-111">مدخل Azure</span><span class="sxs-lookup"><span data-stu-id="3d756-111">Azure portal</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-the-portal)
- [<span data-ttu-id="3d756-112">Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="3d756-112">Azure PowerShell</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-powershell)
- [<span data-ttu-id="3d756-113">Azure CLI</span><span class="sxs-lookup"><span data-stu-id="3d756-113">Azure CLI</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-cli)
- [<span data-ttu-id="3d756-114">واجهه برمجه تطبيقات REST</span><span class="sxs-lookup"><span data-stu-id="3d756-114">REST API</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-rest-api)

<span data-ttu-id="3d756-115">برنامج تعليمي: [نقل موارد Azure إلى مجموعه موارد أخرى أو اشتراك](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)</span><span class="sxs-lookup"><span data-stu-id="3d756-115">Tutorial: [Move Azure resources to another resource group or subscription](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)</span></span>

<span data-ttu-id="3d756-116">**استكشاف الأخطاء وإصلاحها باستخدام Azure Resource Manager**</span><span class="sxs-lookup"><span data-stu-id="3d756-116">**Troubleshoot errors with Azure Resource Manager**</span></span>

<span data-ttu-id="3d756-117">ارجع إلى المقالات أدناه للتعرف علي بعض أخطاء نشر Azure الشائعة وتلقي معلومات لحلها.</span><span class="sxs-lookup"><span data-stu-id="3d756-117">Refer to the articles below to learn about some common Azure deployment errors and receive information to resolve them.</span></span> <span data-ttu-id="3d756-118">إذا لم تتمكن من العثور علي رمز الخطا الخاص برسالة خطا النشر ، فراجع [البحث عن رمز الخطا](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code).</span><span class="sxs-lookup"><span data-stu-id="3d756-118">If you can't find the error code for your deployment error, see [Find error code](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code).</span></span>

- [<span data-ttu-id="3d756-119">استكشاف أخطاء النشر وإصلاحها</span><span class="sxs-lookup"><span data-stu-id="3d756-119">Troubleshoot deployment errors</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors)
- [<span data-ttu-id="3d756-120">استكشاف أخطاء نقل موارد Azure إلى مجموعه موارد جديده أو الاشتراك فيها</span><span class="sxs-lookup"><span data-stu-id="3d756-120">Troubleshoot moving Azure resources to new resource group or subscription</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/troubleshoot-move)

<span data-ttu-id="3d756-121">لاحظ انه إذا كنت ترغب في ترقيه اشتراكك في Azure ، مثل التبديل من التحديث المجاني إلى الدفع اثناء التنقل ، ستحتاج إلى تحويل اشتراكك.</span><span class="sxs-lookup"><span data-stu-id="3d756-121">Note that if you would like to upgrade your Azure subscription, such as switching from free to pay-as-you-go, you will need to convert your subscription.</span></span>

- <span data-ttu-id="3d756-122">لترقيه فتره تجريبية مجانية ، راجع [ترقيه الإصدار التجريبي المجاني أو الاشتراك الخاص ب Microsoft تصور Azure للدفع بالدفع](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription).</span><span class="sxs-lookup"><span data-stu-id="3d756-122">To upgrade a free trial, see [Upgrade your Free Trial or Microsoft Imagine Azure subscription to Pay-As-You-Go](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription).</span></span>
- <span data-ttu-id="3d756-123">لتغيير حساب الدفع اثناء التنقل ، اطلع علي [تغيير الاشتراك المدفوع باستخدام Azure إلى عرض مختلف](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer)عنه.</span><span class="sxs-lookup"><span data-stu-id="3d756-123">To change a pay-as-you-go account, see [Change your Azure Pay-As-You-Go subscription to a different offer](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer).</span></span>

<span data-ttu-id="3d756-124">**لأضافه اشتراك Azure إلى المستاجر الخاص بك في Azure Active Directory أو اقرانه:**</span><span class="sxs-lookup"><span data-stu-id="3d756-124">**To add or associate an Azure subscription to your Azure Active Directory tenant:**</span></span>

1. <span data-ttu-id="3d756-125">سجل الدخول وحدد الاشتراك الذي تريد استخدامه من [صفحه الاشتراكات في مدخل Azure](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade).</span><span class="sxs-lookup"><span data-stu-id="3d756-125">Sign in and select the subscription you want to use from the [Subscriptions page in Azure portal](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade).</span></span>
2. <span data-ttu-id="3d756-126">حدد **تغيير الدليل**.</span><span class="sxs-lookup"><span data-stu-id="3d756-126">Select **Change directory**.</span></span>
3. <span data-ttu-id="3d756-127">راجع اي تحذيرات تظهر ، ثم حدد **تغيير**.</span><span class="sxs-lookup"><span data-stu-id="3d756-127">Review any warnings that appear, and then select **Change**.</span></span>
4. <span data-ttu-id="3d756-128">يتم تغيير الدليل للاشتراك ستحصل علي رسالة نجاح.</span><span class="sxs-lookup"><span data-stu-id="3d756-128">The directory is changed for the subscription and you will get a success message.</span></span>
5. <span data-ttu-id="3d756-129">استخدم مبدل *الدلائل* للانتقال إلى الدليل الجديد.</span><span class="sxs-lookup"><span data-stu-id="3d756-129">Use the *Directory* switcher to go to your new directory.</span></span> <span data-ttu-id="3d756-130">قد يستغرق عرض كل شيء بشكل صحيح حتى 10 دقائق.</span><span class="sxs-lookup"><span data-stu-id="3d756-130">It may take up to 10 minutes for everything to show up properly.</span></span>

<span data-ttu-id="3d756-131">**المستندات المستحسنة**</span><span class="sxs-lookup"><span data-stu-id="3d756-131">**Recommended Documents**</span></span>

- [<span data-ttu-id="3d756-132">نقل ملكيه اشتراك Azure</span><span class="sxs-lookup"><span data-stu-id="3d756-132">Transferring ownership of an Azure subscription</span></span>](https://docs.microsoft.com/azure/billing-subscription-transfer)
- [<span data-ttu-id="3d756-133">نقل الموارد إلى مجموعه موارد جديده أو اشتراك</span><span class="sxs-lookup"><span data-stu-id="3d756-133">Move resources to new resource group or subscription</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources)
- [<span data-ttu-id="3d756-134">أداره الموارد باستخدام مدخل Azure</span><span class="sxs-lookup"><span data-stu-id="3d756-134">Manage resources using Azure portal</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-portal)
