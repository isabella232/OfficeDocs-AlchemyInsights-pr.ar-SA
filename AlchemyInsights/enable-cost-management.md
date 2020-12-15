---
title: تمكين أداره التكلفة
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003547"
- "6463"
ms.openlocfilehash: 0bbf1158f7f5fa8a22cfe7242c86760057fc7bab
ms.sourcegitcommit: 0f26f6b23b3d48c3c6cddf98bc41df484f16cb00
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/08/2020
ms.locfileid: "49676701"
---
# <a name="enable-cost-management"></a><span data-ttu-id="b4a9d-102">تمكين أداره التكلفة</span><span class="sxs-lookup"><span data-stu-id="b4a9d-102">Enable cost management</span></span>

<span data-ttu-id="b4a9d-103">**ما المقصود بتكاليف التكلفة المعطلة لمؤسسك ؟**</span><span class="sxs-lookup"><span data-stu-id="b4a9d-103">**What does 'costs are disabled for your organization' mean?**</span></span>

<span data-ttu-id="b4a9d-104">يمكن للمؤسسات التي تستخدم حسابات اتفاقيه المؤسسة (EA) أو اتفاقيه عملاء Microsoft (MCA) تعطيل الوصول إلى معلومات التكلفة ومعلومات الأسعار.</span><span class="sxs-lookup"><span data-stu-id="b4a9d-104">Organizations using Enterprise Agreement (EA) or Microsoft Customer Agreement (MCA) accounts can disable access to cost information and pricing information.</span></span>

<span data-ttu-id="b4a9d-105">بعد تسجيل الدخول إلى مدخل Azure ، يمكنه استخدام واجات برمجه التطبيقات (Api) للفوترة للحصول علي الفواتير بشكل برمجي (بمجرد تسجيل الدخول) وتفاصيل الاستخدام.</span><span class="sxs-lookup"><span data-stu-id="b4a9d-105">After logging in to Azure portal, they can use the Billing APIs to programmatically get invoices (once opted-in) and usage details.</span></span>

<span data-ttu-id="b4a9d-106">**كيفيه السماح لمستخدمين إضافيين بالوصول إلى الفواتير**</span><span class="sxs-lookup"><span data-stu-id="b4a9d-106">**How to allow additional users to access invoices**</span></span>

1. <span data-ttu-id="b4a9d-107">انتقل إلى **ريش الاشتراكات** في مدخل Azure.</span><span class="sxs-lookup"><span data-stu-id="b4a9d-107">Go to **Subscriptions blade** in Azure portal.</span></span>
2. <span data-ttu-id="b4a9d-108">حدد **الفواتير** ثم **الوصول إلى الفواتير**.</span><span class="sxs-lookup"><span data-stu-id="b4a9d-108">Select **Invoices** and then **Access to invoices**.</span></span>
3. <span data-ttu-id="b4a9d-109">قم بتشغيل access ، متبوعا بحفظ التغييرات ، للسماح للمستخدمين في الأدوار علي نطاق الاشتراكات بتنزيل الفواتير.</span><span class="sxs-lookup"><span data-stu-id="b4a9d-109">Turn on the access, followed by saving the changes, to allow users in subscription-scoped roles to download invoices.</span></span>

> [!NOTE]
> <span data-ttu-id="b4a9d-110">يمكن لمسؤول الحساب أيضا التكوين ليتم إرسال الفواتير عبر البريد الكتروني.</span><span class="sxs-lookup"><span data-stu-id="b4a9d-110">The Account Administrator can also configure to have invoices sent via email.</span></span> <span data-ttu-id="b4a9d-111">لمعرفه المزيد ، راجع [الحصول علي فاتورتك في البريد الكتروني](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?).</span><span class="sxs-lookup"><span data-stu-id="b4a9d-111">To learn more, see [Get your invoice in email](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?).</span></span>

<span data-ttu-id="b4a9d-112">**كيفيه أضافه مستخدمين إلى دور قارئ الفوترة**</span><span class="sxs-lookup"><span data-stu-id="b4a9d-112">**How to add users to the Billing Reader role**</span></span>

1. <span data-ttu-id="b4a9d-113">انتقل إلى **ريش الاشتراكات** في مدخل Azure.</span><span class="sxs-lookup"><span data-stu-id="b4a9d-113">Go to **Subscriptions blade** in Azure portal.</span></span>
2. <span data-ttu-id="b4a9d-114">حدد **التحكم بالوصول (أيام)** ، ثم انقر فوق **أضافه**.</span><span class="sxs-lookup"><span data-stu-id="b4a9d-114">Select **Access control (IAM)** and then click **Add**.</span></span>
3. <span data-ttu-id="b4a9d-115">اختر **قارئ الفوترة** في صفحه **تحديد دور** .</span><span class="sxs-lookup"><span data-stu-id="b4a9d-115">Choose **Billing Reader** in the **Select a role** page.</span></span>
4. <span data-ttu-id="b4a9d-116">اكتب البريد الكتروني للمستخدم الذي تريد دعوته ، ثم انقر فوق **موافق** لإرسال الدعوة.</span><span class="sxs-lookup"><span data-stu-id="b4a9d-116">Type the email of the user you want to invite, and then click **OK** to send the invitation.</span></span>
5. <span data-ttu-id="b4a9d-117">اتبع الإرشادات الواردة في دعوه البريد الكتروني لتسجيل الدخول كقارئ فوتره.</span><span class="sxs-lookup"><span data-stu-id="b4a9d-117">Follow instructions provided in the invite email to log in as a billing reader.</span></span> <span data-ttu-id="b4a9d-118">لمزيد من المعلومات ، راجع [منح حق الوصول إلى الفوترة](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support#opt-in).</span><span class="sxs-lookup"><span data-stu-id="b4a9d-118">For more information, see [Grant access to Billing](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support#opt-in).</span></span>

<span data-ttu-id="b4a9d-119">**المستندات المستحسنة**</span><span class="sxs-lookup"><span data-stu-id="b4a9d-119">**Recommended documents**</span></span>

- [<span data-ttu-id="b4a9d-120">تمكين طرق العرض أو و دا عبر مدخل EA</span><span class="sxs-lookup"><span data-stu-id="b4a9d-120">Enable DA and AO views via EA portal</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/assign-access-acm-data?WT.mc_id=Portal-Microsoft_Azure_Support#enable-access-to-costs-in-the-ea-portal)
- [<span data-ttu-id="b4a9d-121">التكاليف المضمنة في أداره التكاليف</span><span class="sxs-lookup"><span data-stu-id="b4a9d-121">Costs included in Cost Management</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#costs-included-in-cost-management)
- [<span data-ttu-id="b4a9d-122">عروض Microsoft Azure المعتمدة</span><span class="sxs-lookup"><span data-stu-id="b4a9d-122">Supported Microsoft Azure Offers</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#supported-microsoft-azure-offers)
- [<span data-ttu-id="b4a9d-123">مراجعه التكاليف في تحليل التكلفة</span><span class="sxs-lookup"><span data-stu-id="b4a9d-123">Review costs in cost analysis</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support&tabs=azure-portal#review-costs-in-cost-analysis)
- [<span data-ttu-id="b4a9d-124">توفير الوصول إلى معلومات الفوترة</span><span class="sxs-lookup"><span data-stu-id="b4a9d-124">Provide access to billing information</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="b4a9d-125">التحقق من الوصول إلى اتفاقيه عملاء Microsoft</span><span class="sxs-lookup"><span data-stu-id="b4a9d-125">Check access to a Microsoft Customer Agreement</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#check-access-to-a-microsoft-customer-agreement)






