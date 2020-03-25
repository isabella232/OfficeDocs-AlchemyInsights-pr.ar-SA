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
ms.openlocfilehash: 890bba57bc36c034c507e6124cd6593ef4d92af8
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932645"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="ac05a-102">قد يحتاج DLP إلى نوع مخصص</span><span class="sxs-lookup"><span data-stu-id="ac05a-102">DLP might need a custom type</span></span>

<span data-ttu-id="ac05a-103">**هام:** يعمل العديد من عملاء SharePoint Online و OneDrive على تشغيل تطبيقات مهمة للأعمال مقابل الخدمة التي تعمل في الخلفية.</span><span class="sxs-lookup"><span data-stu-id="ac05a-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="ac05a-104">وتشمل هذه ترحيل المحتوى، منع فقدان البيانات (DLP)، وحلول النسخ الاحتياطي.</span><span class="sxs-lookup"><span data-stu-id="ac05a-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="ac05a-105">خلال هذه الأوقات غير المسبوقة، نتخذ خطوات لضمان أن تظل خدمات SharePoint Online و OneDrive متاحة للغاية وموثوقة للمستخدمين الذين يعتمدون على الخدمة أكثر من أي وقت مضى في سيناريوهات العمل عن بعد.</span><span class="sxs-lookup"><span data-stu-id="ac05a-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="ac05a-106">ولدعم هذا الهدف، قمنا بتنفيذ قيود خنق أكثر صرامة على تطبيقات الخلفية (الترحيل وDLP وحلول النسخ الاحتياطي) خلال ساعات النهار في أيام الأسبوع.</span><span class="sxs-lookup"><span data-stu-id="ac05a-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="ac05a-107">يجب أن تتوقع أن تحقق هذه التطبيقات إنتاجية محدودة جدًا خلال هذه الأوقات.</span><span class="sxs-lookup"><span data-stu-id="ac05a-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="ac05a-108">ومع ذلك ، خلال ساعات المساء وعطلة نهاية الأسبوع للمنطقة ، ستكون الخدمة جاهزة لمعالجة حجم أكبر بكثير من الطلبات من تطبيقات الخلفية.</span><span class="sxs-lookup"><span data-stu-id="ac05a-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="ac05a-109">**قد يتطلب DLP نوع معلومات مخصصة**</span><span class="sxs-lookup"><span data-stu-id="ac05a-109">**DLP may require a custom information type**</span></span>

<span data-ttu-id="ac05a-110">باستخدام سياسة منع فقدان البيانات (DLP) ، يمكنك تحديد البيانات الحساسة وحمايتها في مؤسستك.</span><span class="sxs-lookup"><span data-stu-id="ac05a-110">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="ac05a-111">في بعض السيناريوهات، قد تحتاج إلى إنشاء نوع معلومات حساسة **مخصصة** لحماية بيانات مؤسستك.</span><span class="sxs-lookup"><span data-stu-id="ac05a-111">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="ac05a-112">على سبيل المثال، قد تحتاج مؤسستك إلى تحديد وحماية هوية الموظفين أو البيانات الأخرى بتنسيق معين لمؤسستك. إذا كان الأمر كذلك، راجع المقالات التالية لمزيد من المعلومات.</span><span class="sxs-lookup"><span data-stu-id="ac05a-112">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="ac05a-113">**تخصيص نوع معلومات حساسة مدمج**</span><span class="sxs-lookup"><span data-stu-id="ac05a-113">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="ac05a-114">إذا كان نوع المعلومات الحساسة المدمج يلبي احتياجاتك مع بعض التعديلات فقط، يمكنك [تخصيص نوع معلومات حساسة مضمنة.](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type)</span><span class="sxs-lookup"><span data-stu-id="ac05a-114">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="ac05a-115">على سبيل المثال، يمكنك إضافة كلمات رئيسية أو إزالتها، أو إضافة أو إزالة أدلة داعمة مثل تاريخ أو عنوان.</span><span class="sxs-lookup"><span data-stu-id="ac05a-115">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="ac05a-116">**إنشاء نوع معلومات حساسة مخصصة**</span><span class="sxs-lookup"><span data-stu-id="ac05a-116">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="ac05a-117">ولكن إذا كنت بحاجة إلى تحديد وحماية نوع مختلف من المعلومات الحساسة تمامًا، يمكنك [إنشاء نوع معلومات حساسة مخصصة](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) في واجهة المستخدم لمركز التوافق & الأمان.</span><span class="sxs-lookup"><span data-stu-id="ac05a-117">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="ac05a-118">**إنشاء نوع معلومات حساسة مخصصة في مركز التوافق & الأمان PowerShell**</span><span class="sxs-lookup"><span data-stu-id="ac05a-118">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="ac05a-119">أخيرًا، إذا لم توفر واجهة المستخدم جميع الخيارات التي تحتاجها، يمكنك [إنشاء نوع معلومات حساسة مخصصة في مركز الأمان & الامتثال PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="ac05a-119">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="ac05a-120">من خلال البدء بملف XML، يمكنك استخدام كل خيار متاح.</span><span class="sxs-lookup"><span data-stu-id="ac05a-120">By starting with an XML file, you can use every option available.</span></span>
