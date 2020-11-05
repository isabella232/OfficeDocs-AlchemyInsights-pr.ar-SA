---
title: فوتره البريد الكتروني في Azure الحديثة
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
- "9003801"
- "6866"
ms.openlocfilehash: 65df6091a97d4937379ded384a78b5d07aa76e42
ms.sourcegitcommit: a5ba4dc8c349ed79147f67b62bde544281f7c106
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 11/03/2020
ms.locfileid: "48921987"
---
# <a name="email-invoicing-in-azure"></a><span data-ttu-id="42f9d-102">فوتره البريد الكتروني في Azure</span><span class="sxs-lookup"><span data-stu-id="42f9d-102">Email invoicing in Azure</span></span>

<span data-ttu-id="42f9d-103">يجب ان يكون لديك مالك أو دور مساهم علي ملف تعريف الفوترة أو حساب الفوترة الخاص به لتحديث تفضيل فاتورة البريد الكتروني الخاص به.</span><span class="sxs-lookup"><span data-stu-id="42f9d-103">You must have an owner or a contributor role on the billing profile or its billing account to update its email invoice preference.</span></span> <span data-ttu-id="42f9d-104">بمجرد ان تقوم بالاشتراك ، سيحصل كل المستخدمين الذين لديهم المالك والمساهمة والقراء وأدوار أداره الفواتير علي ملف تعريف الفوترة علي الفاتورة الخاصة به في البريد الكتروني.</span><span class="sxs-lookup"><span data-stu-id="42f9d-104">Once you have opted-in, all users with an owner, contributor, readers, and invoice manager roles on a billing profile will get its invoice in email.</span></span>

1. <span data-ttu-id="42f9d-105">سجل دخولك إلى [مدخل Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="42f9d-105">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="42f9d-106">البحث عن **أداره التكاليف + الفوترة**.</span><span class="sxs-lookup"><span data-stu-id="42f9d-106">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="42f9d-107">حدد **الفواتير** من الجانب الأيمن ، ثم حدد **فاتورة البريد الكتروني** من اعلي الصفحة.</span><span class="sxs-lookup"><span data-stu-id="42f9d-107">Select **Invoices** from the left-hand side and then select **Email Invoice** from the top of the page.</span></span>
4. <span data-ttu-id="42f9d-108">إذا كان لديك ملفات تعريف فواتير متعددة ، فحدد ملف تعريف الفوترة ، ثم حدد **الموافقة**.</span><span class="sxs-lookup"><span data-stu-id="42f9d-108">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

5. <span data-ttu-id="42f9d-109">حدد **تحديث**.</span><span class="sxs-lookup"><span data-stu-id="42f9d-109">Select **Update**.</span></span>
6. <span data-ttu-id="42f9d-110">إذا كان لديك ملفات تعريف فواتير متعددة ، فحدد ملف تعريف الفوترة ، ثم حدد **الموافقة**.</span><span class="sxs-lookup"><span data-stu-id="42f9d-110">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

<span data-ttu-id="42f9d-111">يمكنك منح الآخرين امكانيه الوصول إلى عرض الفواتير وتنزيلها ودفعها عن طريق تعيين دور مدير الفواتير لملف تعريف الفوترة في MCA أو MPA.</span><span class="sxs-lookup"><span data-stu-id="42f9d-111">You give others access to view, download, and pay invoices by assigning them the invoice manager role for an MCA or MPA billing profile.</span></span> <span data-ttu-id="42f9d-112">إذا قمت بالاشتراك للحصول علي فاتورتك في البريد الكتروني ، سيتلقى المستخدمون أيضا الفواتير في البريد الكتروني.</span><span class="sxs-lookup"><span data-stu-id="42f9d-112">If you've opted in to get your invoice in email, users also get the invoices in email.</span></span>

1. <span data-ttu-id="42f9d-113">سجل دخولك إلى [مدخل Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="42f9d-113">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="42f9d-114">البحث عن **أداره التكاليف + الفوترة**.</span><span class="sxs-lookup"><span data-stu-id="42f9d-114">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="42f9d-115">حدد **ملفات تعريف الفوترة** من الجانب الأيمن.</span><span class="sxs-lookup"><span data-stu-id="42f9d-115">Select **Billing profiles** from the left-hand side.</span></span> <span data-ttu-id="42f9d-116">من القائمة ملفات تعريف الفواتير ، حدد ملف تعريف الفوترة الذي تريد تعيين دور مدير فاتورة له.</span><span class="sxs-lookup"><span data-stu-id="42f9d-116">From the billing profiles list, select a billing profile for which you want to assign an invoice manager role.</span></span>
4. <span data-ttu-id="42f9d-117">حدد **التحكم بالوصول (أيام)** من الجانب الأيمن ، ثم حدد **أضافه** من اعلي الصفحة.</span><span class="sxs-lookup"><span data-stu-id="42f9d-117">Select **Access Control (IAM)** from the left-hand side and then select **Add** from the top of the page.</span></span>

<span data-ttu-id="42f9d-118">في القائمة المنسدلة الدور ، حدد **مدير الفواتير**.</span><span class="sxs-lookup"><span data-stu-id="42f9d-118">In the Role drop-down list, select **Invoice Manager**.</span></span> <span data-ttu-id="42f9d-119">ادخل عنوان البريد الكتروني الخاص بالمستخدم لمنح حق الوصول.</span><span class="sxs-lookup"><span data-stu-id="42f9d-119">Enter the email address of the user to give access.</span></span> <span data-ttu-id="42f9d-120">حدد **حفظ** لتعيين الدور.</span><span class="sxs-lookup"><span data-stu-id="42f9d-120">Select **Save** to assign the role.</span></span>
