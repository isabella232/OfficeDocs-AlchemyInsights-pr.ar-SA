---
title: قد يحتاج DLP إلى نوع مخصص
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: b83bb77383e2ae7e78c31f35c972182c54487c60
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704476"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="209e4-102">قد يحتاج DLP إلى نوع مخصص</span><span class="sxs-lookup"><span data-stu-id="209e4-102">DLP might need a custom type</span></span>

<span data-ttu-id="209e4-103">**هام**: خلال هذه الأوقات غير المسبوقة، نقوم باتخاذ الخطوات اللازمة لضمان توفر خدمات SharePoint Online و OneDrive بشكل كبير – الرجاء زيارة [تعديلات الميزات المؤقتة لـ SharePoint Online](https://aka.ms/ODSPAdjustments) للحصول على مزيد من المعلومات.</span><span class="sxs-lookup"><span data-stu-id="209e4-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="209e4-104">**قد يتطلب DLP نوع معلومات مخصصة**</span><span class="sxs-lookup"><span data-stu-id="209e4-104">**DLP may require a custom information type**</span></span>

<span data-ttu-id="209e4-105">باستخدام سياسة منع فقدان البيانات (DLP) ، يمكنك تحديد البيانات الحساسة وحمايتها في مؤسستك.</span><span class="sxs-lookup"><span data-stu-id="209e4-105">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="209e4-106">في بعض السيناريوهات، قد تحتاج إلى إنشاء نوع معلومات حساسة **مخصصة** لحماية بيانات مؤسستك.</span><span class="sxs-lookup"><span data-stu-id="209e4-106">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="209e4-107">على سبيل المثال، قد تحتاج مؤسستك إلى تحديد وحماية هوية الموظفين أو البيانات الأخرى بتنسيق معين لمؤسستك. إذا كان الأمر كذلك، راجع المقالات التالية لمزيد من المعلومات.</span><span class="sxs-lookup"><span data-stu-id="209e4-107">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="209e4-108">**تخصيص نوع معلومات حساسة مدمج**</span><span class="sxs-lookup"><span data-stu-id="209e4-108">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="209e4-109">إذا كان نوع المعلومات الحساسة المدمج يلبي احتياجاتك مع بعض التعديلات فقط، يمكنك [تخصيص نوع معلومات حساسة مضمنة.](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type)</span><span class="sxs-lookup"><span data-stu-id="209e4-109">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="209e4-110">على سبيل المثال، يمكنك إضافة كلمات رئيسية أو إزالتها، أو إضافة أو إزالة أدلة داعمة مثل تاريخ أو عنوان.</span><span class="sxs-lookup"><span data-stu-id="209e4-110">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="209e4-111">**إنشاء نوع معلومات حساسة مخصصة**</span><span class="sxs-lookup"><span data-stu-id="209e4-111">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="209e4-112">ولكن إذا كنت بحاجة إلى تحديد وحماية نوع مختلف من المعلومات الحساسة تمامًا، يمكنك [إنشاء نوع معلومات حساسة مخصصة](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) في واجهة المستخدم لمركز التوافق & الأمان.</span><span class="sxs-lookup"><span data-stu-id="209e4-112">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="209e4-113">**إنشاء نوع معلومات حساسة مخصصة في مركز التوافق & الأمان PowerShell**</span><span class="sxs-lookup"><span data-stu-id="209e4-113">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="209e4-114">أخيرًا، إذا لم توفر واجهة المستخدم جميع الخيارات التي تحتاجها، يمكنك [إنشاء نوع معلومات حساسة مخصصة في مركز الأمان & الامتثال PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="209e4-114">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="209e4-115">من خلال البدء بملف XML، يمكنك استخدام كل خيار متاح.</span><span class="sxs-lookup"><span data-stu-id="209e4-115">By starting with an XML file, you can use every option available.</span></span>
