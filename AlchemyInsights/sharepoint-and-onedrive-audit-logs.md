---
title: تقارير سجل تدقيق SharePoint الكلاسيكية
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: daf79f8d75ccdff8ad54f0f307648a5832a6bb71
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47662195"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="1be74-102">سجلات تدقيق SharePoint و OneDrive</span><span class="sxs-lookup"><span data-stu-id="1be74-102">SharePoint and OneDrive audit logs</span></span>

## <a name="sharepoint-classic-audit-logs"></a><span data-ttu-id="1be74-103">سجلات التدقيق الكلاسيكية في SharePoint</span><span class="sxs-lookup"><span data-stu-id="1be74-103">SharePoint classic Audit logs</span></span>

<span data-ttu-id="1be74-104">تم ترحيل تدقيق SPO القديم إلى سجل التدقيق الموحد (أوال).</span><span class="sxs-lookup"><span data-stu-id="1be74-104">SPO legacy auditing was migrated to Unified Audit Log (UAL).</span></span> <span data-ttu-id="1be74-105">سيتم الآن تشغيل كل تقارير التدقيق القديمة لSPO من خلال أوال ، وتم ترحيل إشارات التدقيق القديمة إلى أوال.</span><span class="sxs-lookup"><span data-stu-id="1be74-105">All SPO legacy audit reports will now be powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span>

<span data-ttu-id="1be74-106">التغييرات الاساسيه:</span><span class="sxs-lookup"><span data-stu-id="1be74-106">Key changes:</span></span>

* <span data-ttu-id="1be74-107">لا يتوفر الاقتطاع كامكانيه.</span><span class="sxs-lookup"><span data-stu-id="1be74-107">Trimming is NOT available as a capability.</span></span>
* <span data-ttu-id="1be74-108">اختيار الاحداث المحددة للتدقيق غير متوفر.</span><span class="sxs-lookup"><span data-stu-id="1be74-108">Choosing specific events to audit is NOT available.</span></span> <span data-ttu-id="1be74-109">الرجوع إلى [هذا المستند](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) للحصول علي قائمه كامله بالاحداث التدقيق المتوفرة بشكل افتراضي.</span><span class="sxs-lookup"><span data-stu-id="1be74-109">Refer to [this document](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) for a complete list of audited events available by default.</span></span>
* <span data-ttu-id="1be74-110">لا يتوفر الخيار " **الموقع** " ضمن " **تقارير مخصصه** ".</span><span class="sxs-lookup"><span data-stu-id="1be74-110">The **Location** option under **Customized reports** is NOT available.</span></span>
* <span data-ttu-id="1be74-111">لا يتوفر الخيار **فتح المستندات أو تنزيلها** .</span><span class="sxs-lookup"><span data-stu-id="1be74-111">The **Opening or downloading documents** events option is NOT available.</span></span>

[<span data-ttu-id="1be74-112">تكوين إعدادات التدقيق لمجموعه مواقع مشتركه</span><span class="sxs-lookup"><span data-stu-id="1be74-112">Configure Audit settings for a site collection</span></span>](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a><span data-ttu-id="1be74-113">سجلات التدقيق الموحد ل SharePoint و OneDrive الحديثة من التوافق</span><span class="sxs-lookup"><span data-stu-id="1be74-113">SharePoint and OneDrive Modern Unified Audit logs from compliance</span></span>

* [<span data-ttu-id="1be74-114">تشغيل ميزه تسجيل التدقيق الموحد</span><span class="sxs-lookup"><span data-stu-id="1be74-114">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="1be74-115">لا توجد اي تكوينات اضافيه مطلوبه في SharePoint أو OneDrive.</span><span class="sxs-lookup"><span data-stu-id="1be74-115">No additional configuration is required within SharePoint or OneDrive.</span></span>

<span data-ttu-id="1be74-116">استخدام ميزه البحث عن تسجيل التدقيق للتحقق من نشاط الملفات والمجلدات ، أو المستخدمين (الأسماء) ، والأذونات:</span><span class="sxs-lookup"><span data-stu-id="1be74-116">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

* [<span data-ttu-id="1be74-117">أنشطه الملفات والصفحات</span><span class="sxs-lookup"><span data-stu-id="1be74-117">File and page activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)
* [<span data-ttu-id="1be74-118">أنشطه المجلد</span><span class="sxs-lookup"><span data-stu-id="1be74-118">Folder activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [<span data-ttu-id="1be74-119">أنشطه طلب الوصول والمشاركة</span><span class="sxs-lookup"><span data-stu-id="1be74-119">Sharing and access request activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [<span data-ttu-id="1be74-120">أنشطه المزامنة</span><span class="sxs-lookup"><span data-stu-id="1be74-120">Synchronization activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [<span data-ttu-id="1be74-121">أنشطه أداره الموقع</span><span class="sxs-lookup"><span data-stu-id="1be74-121">Site administration activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

<span data-ttu-id="1be74-122">للحصول علي مزيد من المعلومات حول كيفيه استرداد هذه الاحداث ، راجع [البحث في سجل التدقيق](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span><span class="sxs-lookup"><span data-stu-id="1be74-122">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>
