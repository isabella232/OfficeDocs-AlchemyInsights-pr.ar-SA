---
title: SharePoint اختناق عبر الإنترنت
ms.author: pebaum
author: pebaum
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.custom:
- "9000149"
- "1662"
- "3491"
ms.openlocfilehash: 59104ef96c95de4e4bc7744825245bdafba97d7c
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931213"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="b251a-102">SharePoint اختناق عبر الإنترنت</span><span class="sxs-lookup"><span data-stu-id="b251a-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="b251a-103">**هام:** يعمل العديد من عملاء SharePoint Online و OneDrive على تشغيل تطبيقات مهمة للأعمال مقابل الخدمة التي تعمل في الخلفية.</span><span class="sxs-lookup"><span data-stu-id="b251a-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="b251a-104">وتشمل هذه ترحيل المحتوى، منع فقدان البيانات (DLP)، وحلول النسخ الاحتياطي.</span><span class="sxs-lookup"><span data-stu-id="b251a-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="b251a-105">خلال هذه الأوقات غير المسبوقة، نتخذ خطوات لضمان أن تظل خدمات SharePoint Online و OneDrive متاحة للغاية وموثوقة للمستخدمين الذين يعتمدون على الخدمة أكثر من أي وقت مضى في سيناريوهات العمل عن بعد.</span><span class="sxs-lookup"><span data-stu-id="b251a-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="b251a-106">ولدعم هذا الهدف، قمنا بتنفيذ قيود خنق أكثر صرامة على تطبيقات الخلفية (الترحيل وDLP وحلول النسخ الاحتياطي) خلال ساعات النهار في أيام الأسبوع.</span><span class="sxs-lookup"><span data-stu-id="b251a-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="b251a-107">يجب أن تتوقع أن تحقق هذه التطبيقات إنتاجية محدودة جدًا خلال هذه الأوقات.</span><span class="sxs-lookup"><span data-stu-id="b251a-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="b251a-108">ومع ذلك ، خلال ساعات المساء وعطلة نهاية الأسبوع للمنطقة ، ستكون الخدمة جاهزة لمعالجة حجم أكبر بكثير من الطلبات من تطبيقات الخلفية.</span><span class="sxs-lookup"><span data-stu-id="b251a-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="b251a-109">**503 خادم خطأ مشغول**</span><span class="sxs-lookup"><span data-stu-id="b251a-109">**503 server is busy error**</span></span>

<span data-ttu-id="b251a-110">قد يتلقى المستخدمون ملقم 503 خطأ مشغول عند محاولة الانتقال إلى مواقع SharePoint أو OneDrive.</span><span class="sxs-lookup"><span data-stu-id="b251a-110">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="b251a-111">يمكن أن يكون سبب هذا الخطأ اختناق داخل خدمة SharePoint.</span><span class="sxs-lookup"><span data-stu-id="b251a-111">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="b251a-112">يستخدم SharePoint Online الاختناق للحفاظ على الأداء الأمثل وموثوقية خدمة SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="b251a-112">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="b251a-113">الاختناق يحد من عدد إجراءات المستخدم أو المكالمات المتزامنة (بواسطة البرنامج النصي أو التعليمات البرمجية) لمنع الإفراط في استخدام الموارد.</span><span class="sxs-lookup"><span data-stu-id="b251a-113">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> 

<span data-ttu-id="b251a-114">لمزيد من المعلومات حول الاختناق انظر، [تجنب الحصول على خنق أو حظر في SharePoint عبر الإنترنت](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="b251a-114">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="b251a-115">إذا كنت تعتقد أن هذا الخطأ لا علاقة له بالاختناق، يمكنك التحقق مما إذا كانت هناك صيانة نشطة تحدث على المستأجر الخاص بك عن طريق التنقل إلى [مركز الرسائل](https://portal.office.com/adminportal/home#/MessageCenter).</span><span class="sxs-lookup"><span data-stu-id="b251a-115">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="b251a-116">أخيرًا، تأكد من زيارة صفحة ["صحة الخدمة"](https://portal.office.com/adminportal/home#/servicehealth) للتحقق من أي تحذيرات/حوادث قد تحدث.</span><span class="sxs-lookup"><span data-stu-id="b251a-116">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

