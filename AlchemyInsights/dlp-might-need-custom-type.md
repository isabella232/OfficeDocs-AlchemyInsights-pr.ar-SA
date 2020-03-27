---
title: قد يحتاج DLP إلى نوع مخصص
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: ''
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 87fcb5c3cc9ccd525265097b66d9d9b3a85c5feb
ms.sourcegitcommit: d108a2da2f5dab05246e30b5108cca5173e09051
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/26/2020
ms.locfileid: "42977257"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="d7c82-102">قد يحتاج DLP إلى نوع مخصص</span><span class="sxs-lookup"><span data-stu-id="d7c82-102">DLP might need a custom type</span></span>

<span data-ttu-id="d7c82-103">**هام:** خلال هذه الأوقات غير المسبوقة، نتخذ خطوات لضمان أن تظل خدمات SharePoint Online و OneDrive متاحة للغاية - يرجى زيارة [SharePoint Online تعديلات الميزة المؤقتة](https://aka.ms/ODSPAdjustments) للحصول على مزيد من المعلومات.</span><span class="sxs-lookup"><span data-stu-id="d7c82-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="d7c82-104">**قد يتطلب DLP نوع معلومات مخصصة**</span><span class="sxs-lookup"><span data-stu-id="d7c82-104">**DLP may require a custom information type**</span></span>

<span data-ttu-id="d7c82-105">باستخدام سياسة منع فقدان البيانات (DLP) ، يمكنك تحديد البيانات الحساسة وحمايتها في مؤسستك.</span><span class="sxs-lookup"><span data-stu-id="d7c82-105">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="d7c82-106">في بعض السيناريوهات، قد تحتاج إلى إنشاء نوع معلومات حساسة **مخصصة** لحماية بيانات مؤسستك.</span><span class="sxs-lookup"><span data-stu-id="d7c82-106">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="d7c82-107">على سبيل المثال، قد تحتاج مؤسستك إلى تحديد وحماية هوية الموظفين أو البيانات الأخرى بتنسيق معين لمؤسستك. إذا كان الأمر كذلك، راجع المقالات التالية لمزيد من المعلومات.</span><span class="sxs-lookup"><span data-stu-id="d7c82-107">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="d7c82-108">**تخصيص نوع معلومات حساسة مدمج**</span><span class="sxs-lookup"><span data-stu-id="d7c82-108">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="d7c82-109">إذا كان نوع المعلومات الحساسة المدمج يلبي احتياجاتك مع بعض التعديلات فقط، يمكنك [تخصيص نوع معلومات حساسة مضمنة.](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type)</span><span class="sxs-lookup"><span data-stu-id="d7c82-109">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="d7c82-110">على سبيل المثال، يمكنك إضافة كلمات رئيسية أو إزالتها، أو إضافة أو إزالة أدلة داعمة مثل تاريخ أو عنوان.</span><span class="sxs-lookup"><span data-stu-id="d7c82-110">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="d7c82-111">**إنشاء نوع معلومات حساسة مخصصة**</span><span class="sxs-lookup"><span data-stu-id="d7c82-111">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="d7c82-112">ولكن إذا كنت بحاجة إلى تحديد وحماية نوع مختلف من المعلومات الحساسة تمامًا، يمكنك [إنشاء نوع معلومات حساسة مخصصة](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) في واجهة المستخدم لمركز التوافق & الأمان.</span><span class="sxs-lookup"><span data-stu-id="d7c82-112">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="d7c82-113">**إنشاء نوع معلومات حساسة مخصصة في مركز التوافق & الأمان PowerShell**</span><span class="sxs-lookup"><span data-stu-id="d7c82-113">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="d7c82-114">أخيرًا، إذا لم توفر واجهة المستخدم جميع الخيارات التي تحتاجها، يمكنك [إنشاء نوع معلومات حساسة مخصصة في مركز الأمان & الامتثال PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="d7c82-114">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="d7c82-115">من خلال البدء بملف XML، يمكنك استخدام كل خيار متاح.</span><span class="sxs-lookup"><span data-stu-id="d7c82-115">By starting with an XML file, you can use every option available.</span></span>
