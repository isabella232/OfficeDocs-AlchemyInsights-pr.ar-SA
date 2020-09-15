---
title: قد يحتاج DLP إلى نوع مخصص
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 72b16d437f97de27cbdc364f022c3e2059b31ef0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47712171"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="b6c60-102">قد يحتاج DLP إلى نوع مخصص</span><span class="sxs-lookup"><span data-stu-id="b6c60-102">DLP might need a custom type</span></span>

<span data-ttu-id="b6c60-103">**هام**: خلال هذه الأوقات غير المسبوقة، نقوم باتخاذ الخطوات اللازمة لضمان توفر خدمات SharePoint Online و OneDrive بشكل كبير – الرجاء زيارة [تعديلات الميزات المؤقتة لـ SharePoint Online](https://aka.ms/ODSPAdjustments) للحصول على مزيد من المعلومات.</span><span class="sxs-lookup"><span data-stu-id="b6c60-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="b6c60-104">**قد يتطلب DLP نوع معلومات مخصصا**</span><span class="sxs-lookup"><span data-stu-id="b6c60-104">**DLP may require a custom information type**</span></span>

<span data-ttu-id="b6c60-105">باستخدام نهج تفادي فقدان البيانات (DLP) ، يمكنك تحديد البيانات الحساسة وحمايتها في مؤسستك.</span><span class="sxs-lookup"><span data-stu-id="b6c60-105">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="b6c60-106">في بعض السيناريوهات ، قد تحتاج إلى إنشاء نوع المعلومات **الحساسة المخصصة** لحماية بيانات المؤسسة.</span><span class="sxs-lookup"><span data-stu-id="b6c60-106">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="b6c60-107">علي سبيل المثال ، قد تحتاج مؤسستك إلى تحديد معرفات الموظفين أو البيانات الأخرى وحمايتها بتنسيق مخصص لمؤسسك. إذا كان الأمر كذلك ، فراجع المقالات التالية للحصول علي مزيد من المعلومات.</span><span class="sxs-lookup"><span data-stu-id="b6c60-107">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="b6c60-108">**تخصيص نوع المعلومات الحساسة المضمن**</span><span class="sxs-lookup"><span data-stu-id="b6c60-108">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="b6c60-109">إذا كان نوع المعلومات الحساسة المضمن يفي باحتياجاتك باستخدام بضع نهائي فقط ، فيمكنك [تخصيص نوع معلومات مضمن](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="b6c60-109">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="b6c60-110">علي سبيل المثال ، يمكنك أضافه الكلمات الاساسيه أو ازالتها ، أو أضافه أو أزاله الادله المعتمدة مثل التاريخ أو العنوان.</span><span class="sxs-lookup"><span data-stu-id="b6c60-110">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="b6c60-111">**إنشاء نوع معلومات حساس مخصص**</span><span class="sxs-lookup"><span data-stu-id="b6c60-111">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="b6c60-112">ولكن إذا كنت بحاجه إلى تحديد نوع آخر من المعلومات الهامه وحمايته تماما ، فيمكنك [إنشاء نوع معلومات حساس مخصص](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) في واجهه المستخدم الخاصة بمركز توافق & الأمان.</span><span class="sxs-lookup"><span data-stu-id="b6c60-112">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="b6c60-113">**إنشاء نوع معلومات حساس مخصص في مركز توافق & الأمان PowerShell**</span><span class="sxs-lookup"><span data-stu-id="b6c60-113">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="b6c60-114">وأخيرا ، إذا لم توفر واجهه المستخدم كل الخيارات التي تحتاج اليها ، فيمكنك [إنشاء نوع معلومات حساس مخصص في "مركز توافق ال& الأمان"](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="b6c60-114">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="b6c60-115">بالبدء باستخدام ملف XML ، يمكنك استخدام كل خيار متوفر.</span><span class="sxs-lookup"><span data-stu-id="b6c60-115">By starting with an XML file, you can use every option available.</span></span>
