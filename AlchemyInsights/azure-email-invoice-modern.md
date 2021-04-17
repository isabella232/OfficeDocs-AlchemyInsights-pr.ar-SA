---
title: فوترة البريد الإلكتروني الحديث لـ Azure
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
- "9003801"
- "6866"
ms.openlocfilehash: 4df8c49880fe638c1659f76edc0905532d091e45
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820813"
---
# <a name="email-invoicing-in-azure"></a><span data-ttu-id="92c56-102">فوترة البريد الإلكتروني في Azure</span><span class="sxs-lookup"><span data-stu-id="92c56-102">Email invoicing in Azure</span></span>

<span data-ttu-id="92c56-103">يجب أن يكون لديك دور المالك أو المساهم في ملف تعريف الفوترة أو حساب الفوترة لتحديث تفضيل فاتورة البريد الإلكتروني.</span><span class="sxs-lookup"><span data-stu-id="92c56-103">You must have an owner or a contributor role on the billing profile or its billing account to update its email invoice preference.</span></span> <span data-ttu-id="92c56-104">بمجرد الاشتراك، سيحصل جميع المستخدمين الذين لديهم أدوار المالك والمساهم وقراء ومدير الفواتير في ملف تعريف الفوترة على فاتورته عبر البريد الإلكتروني.</span><span class="sxs-lookup"><span data-stu-id="92c56-104">Once you have opted-in, all users with an owner, contributor, readers, and invoice manager roles on a billing profile will get its invoice in email.</span></span>

1. <span data-ttu-id="92c56-105">سجّل الدخول إلى [مدخل Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="92c56-105">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="92c56-106">ابحث عن **إدارة التكلفة + الفوترة**.</span><span class="sxs-lookup"><span data-stu-id="92c56-106">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="92c56-107">حدد **الفواتير** في الجهة اليمنى، ثم حدد **فاتورة البريد الإلكتروني** من أعلى الصفحة.</span><span class="sxs-lookup"><span data-stu-id="92c56-107">Select **Invoices** from the left-hand side and then select **Email Invoice** from the top of the page.</span></span>
4. <span data-ttu-id="92c56-108">إذا كان لديك عدة ملفات تعريف فوترة، فحدد ملف تعريف فوترة ثم حدد **اشتراك**.</span><span class="sxs-lookup"><span data-stu-id="92c56-108">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

5. <span data-ttu-id="92c56-109">حدد **تحديث**.</span><span class="sxs-lookup"><span data-stu-id="92c56-109">Select **Update**.</span></span>
6. <span data-ttu-id="92c56-110">إذا كان لديك عدة ملفات تعريف فوترة، فحدد ملف تعريف فوترة ثم حدد **اشتراك**.</span><span class="sxs-lookup"><span data-stu-id="92c56-110">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

<span data-ttu-id="92c56-111">أنت تمنح الآخرين حق الوصول لعرض الفواتير وتنزيلها ودفعها عن طريق تعيين دور مدير الفواتير لملف تعريف فوترة MCA أو MPA.</span><span class="sxs-lookup"><span data-stu-id="92c56-111">You give others access to view, download, and pay invoices by assigning them the invoice manager role for an MCA or MPA billing profile.</span></span> <span data-ttu-id="92c56-112">إذا اشتركت في الحصول على فاتورتك عبر البريد الإلكتروني، فسيحصل المستخدمون أيضًا على الفواتير عبر البريد الإلكتروني.</span><span class="sxs-lookup"><span data-stu-id="92c56-112">If you've opted in to get your invoice in email, users also get the invoices in email.</span></span>

1. <span data-ttu-id="92c56-113">سجّل الدخول إلى [مدخل Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="92c56-113">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="92c56-114">ابحث عن **إدارة التكلفة + الفوترة**.</span><span class="sxs-lookup"><span data-stu-id="92c56-114">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="92c56-115">حدد **ملفات فوترة** من الجانب الأيمن.</span><span class="sxs-lookup"><span data-stu-id="92c56-115">Select **Billing profiles** from the left-hand side.</span></span> <span data-ttu-id="92c56-116">من قائمة ملفات تعريف الفوترة، حدد ملف تعريف الفوترة الذي تريد تعيين دور مدير الفواتير له.</span><span class="sxs-lookup"><span data-stu-id="92c56-116">From the billing profiles list, select a billing profile for which you want to assign an invoice manager role.</span></span>
4. <span data-ttu-id="92c56-117">حدد **التحكم في الوصول (IAM)** من الجانب الأيسر ثم حدد **إضافة** من أعلى الصفحة.</span><span class="sxs-lookup"><span data-stu-id="92c56-117">Select **Access Control (IAM)** from the left-hand side and then select **Add** from the top of the page.</span></span>

<span data-ttu-id="92c56-118">في القائمة المنسدلة «الدور»، حدد **مدير الفواتير**.</span><span class="sxs-lookup"><span data-stu-id="92c56-118">In the Role drop-down list, select **Invoice Manager**.</span></span> <span data-ttu-id="92c56-119">أدخل عنوان البريد الإلكتروني للمستخدم لمنحه حق الوصول.</span><span class="sxs-lookup"><span data-stu-id="92c56-119">Enter the email address of the user to give access.</span></span> <span data-ttu-id="92c56-120">حدد **حفظ** لتعيين الدور.</span><span class="sxs-lookup"><span data-stu-id="92c56-120">Select **Save** to assign the role.</span></span>
