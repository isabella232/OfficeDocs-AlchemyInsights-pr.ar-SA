---
title: تكوين نقطة اتصال الخدمة (SCP)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9732"
- "9003244"
ms.openlocfilehash: 9d733a1a0a3b8d92bdd5477a8978b6fbeede9653
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/19/2021
ms.locfileid: "51034795"
---
# <a name="configure-service-connection-point-scp"></a><span data-ttu-id="d1c3c-102">تكوين نقطة اتصال الخدمة (SCP)</span><span class="sxs-lookup"><span data-stu-id="d1c3c-102">Configure Service connection Point (SCP)</span></span>

<span data-ttu-id="d1c3c-103">**DSREG_AUTOJOIN_ADCONFIG_READ_FAILED (0x801c001d/-2145648611)**</span><span class="sxs-lookup"><span data-stu-id="d1c3c-103">**DSREG_AUTOJOIN_ADCONFIG_READ_FAILED (0x801c001d/-2145648611)**</span></span>

- <span data-ttu-id="d1c3c-104">**السبب**: يتعذر قراءة كائن SCP والحصول على معلومات مستأجر Azure AD</span><span class="sxs-lookup"><span data-stu-id="d1c3c-104">**Reason**: Unable to read the SCP object and get the Azure AD tenant information</span></span>
- <span data-ttu-id="d1c3c-105">**الدقة**: الرجوع إلى المقطع [تكوين نقطة اتصال الخدمة](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains#configure-hybrid-azure-ad-join)</span><span class="sxs-lookup"><span data-stu-id="d1c3c-105">**Resolution**: Refer to the section [Configure a Service Connection Point](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains#configure-hybrid-azure-ad-join)</span></span>


<span data-ttu-id="d1c3c-106">**خطة الإجراء**</span><span class="sxs-lookup"><span data-stu-id="d1c3c-106">**Action plan**</span></span>

- <span data-ttu-id="d1c3c-107">تحقق مما إذا كان الجهاز قد استلم "GPO" للتحقق من الصحة الذي تم التحكم به.</span><span class="sxs-lookup"><span data-stu-id="d1c3c-107">Check whether the device has received the GPO for the controlled validation.</span></span>
- <span data-ttu-id="d1c3c-108">تأكد من أن مكتب GPO قد أنشأ مفاتيح التسجيل.</span><span class="sxs-lookup"><span data-stu-id="d1c3c-108">Ensure that the GPO has created the registry keys.</span></span>
- <span data-ttu-id="d1c3c-109">تأكد من أن لديك مفتاحين تم إنشاؤهما باستخدام مجال Onmicrosoft وم ID الدليل.</span><span class="sxs-lookup"><span data-stu-id="d1c3c-109">Ensure that you have 2 keys created with your Directory ID and onmicrosoft domain.</span></span>

<span data-ttu-id="d1c3c-110">**تكوين إعداد التسجيل من جانب العميل ل SCP**</span><span class="sxs-lookup"><span data-stu-id="d1c3c-110">**Configure client-side registry setting for SCP**</span></span>

<span data-ttu-id="d1c3c-111">استخدم المثال التالي لإنشاء كائن نهج المجموعة (GPO) لنشر إعداد تسجيل ينشئ إدخال SCP في سجل أجهزتك.</span><span class="sxs-lookup"><span data-stu-id="d1c3c-111">Use the following example to create a Group Policy Object (GPO) to deploy a registry setting that configures an SCP entry in the registry of your devices.</span></span>

1. <span data-ttu-id="d1c3c-112">افتح وحدة تحكم "إدارة نهج المجموعة" وأنشئ "نهج نهج المجموعة" جديدا في مجالك.</span><span class="sxs-lookup"><span data-stu-id="d1c3c-112">Open a Group Policy Management console and create a new GPO in your domain.</span></span>
     - <span data-ttu-id="d1c3c-113">قم بتوفير اسم ل GPO الذي تم إنشاؤه حديثا (على سبيل المثال، ClientSideSCP)</span><span class="sxs-lookup"><span data-stu-id="d1c3c-113">Provide your newly created GPO a name (for example, ClientSideSCP)</span></span>

2. <span data-ttu-id="d1c3c-114">قم بتحرير GPO وحدد موقع المسار التالي: تكوين الكمبيوتر > التفضيلات > **Windows > السجل.**</span><span class="sxs-lookup"><span data-stu-id="d1c3c-114">Edit the GPO and locate the following path: **Computer Configuration > Preferences > Windows Settings > Registry**.</span></span>

3. <span data-ttu-id="d1c3c-115">انقر بضغطة زر الماوس **الأيمن فوق التسجيل** وحدد عنصر > السجل **الجديد.**</span><span class="sxs-lookup"><span data-stu-id="d1c3c-115">Right-click on **Registry** and select **New > Registry Item**.</span></span>

4. <span data-ttu-id="d1c3c-116">على علامة **التبويب عام،** قم بتكوين ما يلي:</span><span class="sxs-lookup"><span data-stu-id="d1c3c-116">On the **General** tab, configure the following:</span></span>
  
- <span data-ttu-id="d1c3c-117">**الإجراء**: تحديث</span><span class="sxs-lookup"><span data-stu-id="d1c3c-117">**Action**: Update</span></span>
    
- <span data-ttu-id="d1c3c-118">**الخلية**: HKEY_LOCAL_MACHINE</span><span class="sxs-lookup"><span data-stu-id="d1c3c-118">**Hive**: HKEY_LOCAL_MACHINE</span></span>
    
- <span data-ttu-id="d1c3c-119">**مسار المفتاح**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span><span class="sxs-lookup"><span data-stu-id="d1c3c-119">**Key Path**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span></span>
    
- <span data-ttu-id="d1c3c-120">**اسم القيمة**: TenantId</span><span class="sxs-lookup"><span data-stu-id="d1c3c-120">**Value name**: TenantId</span></span>
    
- <span data-ttu-id="d1c3c-121">**نوع القيمة**: REG_SZ</span><span class="sxs-lookup"><span data-stu-id="d1c3c-121">**Value type**: REG_SZ</span></span>
    
- <span data-ttu-id="d1c3c-122">**بيانات القيمة**: المثيل GUID أو الدليل لمثيل Azure AD (يمكن العثور على هذه القيمة في مدخل **Azure > Azure Active Directory > Properties > الدليل**)</span><span class="sxs-lookup"><span data-stu-id="d1c3c-122">**Value data**: The GUID or Directory ID of your Azure AD instance (This value can be found in **Azure portal > Azure Active Directory > Properties > Directory ID**)</span></span>
 
- <span data-ttu-id="d1c3c-123">انقر فوق **موافق**.</span><span class="sxs-lookup"><span data-stu-id="d1c3c-123">Click **OK**.</span></span>
 
5. <span data-ttu-id="d1c3c-124">انقر بضغطة زر الماوس **الأيمن فوق التسجيل** وحدد عنصر > السجل **الجديد.**</span><span class="sxs-lookup"><span data-stu-id="d1c3c-124">Right-click on **Registry** and select **New > Registry Item**.</span></span>

6. <span data-ttu-id="d1c3c-125">على علامة **التبويب عام،** قم بتكوين ما يلي:</span><span class="sxs-lookup"><span data-stu-id="d1c3c-125">On the **General** tab, configure the following:</span></span>
  
- <span data-ttu-id="d1c3c-126">**الإجراء**: تحديث</span><span class="sxs-lookup"><span data-stu-id="d1c3c-126">**Action**: Update</span></span>
    
- <span data-ttu-id="d1c3c-127">**الخلية**: HKEY_LOCAL_MACHINE</span><span class="sxs-lookup"><span data-stu-id="d1c3c-127">**Hive**: HKEY_LOCAL_MACHINE</span></span>
    
- <span data-ttu-id="d1c3c-128">**مسار المفتاح**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span><span class="sxs-lookup"><span data-stu-id="d1c3c-128">**Key Path**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span></span>
    
- <span data-ttu-id="d1c3c-129">**اسم القيمة**: TenantName</span><span class="sxs-lookup"><span data-stu-id="d1c3c-129">**Value name**: TenantName</span></span>
    
- <span data-ttu-id="d1c3c-130">**نوع القيمة**: REG_SZ</span><span class="sxs-lookup"><span data-stu-id="d1c3c-130">**Value type**: REG_SZ</span></span>
    
- <span data-ttu-id="d1c3c-131">**بيانات القيمة**: اسم المجال الذي تم التحقق منه إذا كنت تستخدم بيئة متكاتف مثل AD FS.</span><span class="sxs-lookup"><span data-stu-id="d1c3c-131">**Value data**: Your verified domain name if you are using federated environment such as AD FS.</span></span> <span data-ttu-id="d1c3c-132">اسم المجال المتحقق منه أو اسم مجالك onmicrosoft.com (على سبيل المثال، contoso.onmicrosoft).com إذا كنت تستخدم بيئة مدارة</span><span class="sxs-lookup"><span data-stu-id="d1c3c-132">Your verified domain name or your onmicrosoft.com domain name (for example, contoso.onmicrosoft).com if you are using managed environment</span></span>

- <span data-ttu-id="d1c3c-133">انقر فوق **موافق**.</span><span class="sxs-lookup"><span data-stu-id="d1c3c-133">Click **OK**.</span></span>

7. <span data-ttu-id="d1c3c-134">أغلق محرر GPO الذي تم إنشاؤه حديثا.</span><span class="sxs-lookup"><span data-stu-id="d1c3c-134">Close the editor for the newly created GPO.</span></span>

8. <span data-ttu-id="d1c3c-135">ربط "مجموعة معلومات المجموعة" التي تم إنشاؤها حديثا ب OU المطلوب الذي يحتوي على أجهزة الكمبيوتر المنضمة إلى المجال والتي تنتمي إلى عدد السكان الذي تم التحكم في طرحه.</span><span class="sxs-lookup"><span data-stu-id="d1c3c-135">Link the newly created GPO to the desired OU containing domain-joined computers that belong to your controlled rollout population.</span></span>

<span data-ttu-id="d1c3c-136">لمزيد من المعلومات، راجع التحقق من الصحة المتحكم به لضم [Azure AD المختلط - Azure AD | أجهزة Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control) وإصلاحها المختلطة  [التي انضم إليها Azure Active Directory | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current).</span><span class="sxs-lookup"><span data-stu-id="d1c3c-136">For more information, see [Controlled validation of hybrid Azure AD join - Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control) and  [Troubleshooting hybrid Azure Active Directory joined devices | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current).</span></span>









