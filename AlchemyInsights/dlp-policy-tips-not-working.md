---
title: نصائح نهج DLP لا تعمل
ms.author: deniseb
author: denisebmsft
manager: laurawims
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: c03d30be-474a-4a34-b3c0-240eb2a2c466
ms.custom:
- "1428"
- "3200001"
ms.openlocfilehash: 51b4472fa721443192eb542cac45965df67634df
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932573"
---
# <a name="dlp-policy-tip-issues"></a><span data-ttu-id="2ce9d-102">مشكلات تلميح نهج DLP</span><span class="sxs-lookup"><span data-stu-id="2ce9d-102">DLP Policy Tip issues</span></span>

<span data-ttu-id="2ce9d-103">**هام:** يعمل العديد من عملاء SharePoint Online و OneDrive على تشغيل تطبيقات مهمة للأعمال مقابل الخدمة التي تعمل في الخلفية.</span><span class="sxs-lookup"><span data-stu-id="2ce9d-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="2ce9d-104">وتشمل هذه ترحيل المحتوى، منع فقدان البيانات (DLP)، وحلول النسخ الاحتياطي.</span><span class="sxs-lookup"><span data-stu-id="2ce9d-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="2ce9d-105">خلال هذه الأوقات غير المسبوقة، نتخذ خطوات لضمان أن تظل خدمات SharePoint Online و OneDrive متاحة للغاية وموثوقة للمستخدمين الذين يعتمدون على الخدمة أكثر من أي وقت مضى في سيناريوهات العمل عن بعد.</span><span class="sxs-lookup"><span data-stu-id="2ce9d-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="2ce9d-106">ولدعم هذا الهدف، قمنا بتنفيذ قيود خنق أكثر صرامة على تطبيقات الخلفية (الترحيل وDLP وحلول النسخ الاحتياطي) خلال ساعات النهار في أيام الأسبوع.</span><span class="sxs-lookup"><span data-stu-id="2ce9d-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="2ce9d-107">يجب أن تتوقع أن تحقق هذه التطبيقات إنتاجية محدودة جدًا خلال هذه الأوقات.</span><span class="sxs-lookup"><span data-stu-id="2ce9d-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="2ce9d-108">ومع ذلك ، خلال ساعات المساء وعطلة نهاية الأسبوع للمنطقة ، ستكون الخدمة جاهزة لمعالجة حجم أكبر بكثير من الطلبات من تطبيقات الخلفية.</span><span class="sxs-lookup"><span data-stu-id="2ce9d-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="2ce9d-109">**نصائح سياسة DLP**</span><span class="sxs-lookup"><span data-stu-id="2ce9d-109">**DLP policy tips**</span></span>

<span data-ttu-id="2ce9d-110">عند استخدام **نُهج DLP،** يمكن إعلام المستخدمين بانتهاك النهج باستخدام **نصائح النهج.**</span><span class="sxs-lookup"><span data-stu-id="2ce9d-110">When using **DLP policies**, users can be notified of a policy violation with **policy tips**.</span></span> <span data-ttu-id="2ce9d-111">يمكن للمسؤولين تكوين تلميحات النهج لعرضأثناء اختبار نهج DLP أو عندما يكون النهج في وضع التطبيق الكامل.</span><span class="sxs-lookup"><span data-stu-id="2ce9d-111">Admins can configure policy tips to display while testing their DLP policy or when the policy is in full enforcement mode.</span></span>
  
<span data-ttu-id="2ce9d-112">لتكوين تلميحات النهج حول نهج DLP الخاص بك في مركز الأمان والامتثال في وضع التنفيذ الكامل، قم بما يلي:</span><span class="sxs-lookup"><span data-stu-id="2ce9d-112">To configure policy tips on your DLP policy in the Security and Compliance center in full enforcement mode, do the following:</span></span>
  
- <span data-ttu-id="2ce9d-113">تأكد من **تمكين** تلميحات السياسة على قاعدة DLP باستخدام الخطوات [هنا](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips).</span><span class="sxs-lookup"><span data-stu-id="2ce9d-113">Ensure policy tips have been **enabled** on the DLP rule using the steps [here](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips).</span></span>

- <span data-ttu-id="2ce9d-114">تأكد من **تطابق المحتوى** الخاص بك مع ما هو **مطلوب** لتشغيل القاعدة الموضحة في هذه المقالة [هنا](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span><span class="sxs-lookup"><span data-stu-id="2ce9d-114">Ensure your **content matches** what is **required** to trigger the rule outlined in this article [here](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="2ce9d-115">يتم عرض تلميحات النهج في كل من OWA و Outlook.</span><span class="sxs-lookup"><span data-stu-id="2ce9d-115">Policy tips display in both OWA and Outlook.</span></span> <span data-ttu-id="2ce9d-116">ومع ذلك، عند استخدام **Outlook 2013 أو أحدث،** يتم عرض تلميحات النهج فقط تحت ظروف معينة.</span><span class="sxs-lookup"><span data-stu-id="2ce9d-116">However, when using **Outlook 2013 or later**, policy tips are only displayed under certain conditions.</span></span> <span data-ttu-id="2ce9d-117">يتم سرد هذه الشروط هنا: [الشروط المعتمدة لـ Outlook 2013 أو أحدث لعرض تلميحات النهج](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips#outlook-2013-and-later-supports-showing-policy-tips-for-only-some-conditions)</span><span class="sxs-lookup"><span data-stu-id="2ce9d-117">These conditions are listed here: [Supported conditions for Outlook 2013 or later for displaying Policy Tips](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips#outlook-2013-and-later-supports-showing-policy-tips-for-only-some-conditions)</span></span>

<span data-ttu-id="2ce9d-118">للحصول على معلومات إضافية حول نصائح سياسة DLP، راجع: [إظهار نصائح السياسة لسياسات DLP](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)</span><span class="sxs-lookup"><span data-stu-id="2ce9d-118">For additional information on DLP policy tips, see: [Show policy tips for DLP Policies](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)</span></span>
  