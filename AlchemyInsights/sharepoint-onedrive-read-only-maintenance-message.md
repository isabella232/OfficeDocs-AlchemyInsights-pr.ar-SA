---
title: للقراءة فقط لرسالة الصيانة عند محاولة استخدام SharePoint أو اندريف
ms.author: pebaum
author: pebaum
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
ms.openlocfilehash: 02cf1aa7abae365a3d317af9e785648d1c1517e1
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051268"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a><span data-ttu-id="948c1-102">للقراءة فقط لرسالة الصيانة عند محاولة استخدام SharePoint أو اندريف</span><span class="sxs-lookup"><span data-stu-id="948c1-102">Read-Only for Maintenance message when attempting to use SharePoint or OneDrive</span></span>

<span data-ttu-id="948c1-103">قد يتلقى المستخدمون **للقراءة فقط لرسالة الصيانة** عند محاولة استخدام SharePoint أو اندريف لأحد السيناريوهات التالية.</span><span class="sxs-lookup"><span data-stu-id="948c1-103">Users may receive a **Read-Only for Maintenance** message when attempting to use SharePoint or OneDrive for one of the following scenarios.</span></span> 

-   <span data-ttu-id="948c1-104">نشاط صيانة مخطط أو نشط.</span><span class="sxs-lookup"><span data-stu-id="948c1-104">A planned or active maintenance activity.</span></span>  <span data-ttu-id="948c1-105">تحقق منها عن طريق الانتقال إلى [مركز الرسائل](https://portal.office.com/adminportal/home#/messagecenter).</span><span class="sxs-lookup"><span data-stu-id="948c1-105">Check for them by navigating to the [Message Center](https://portal.office.com/adminportal/home#/messagecenter).</span></span>
-   <span data-ttu-id="948c1-106">حادثه خدمه نشطه ذات اولويه عاليه قد تحدث.</span><span class="sxs-lookup"><span data-stu-id="948c1-106">A high-priority, active service incident that may be occurring.</span></span> <span data-ttu-id="948c1-107">التحقق من وجود اي نصائح/الحوادث عن طريق الانتقال إلى [خدمه الصحة](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="948c1-107">Check for any advisories/incidents by navigating to [Service Health](https://portal.office.com/adminportal/home#/servicehealth).</span></span>
-   <span data-ttu-id="948c1-108">سيناريو استرداد الشفاء التلقائي البسيطة التي يمكن ان يحدث بسبب اي احداث غير متوقعه علي الملقمات التي قد تستمر لمده اقل من 30 دقيقه أو نحو ذلك.</span><span class="sxs-lookup"><span data-stu-id="948c1-108">A minor auto-healing recovery scenario that could be happening due to any unexpected events on the servers which might last for less than 30 min or so.</span></span> 
    
    <span data-ttu-id="948c1-109">لا توجد مراكز الرسائل أو الخدمات الصحية المشاركات لهذه المبالغ المستردة البسيطة ولكن يجب ان تكون العودة إلى طبيعتها قريبا جدا.</span><span class="sxs-lookup"><span data-stu-id="948c1-109">There are no Message Center or Service Health posts for these minor recoveries but you should be back to normal very soon.</span></span>

<span data-ttu-id="948c1-110">في مناسبات قليله جدا لاحظنا ان واحدا من السيناريوهات الثلاثة المذكورة أعلاه كان السبب ، وتم استعاده الخدمة ، ولكن لم يتم مسح ذاكره التخزين المؤقت للمتصفح المستخدمين.</span><span class="sxs-lookup"><span data-stu-id="948c1-110">On very few occasions we observed that one of the three scenarios listed above have been the cause, and service has been restored, but the users browser cache hasn’t been cleared up.</span></span>

<span data-ttu-id="948c1-111">الرجاء محاولة مسح ذاكره التخزين المؤقت للمتصفح قبل الانتقال إلى الموقع.</span><span class="sxs-lookup"><span data-stu-id="948c1-111">Please attempt to clear the browser cache before navigating to the site.</span></span>

1. <span data-ttu-id="948c1-112">في مستعرض Microsoft Edge ، حدد **الإعدادات**، ثم حدد **الخصوصية والأمان**.</span><span class="sxs-lookup"><span data-stu-id="948c1-112">In your Microsoft Edge browser, select **Settings**, and then select **Privacy and Security**.</span></span>
2. <span data-ttu-id="948c1-113">ضمن **استعراض واضح**، حدد **اختيار ما تريد إلغاء**تحديده.</span><span class="sxs-lookup"><span data-stu-id="948c1-113">Under **Clear browsing**, select **Choose what to clear**.</span></span>
3. <span data-ttu-id="948c1-114">حدد **ملفات تعريف الارتباط وبيانات موقع الويب المحفوظة**، ثم اختر **مسح**.</span><span class="sxs-lookup"><span data-stu-id="948c1-114">Select **Cookies and saved website data**, and select **Clear**.</span></span>

>[!Note] 
> <span data-ttu-id="948c1-115">قد تختلف هذه الخطوات عند استخدام متصفحات أخرى مثل موزيلا فايرفوكس أو جوجل كروم.</span><span class="sxs-lookup"><span data-stu-id="948c1-115">These steps may differ when using other browsers such as Mozilla Firefox or Google Chrome.</span></span>

>[!Note] 
> <span data-ttu-id="948c1-116">سيكون خيار آخر لفتح موقع SharePoint أو اندريف في اطار InPrivate جديد.</span><span class="sxs-lookup"><span data-stu-id="948c1-116">Another option would be to open your SharePoint site or OneDrive in a new InPrivate window.</span></span>