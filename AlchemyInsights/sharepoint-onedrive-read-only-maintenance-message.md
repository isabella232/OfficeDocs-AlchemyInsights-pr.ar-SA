---
title: القراءة فقط لصيانة رسالة عند محاولة استخدام SharePoint أو أندريف
ms.author: efrene
author: efrene
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: 5b1e56253d6deeb0f9ba2f753eff5c00ff9c51a2
ms.sourcegitcommit: cd79ecca88b2cb166f78f44ab8bc4e8136729418
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/23/2019
ms.locfileid: "36620710"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a><span data-ttu-id="17645-102">القراءة فقط لصيانة رسالة عند محاولة استخدام SharePoint أو أندريف</span><span class="sxs-lookup"><span data-stu-id="17645-102">Read-Only for Maintenance message when attempting to use SharePoint or OneDrive</span></span>

<span data-ttu-id="17645-103">ظهور رسالة **القراءة فقط للحفاظ على** المستخدمين عند محاولة استخدام SharePoint أو أندريف لأحد السيناريوهات التالية.</span><span class="sxs-lookup"><span data-stu-id="17645-103">Users may receive a **Read-Only for Maintenance** message when attempting to use SharePoint or OneDrive for one of the following scenarios.</span></span> 

-   <span data-ttu-id="17645-104">بنشاط صيانة المخططة أو غير نشط.</span><span class="sxs-lookup"><span data-stu-id="17645-104">A planned or active maintenance activity.</span></span>  <span data-ttu-id="17645-105">البحث عنها عن طريق الانتقال إلى [مركز الرسائل](https://portal.office.com/adminportal/home#/messagecenter).</span><span class="sxs-lookup"><span data-stu-id="17645-105">Check for them by navigating to the [Message Center](https://portal.office.com/adminportal/home#/messagecenter).</span></span>
-   <span data-ttu-id="17645-106">حادث خدمة النشطة ذات أولوية عالية، التي قد تحدث.</span><span class="sxs-lookup"><span data-stu-id="17645-106">A high-priority, active service incident that may be occurring.</span></span> <span data-ttu-id="17645-107">التحقق من وجود أية نصائح/الحوادث المتعلقة بالتنقل إلى [الخدمات الصحية](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="17645-107">Check for any advisories/incidents by navigating to [Service Health](https://portal.office.com/adminportal/home#/servicehealth).</span></span>
-   <span data-ttu-id="17645-108">ثانوية الإصلاح تلقائي استرداد سيناريو الذي قد يحدث نتيجة لأي أحداث غير متوقعة على الخوادم التي قد تستمر لمدة تقل عن 30 دقيقة أو نحو ذلك.</span><span class="sxs-lookup"><span data-stu-id="17645-108">A minor auto-healing recovery scenario that could be happening due to any unexpected events on the servers which might last for less than 30 min or so.</span></span> 
    
    <span data-ttu-id="17645-109">هناك لا مركز أو وظائف "الحماية خدمة" لهذه المبالغ المستردة الثانوية لكن يجب أن تكون العودة إلى طبيعتها قريبا جداً.</span><span class="sxs-lookup"><span data-stu-id="17645-109">There are no Message Center or Service Health posts for these minor recoveries but you should be back to normal very soon.</span></span>

<span data-ttu-id="17645-110">وفي حالات قليلة جداً أننا لاحظنا أن أحد السيناريوهات الثلاثة المذكورة أعلاه هي سبب، وتمت استعادة الخدمة، ولكن لم يتم مسح التخزين المؤقت للمستعرض المستخدمين.</span><span class="sxs-lookup"><span data-stu-id="17645-110">On very few occasions we observed that one of the three scenarios listed above have been the cause, and service has been restored, but the users browser cache hasn’t been cleared up.</span></span>

<span data-ttu-id="17645-111">الرجاء محاولة مسح التخزين المؤقت للمستعرض قبل الانتقال إلى الموقع.</span><span class="sxs-lookup"><span data-stu-id="17645-111">Please attempt to clear the browser cache before navigating to the site.</span></span>

1. <span data-ttu-id="17645-112">في مستعرض حافة Microsoft، حدد **إعدادات**، وحدد **الخصوصية والأمان**.</span><span class="sxs-lookup"><span data-stu-id="17645-112">In your Microsoft Edge browser, select **Settings**, and then select **Privacy and Security**.</span></span>
2. <span data-ttu-id="17645-113">ضمن **الاستعراض واضحة**، حدد **اختر ما تريد مسح**.</span><span class="sxs-lookup"><span data-stu-id="17645-113">Under **Clear browsing**, select **Choose what to clear**.</span></span>
3. <span data-ttu-id="17645-114">حدد **ملفات تعريف الارتباط وبيانات موقع ويب المحفوظة**، وحدد **مسح**.</span><span class="sxs-lookup"><span data-stu-id="17645-114">Select **Cookies and saved website data**, and select **Clear**.</span></span>

>[!Note] 
> <span data-ttu-id="17645-115">قد تختلف الخطوات التالية عند استخدام المستعرضات الأخرى مثل موزيلا فايرفوكس أو جوجل كروم.</span><span class="sxs-lookup"><span data-stu-id="17645-115">These steps may differ when using other browsers such as Mozilla Firefox or Google Chrome.</span></span>

>[!Note] 
> <span data-ttu-id="17645-116">خيار آخر يتمثل في فتح موقع SharePoint الخاص بك أو أندريف في نافذة جديدة InPrivate.</span><span class="sxs-lookup"><span data-stu-id="17645-116">Another option would be to open your SharePoint site or OneDrive in a new InPrivate window.</span></span>