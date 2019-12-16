---
title: قد تحتاج DLP نوع مخصص
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
ms.openlocfilehash: 872fca326065ada002300061c951620b3d9a8d0e
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/15/2019
ms.locfileid: "40052888"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="9d8dc-102">قد تحتاج DLP نوع مخصص</span><span class="sxs-lookup"><span data-stu-id="9d8dc-102">DLP might need a custom type</span></span>

<span data-ttu-id="9d8dc-103">باستخدام نهج منع فقدان البيانات (DLP) ، يمكنك تحديد البيانات الحساسة وحمايتها في مؤسستك.</span><span class="sxs-lookup"><span data-stu-id="9d8dc-103">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="9d8dc-104">في بعض وحدات السيناريو ، قد تحتاج إلى إنشاء نوع المعلومات الحساسة **المخصصة** الخاصة بك لحماية بيانات مؤسستك.</span><span class="sxs-lookup"><span data-stu-id="9d8dc-104">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="9d8dc-105">علي سبيل المثال ، قد تحتاج مؤسستك إلى تحديد وحماية معرفات الموظفين أو البيانات الأخرى في بعض التنسيقات الخاصة بالمؤسسة. إذا كان الأمر كذلك ، راجع المقالات التالية للحصول علي مزيد من المعلومات.</span><span class="sxs-lookup"><span data-stu-id="9d8dc-105">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="9d8dc-106">**تخصيص نوع معلومات حساس مضمن**</span><span class="sxs-lookup"><span data-stu-id="9d8dc-106">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="9d8dc-107">إذا كان نوع المعلومات الحساسة المضمنة يلبي الاحتياجات الخاصة بك مع عدد قليل من القرص ، يمكنك [تخصيص نوع المعلومات الحساسة المضمنة](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="9d8dc-107">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="9d8dc-108">علي سبيل المثال ، يمكنك أضافه أو أزاله الكلمات الرئيسية ، أو أضافه أو أزاله الادله الداعمة مثل التاريخ أو العنوان.</span><span class="sxs-lookup"><span data-stu-id="9d8dc-108">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="9d8dc-109">**إنشاء نوع معلومات حساسة مخصصه**</span><span class="sxs-lookup"><span data-stu-id="9d8dc-109">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="9d8dc-110">ولكن إذا كنت بحاجه إلى تحديد وحماية نوع مختلف من المعلومات الحساسة تماما ، يمكنك [إنشاء نوع معلومات حساسة مخصصه](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) في واجهه المستخدم لمركز التوافق & الأمان.</span><span class="sxs-lookup"><span data-stu-id="9d8dc-110">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="9d8dc-111">**إنشاء نوع معلومات حساسة مخصصه في الأمان & PowerShell مركز التوافق**</span><span class="sxs-lookup"><span data-stu-id="9d8dc-111">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="9d8dc-112">وأخيرا ، إذا لم يوفر واجهه المستخدم كافة الخيارات التي تحتاجها ، يمكنك [إنشاء نوع معلومات حساسة مخصصه في الأمان & PowerShell مركز التوافق](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="9d8dc-112">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="9d8dc-113">بالبدء بملف XML ، يمكنك استخدام كل خيار متوفر.</span><span class="sxs-lookup"><span data-stu-id="9d8dc-113">By starting with an XML file, you can use every option available.</span></span>
