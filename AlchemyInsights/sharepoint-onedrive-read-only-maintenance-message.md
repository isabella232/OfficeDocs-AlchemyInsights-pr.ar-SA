---
title: للقراءة فقط لرسالة الصيانة عند محاولة استخدام SharePoint أو OneDrive
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: a3d313816beefcefa4d93528d3ad9a684e60390e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670819"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a><span data-ttu-id="e82eb-102">للقراءة فقط لرسالة الصيانة عند محاولة استخدام SharePoint أو OneDrive</span><span class="sxs-lookup"><span data-stu-id="e82eb-102">Read-Only for Maintenance message when attempting to use SharePoint or OneDrive</span></span>

<span data-ttu-id="e82eb-103">قد يتلقى **المستخدمون للقراءة فقط لرسالة الصيانة** عند محاولة استخدام SharePoint أو OneDrive لأحدي السيناريوهات التالية.</span><span class="sxs-lookup"><span data-stu-id="e82eb-103">Users may receive a **Read-Only for Maintenance** message when attempting to use SharePoint or OneDrive for one of the following scenarios.</span></span> 

-   <span data-ttu-id="e82eb-104">نشاط صيانة مخطط أو نشط.</span><span class="sxs-lookup"><span data-stu-id="e82eb-104">A planned or active maintenance activity.</span></span>  <span data-ttu-id="e82eb-105">ابحث عنها عن طريق الانتقال إلى [مركز الرسائل](https://portal.office.com/adminportal/home#/messagecenter).</span><span class="sxs-lookup"><span data-stu-id="e82eb-105">Check for them by navigating to the [Message Center](https://portal.office.com/adminportal/home#/messagecenter).</span></span>
-   <span data-ttu-id="e82eb-106">حدث الخدمة ذات الاولويه العالية والفعالة التي قد تحدث.</span><span class="sxs-lookup"><span data-stu-id="e82eb-106">A high-priority, active service incident that may be occurring.</span></span> <span data-ttu-id="e82eb-107">ابحث عن اي نصائح/حوادث عن طريق الانتقال إلى [حماية الخدمة](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="e82eb-107">Check for any advisories/incidents by navigating to [Service Health](https://portal.office.com/adminportal/home#/servicehealth).</span></span>
-   <span data-ttu-id="e82eb-108">سيناريو الإصلاح التلقائي الثانوي الذي يمكن ان يحدث بسبب اي احداث غير متوقعه علي الخوادم التي قد تقل عن 30 دقيقه أو بالتالي.</span><span class="sxs-lookup"><span data-stu-id="e82eb-108">A minor auto-healing recovery scenario that could be happening due to any unexpected events on the servers which might last for less than 30 min or so.</span></span> 
    
    <span data-ttu-id="e82eb-109">لا توجد اي عمليات نشر لمركز الرسائل أو الخدمة لهذه الريكوفيريس الثانوية ولكن يجب ان تعود إلى الحالة العادية قريبا.</span><span class="sxs-lookup"><span data-stu-id="e82eb-109">There are no Message Center or Service Health posts for these minor recoveries but you should be back to normal very soon.</span></span>

<span data-ttu-id="e82eb-110">في حالات قليله جدا ، لقد قمنا بملاحظه ان أحدي السيناريوهات الثلاثة المدرجة أعلاه قد حدثت ، وتمت استعاده الخدمة ، ولكن لم يتم مسح ذاكره التخزين المؤقت لمستعرض المستخدمين.</span><span class="sxs-lookup"><span data-stu-id="e82eb-110">On very few occasions we observed that one of the three scenarios listed above have been the cause, and service has been restored, but the users browser cache hasn’t been cleared up.</span></span>

<span data-ttu-id="e82eb-111">يرجى محاولة مسح ذاكره التخزين المؤقت للمستعرض قبل التنقل إلى الموقع.</span><span class="sxs-lookup"><span data-stu-id="e82eb-111">Please attempt to clear the browser cache before navigating to the site.</span></span>

1. <span data-ttu-id="e82eb-112">في مستعرض Microsoft Edge ، حدد **إعدادات**، ثم حدد **الخصوصية والأمان**.</span><span class="sxs-lookup"><span data-stu-id="e82eb-112">In your Microsoft Edge browser, select **Settings**, and then select **Privacy and Security**.</span></span>
2. <span data-ttu-id="e82eb-113">ضمن **مسح الاستعراض**، حدد **اختيار ما تريد مسحه**.</span><span class="sxs-lookup"><span data-stu-id="e82eb-113">Under **Clear browsing**, select **Choose what to clear**.</span></span>
3. <span data-ttu-id="e82eb-114">حدد **ملفات تعريف الارتباط وبيانات موقع ويب محفوظه**، وحدد **مسح**.</span><span class="sxs-lookup"><span data-stu-id="e82eb-114">Select **Cookies and saved website data**, and select **Clear**.</span></span>

>[!Note] 
> <span data-ttu-id="e82eb-115">قد تختلف هذه الخطوات عند استخدام مستعرضات أخرى مثل Mozilla Firefox أو Google Chrome.</span><span class="sxs-lookup"><span data-stu-id="e82eb-115">These steps may differ when using other browsers such as Mozilla Firefox or Google Chrome.</span></span>

>[!Note] 
> <span data-ttu-id="e82eb-116">هناك خيار آخر لفتح موقع SharePoint أو OneDrive في نافذه InPrivate جديده.</span><span class="sxs-lookup"><span data-stu-id="e82eb-116">Another option would be to open your SharePoint site or OneDrive in a new InPrivate window.</span></span>