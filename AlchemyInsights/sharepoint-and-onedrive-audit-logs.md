---
title: تقارير سجل تدقيق SharePoint الكلاسيكية
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: af5b3c76b82db13bc89c917247e41fa1d8779b68
ms.sourcegitcommit: d5bf97a0bf0547f36b6da9684ce9f16a13a7749e
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/20/2019
ms.locfileid: "37068010"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="d0c32-102">سجلات تدقيق SharePoint وOneDrive</span><span class="sxs-lookup"><span data-stu-id="d0c32-102">SharePoint and OneDrive audit logs</span></span>

<span data-ttu-id="d0c32-103">**سجلات التدقيق الموحدة الحديثة SharePoint وOneDrive من التوافق**</span><span class="sxs-lookup"><span data-stu-id="d0c32-103">**SharePoint and OneDrive Modern Unified Audit logs from compliance**</span></span>

- [<span data-ttu-id="d0c32-104">تشغيل/إيقاف تشغيل تسجيل التدقيق الموحد</span><span class="sxs-lookup"><span data-stu-id="d0c32-104">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="d0c32-105">لا يوجد تكوين إضافي مطلوب داخل SharePoint أو أندريف.</span><span class="sxs-lookup"><span data-stu-id="d0c32-105">No additional configuration is required within SharePoint or OneDrive.</span></span>

- <span data-ttu-id="d0c32-106">استخدم البحث عن تسجيل التدقيق للتحقق من نشاط الملف (الملفات) والمجلد (المجلدات) والمستخدمين والأذونات:</span><span class="sxs-lookup"><span data-stu-id="d0c32-106">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

    - [<span data-ttu-id="d0c32-107">أنشطة الملفات والصفحات</span><span class="sxs-lookup"><span data-stu-id="d0c32-107">File and page activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
    - [<span data-ttu-id="d0c32-108">أنشطة المجلد</span><span class="sxs-lookup"><span data-stu-id="d0c32-108">Folder activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
    - [<span data-ttu-id="d0c32-109">أنشطة طلب المشاركة والوصول</span><span class="sxs-lookup"><span data-stu-id="d0c32-109">Sharing and access request activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
    - [<span data-ttu-id="d0c32-110">أنشطة التزامن</span><span class="sxs-lookup"><span data-stu-id="d0c32-110">Synchronization activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
    - [<span data-ttu-id="d0c32-111">أنشطة إدارة الموقع</span><span class="sxs-lookup"><span data-stu-id="d0c32-111">Site administration activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)
- <span data-ttu-id="d0c32-112">لمزيد من المعلومات حول كيفية استرداد هذه الأحداث، راجع [البحث في سجل التدقيق](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span><span class="sxs-lookup"><span data-stu-id="d0c32-112">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>

<span data-ttu-id="d0c32-113">**سجلات التدقيق الكلاسيكية SharePoint**</span><span class="sxs-lookup"><span data-stu-id="d0c32-113">**SharePoint classic Audit logs**</span></span>

<span data-ttu-id="d0c32-114">لقد قمنا بترحيل التدقيق القديم لـ SPO إلى سجل التدقيق الموحد (UAL).</span><span class="sxs-lookup"><span data-stu-id="d0c32-114">We migrated SPO legacy auditing to Unified Audit Log (UAL).</span></span> <span data-ttu-id="d0c32-115">وهذا يعني أساسا أن جميع تقارير التدقيق القديمة SPO سيتم الآن تشغيلها من خلال UAL، وقد تم ترحيل إشارات التدقيق القديمة إلى UAL.</span><span class="sxs-lookup"><span data-stu-id="d0c32-115">This essentially means that all SPO legacy audit reports will now be powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span>

<span data-ttu-id="d0c32-116">التغييرات الرئيسية:</span><span class="sxs-lookup"><span data-stu-id="d0c32-116">Key changes:</span></span>

- <span data-ttu-id="d0c32-117">التشذيب كقدرة غير متوفرة.</span><span class="sxs-lookup"><span data-stu-id="d0c32-117">Trimming as a capability is NOT available.</span></span>
- <span data-ttu-id="d0c32-118">لا يتوفر القسم الذي تختار فيه أحداث معينة للتدقيق.</span><span class="sxs-lookup"><span data-stu-id="d0c32-118">The section where you choose specific events to audit is NOT available.</span></span> <span data-ttu-id="d0c32-119">الرجاء الرجوع إلى [هذا المستند](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) للحصول على قائمة كاملة بالأحداث المدققة المتوفرة بشكل افتراضي.</span><span class="sxs-lookup"><span data-stu-id="d0c32-119">Please refer to [this document](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) for a complete list of audited events available by default.</span></span>
- <span data-ttu-id="d0c32-120">الخيار "الموقع" ضمن **التقارير المخصصة** غير متوفر.</span><span class="sxs-lookup"><span data-stu-id="d0c32-120">The "Location" option under **Customized reports** is NOT available.</span></span> 
- <span data-ttu-id="d0c32-121">أحداث "فتح المستندات أو تنزيلها" غير متوفرة.</span><span class="sxs-lookup"><span data-stu-id="d0c32-121">“Opening or downloading documents” events is NOT available.</span></span> 

