---
title: مشكلة في عامل تصفية السمات وتصفيتها
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8470"
- "9004687"
ms.openlocfilehash: 78df24c0d8a670d678e26879cf81476f1ae9b92d
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/04/2021
ms.locfileid: "50480841"
---
# <a name="problem-with-attribute-and-scoping-filter"></a><span data-ttu-id="b59ce-102">مشكلة في عامل تصفية السمات وتصفيتها</span><span class="sxs-lookup"><span data-stu-id="b59ce-102">Problem with attribute and scoping filter</span></span>

<span data-ttu-id="b59ce-103">**مشكلة في قيم UPN المتضاربة**</span><span class="sxs-lookup"><span data-stu-id="b59ce-103">**Issue with conflicting UPN values**</span></span>

<span data-ttu-id="b59ce-104">يعرض يوم العمل إلى AD User Provisioning Workday to AD User Provisioning رسالة الخطأ **HybridSynchronizationActiveDirectoryUserPrincipalNameNotUnique**.</span><span class="sxs-lookup"><span data-stu-id="b59ce-104">The Workday to AD User Provisioning Workday to AD User Provisioning shows error message **HybridSynchronizationActiveDirectoryUserPrincipalNameNotUnique**.</span></span> <span data-ttu-id="b59ce-105">فشلت العملية لأن قيمة UPN المتوفرة للالإضافة/التعديل ليست فريدة على مستوى الغابات.</span><span class="sxs-lookup"><span data-stu-id="b59ce-105">The operation failed because UPN value provided for addition/modification is not unique forest-wide.</span></span> <span data-ttu-id="b59ce-106">تفاصيل الخطأ: CONSTRAINT_ATT_TYPE **- userPrincipalName.**</span><span class="sxs-lookup"><span data-stu-id="b59ce-106">Error Details: **CONSTRAINT_ATT_TYPE - userPrincipalName**.</span></span>

<span data-ttu-id="b59ce-107">قيمة **userPrincipalName** التي يحاول موصل Workday تعيينها عند إنشاء حساب مستخدم AD موجودة بالفعل في مجال AD الهدف.</span><span class="sxs-lookup"><span data-stu-id="b59ce-107">The **userPrincipalName** value that Workday connector is trying to set when creating the AD user account already exists in the target AD domain.</span></span> <span data-ttu-id="b59ce-108">وهذا يعني أن (1) المستخدم موجود بالفعل وفشل فحص الم ID المطابق للمستخدم أو (2) إنشاء قيمة متعارضة لقاعدة الجيل UPN.</span><span class="sxs-lookup"><span data-stu-id="b59ce-108">This implies that either (1) the user already exists and the matching ID check failed for the user or (2) the UPN generation rule generated a conflicting value.</span></span>

<span data-ttu-id="b59ce-109">فيما يلي خطوات الحل المقترحة:</span><span class="sxs-lookup"><span data-stu-id="b59ce-109">Here are the suggested resolution steps:</span></span>

<span data-ttu-id="b59ce-110">إذا كان المستخدم موجودا بالفعل وفشلت عملية التحقق من الم ID المطابقة في ربط حساب يوم العمل إلى حساب Active Directory، فتحقق مما إذا كانت سمة المرجع المطابقة (عادة ما تكون "المرجع الموظف") في كل من "يوم العمل" و"AD" تتضمن تطابقا دقيقا.</span><span class="sxs-lookup"><span data-stu-id="b59ce-110">If the user already exists and the matching ID check failed to link the Workday account to Active Directory account, then check if the matching ID attribute (typically **employeeID**) in both Workday and AD have an exact match.</span></span> <span data-ttu-id="b59ce-111">إذا لم يكن لديهم تطابق، فهي مشكلة في البيانات يجب إصلاحها.</span><span class="sxs-lookup"><span data-stu-id="b59ce-111">If they don't have a match, it is a data issue that needs to be fixed.</span></span> <span data-ttu-id="b59ce-112">على سبيل المثال، إذا كان "الموظف" في "يوم العمل" هو 001052 وفي AD هو 1052، سيفشل محرك توفير البيانات في ربط الحسابين وسيحاول إنشاء مستخدم موجود بالفعل.</span><span class="sxs-lookup"><span data-stu-id="b59ce-112">For example, if the EmployeeID in Workday is 001052 and in AD it is 1052, then the provisioning engine will fail to link the two accounts and will try to create a user that already exists.</span></span> <span data-ttu-id="b59ce-113">الحل في هذه الحالة هو تغيير قيمة **EmployeeID** في AD لتضمين الأصفار البدلة لجعلها 001052.</span><span class="sxs-lookup"><span data-stu-id="b59ce-113">The solution in this case is to change the **EmployeeID** value in AD to include the leading zeros to make it 001052.</span></span>
<span data-ttu-id="b59ce-114">إذا لم ينشئ التعبير الذي ينشئ UPN قيمة فريدة، **فحددUniqueValue** استخدام دالة إزالة التكرار لإنشاء قيمة فريدة في كل مرة.</span><span class="sxs-lookup"><span data-stu-id="b59ce-114">If the UPN-generating expression is not generating a unique value, consider using the de-duplication function **SelectUniqueValue** to generate a unique value each time.</span></span>

<span data-ttu-id="b59ce-115">**لا يقوم توفير يوم عمل لمستخدم AD بتعيين قيمة سمة المدير لحساب مستخدم AD**</span><span class="sxs-lookup"><span data-stu-id="b59ce-115">**Workday to AD User Provisioning does not set manager attribute value for AD user account**</span></span>

<span data-ttu-id="b59ce-116">لا تعمل مهمة توفير يوم العمل لمستخدم AD على تعيين قيمة **سمة** المدير الخاصة حسابات مستخدمي AD.</span><span class="sxs-lookup"><span data-stu-id="b59ce-116">The Workday to AD User Provisioning job is not setting the **manager** attribute value for AD user accounts.</span></span> <span data-ttu-id="b59ce-117">هناك سيناريوهان محتملان عند رؤية هذا السلوك:</span><span class="sxs-lookup"><span data-stu-id="b59ce-117">There are two possible scenarios when this behavior is seen:</span></span>

1. <span data-ttu-id="b59ce-118">يتعذر حل المدير في يوم العمل إلى حساب مستخدم AD مقابل لأن المدير غير ضمن النطاق.</span><span class="sxs-lookup"><span data-stu-id="b59ce-118">The manager in Workday cannot be resolved to a corresponding AD User account because the manager is not in scope.</span></span>
2. <span data-ttu-id="b59ce-119">في سيناريو **مجالات AD** متعددة، لا يكون المدير في Workday موجودا في المجال نفسه الذي لدى المستخدم.</span><span class="sxs-lookup"><span data-stu-id="b59ce-119">In a **multiple AD domains** scenario, the manager in Workday is not present in the same domain as the user.</span></span>

<span data-ttu-id="b59ce-120">جرب هذه الخطوات لحل المشكلة:</span><span class="sxs-lookup"><span data-stu-id="b59ce-120">Try these steps to resolve the issue:</span></span>

1. <span data-ttu-id="b59ce-121">إذا قمت بتعريف عوامل تصفية تحديد النطاق، فتحقق أولا مما إذا كان المدير في النطاق وأن المدير يلبي عبارة تحديد النطاق.</span><span class="sxs-lookup"><span data-stu-id="b59ce-121">If you have defined scoping filters, first check if the manager is in scope and that it satisfies the scoping clause.</span></span> <span data-ttu-id="b59ce-122">إذا لم يوفي المدير عامل تصفية تحديد النطاق، فغير عامل التصفية بحيث يكون المدير أيضا في نطاق عملية توفير.</span><span class="sxs-lookup"><span data-stu-id="b59ce-122">If the manager does not satisfy the scoping filter, change the filter so that the manager is also in scope of the provisioning operation.</span></span>
2. <span data-ttu-id="b59ce-123">إذا كان لديك عدة مجالات AD، فإن الموصل لديه قيد معروف وهو عدم القدرة على حل مراجع إدارة المجالات المتعددة.</span><span class="sxs-lookup"><span data-stu-id="b59ce-123">If you have multiple AD domains, then the connector has a known limitation of inability to resolve cross-domain manager references.</span></span>

<span data-ttu-id="b59ce-124">لمزيد من التفاصيل حول تكوين يوم العمل للتكوين التلقائي، راجع البرنامج [التعليمي: تكوين يوم](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)عمل للتكوين التلقائي للمستخدم.</span><span class="sxs-lookup"><span data-stu-id="b59ce-124">For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>













