---
title: استعادة ملف أو مجلد محذوف
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: ba1573a5-9f44-482b-8082-6f648f169449
ms.openlocfilehash: 8c7ce48f50b5c933ea15c23a486b99ad7a7f4d79
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707509"
---
# <a name="restore-a-deleted-file-or-folder"></a><span data-ttu-id="7a2d0-102">استعادة ملف أو مجلد محذوف</span><span class="sxs-lookup"><span data-stu-id="7a2d0-102">Restore a deleted file or folder</span></span>

<span data-ttu-id="7a2d0-103">يحافظ SharePoint Online علي النسخ الاحتياطية لكل المحتويات لمدة 14 يومًا إضافية بعد الحذف الفعلي.</span><span class="sxs-lookup"><span data-stu-id="7a2d0-103">SharePoint Online retains backups of all content for 14 additional days beyond actual deletion.</span></span> <span data-ttu-id="7a2d0-104">إذا لم يكن من الممكن استعادة المحتوى عبر "سلة المهملات" أو "استعادة الملفات"، يمكن للمسؤول الاتصال بدعم Microsoft لطلب استعادة في أي وقت داخل نافذة ال 14 يوما.</span><span class="sxs-lookup"><span data-stu-id="7a2d0-104">If content cannot be restored via the Recycle Bin or Files Restore, an administrator can contact Microsoft Support to request a restore any time inside the 14 day window.</span></span> <span data-ttu-id="7a2d0-105">لا يمكن استكمال عمليات الاستعادة من النسخ الاحتياطية إلا لمجموعات المواقع أو المواقع الفرعية، وليس لملفات أو قوائم أو مكتبات محددة.</span><span class="sxs-lookup"><span data-stu-id="7a2d0-105">Restorations from backups can only be completed for site collections or sub-sites, not for specific files, lists, or libraries.</span></span>

<span data-ttu-id="7a2d0-106">عند حذف عنصر أو موقع من Sharepoint، لن تتم إزالته على الفور.</span><span class="sxs-lookup"><span data-stu-id="7a2d0-106">When you delete an item or site from Sharepoint, it isn't immediately removed.</span></span> <span data-ttu-id="7a2d0-107">تنتقل العناصر المحذوفة إلى "سله المحذوفات" لفترة زمنية.</span><span class="sxs-lookup"><span data-stu-id="7a2d0-107">Deleted items go into the recycle bin for a period of time.</span></span> <span data-ttu-id="7a2d0-108">خلال ذلك الوقت، يمكنك استعادة العناصر التي حذفتها إلى موقعها الأصلي.</span><span class="sxs-lookup"><span data-stu-id="7a2d0-108">During that time, you can restore the items you deleted to their original location.</span></span> <span data-ttu-id="7a2d0-109">للحصول على مزيد من المعلومات، الرجاء زيارة الارتباطات الموجودة أدناه.</span><span class="sxs-lookup"><span data-stu-id="7a2d0-109">For more information, please visit the links below.</span></span>

<span data-ttu-id="7a2d0-110">[استعادة العناصر في سلة مواعيد موقع SharePoint.](https://support.microsoft.com/office/restore-items-in-the-recycle-bin-that-were-deleted-from-sharepoint-or-teams-6df466b6-55f2-4898-8d6e-c0dff851a0be)</span><span class="sxs-lookup"><span data-stu-id="7a2d0-110">[Restore items in the Recycle Bin of a SharePoint site](https://support.microsoft.com/office/restore-items-in-the-recycle-bin-that-were-deleted-from-sharepoint-or-teams-6df466b6-55f2-4898-8d6e-c0dff851a0be).</span></span>

[<span data-ttu-id="7a2d0-111">استعادة الملفات أو المجلدات المحذوفة في OneDrive</span><span class="sxs-lookup"><span data-stu-id="7a2d0-111">Restore deleted files or folders in OneDrive</span></span>](https://support.office.com/article/Restore-deleted-files-or-folders-in-OneDrive-949ada80-0026-4db3-a953-c99083e6a84f)

[<span data-ttu-id="7a2d0-112">استعادة مجموعة مواقع ويب محذوفة (بما في ذلك المجموعة والاتصال والمواقع الأخرى)</span><span class="sxs-lookup"><span data-stu-id="7a2d0-112">Restore a deleted site collection (Including group, communication and other sites)</span></span>](https://docs.microsoft.com/sharepoint/restore-deleted-site-collection)

[<span data-ttu-id="7a2d0-113">استعادة موقع OneDrive محذوف</span><span class="sxs-lookup"><span data-stu-id="7a2d0-113">Restore a deleted OneDrive site</span></span>](https://docs.microsoft.com/onedrive/restore-deleted-onedrive)

<span data-ttu-id="7a2d0-114">بالنسبة إلى إجراءات سلة المهملات المجمعة، قد تفكر المسؤولين في استخدام [Sharepoint Online PNP.](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps)</span><span class="sxs-lookup"><span data-stu-id="7a2d0-114">For bulk recycle bin actions, admins may consider using [Sharepoint Online PNP](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps).</span></span>

<span data-ttu-id="7a2d0-115">**ميزة استعادة الملفات**</span><span class="sxs-lookup"><span data-stu-id="7a2d0-115">**Files Restore feature**</span></span>

<span data-ttu-id="7a2d0-116">إذا تم حذف الكثير من ملفات OneDrive أو SharePoint أو الكتابة فوقها أو إصابتها بالتلف أو أصيبت بالبرامج الضارة، يمكنك استعادة مكتبة OneDrive أو SharePoint بالكامل إلى وقت سابق باستخدام ميزة استعادة الملفات.</span><span class="sxs-lookup"><span data-stu-id="7a2d0-116">If lots of your OneDrive or SharePoint files get deleted, overwritten, corrupted, or infected by malware, you can restore your entire OneDrive or SharePoint library to a previous time using the files restore feature.</span></span>

[<span data-ttu-id="7a2d0-117">استعادة مكتبة OneDrive</span><span class="sxs-lookup"><span data-stu-id="7a2d0-117">Restore a OneDrive library</span></span>](https://support.office.com/article/restore-your-onedrive-fa231298-759d-41cf-bcd0-25ac53eb8a15)

[<span data-ttu-id="7a2d0-118">استعادة مكتبة مستندات</span><span class="sxs-lookup"><span data-stu-id="7a2d0-118">Restore a Document library</span></span>](https://support.office.com/article/restore-a-document-library-317791c3-8bd0-4dfd-8254-3ca90883d39a)

