---
title: استعاده ملف أو مجلد محذوف
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
ms.openlocfilehash: fc560686ec5c6a3d42a97687fda80ae5001b5c60
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47797535"
---
# <a name="restore-a-deleted-file-or-folder"></a><span data-ttu-id="f801d-102">استعاده ملف أو مجلد محذوف</span><span class="sxs-lookup"><span data-stu-id="f801d-102">Restore a deleted file or folder</span></span>

<span data-ttu-id="f801d-103">يحافظ SharePoint Online علي النسخ الاحتياطية لكل المحتويات لمدة 14 يومًا إضافية بعد الحذف الفعلي.</span><span class="sxs-lookup"><span data-stu-id="f801d-103">SharePoint Online retains backups of all content for 14 additional days beyond actual deletion.</span></span> <span data-ttu-id="f801d-104">إذا تعذرت استعاده المحتوي عبر "سله المحذوفات" أو "استعاده الملفات" ، فبامكان المسؤول الاتصال بدعم Microsoft لطلب استعاده اي وقت داخل نافذه 14 يوما.</span><span class="sxs-lookup"><span data-stu-id="f801d-104">If content cannot be restored via the Recycle Bin or Files Restore, an administrator can contact Microsoft Support to request a restore any time inside the 14 day window.</span></span> <span data-ttu-id="f801d-105">لا يمكن استكمال عمليات الاستعادة من النسخ الاحتياطية إلا لمجموعات المواقع أو المواقع الفرعية، وليس لملفات أو قوائم أو مكتبات محددة.</span><span class="sxs-lookup"><span data-stu-id="f801d-105">Restorations from backups can only be completed for site collections or sub-sites, not for specific files, lists, or libraries.</span></span>

<span data-ttu-id="f801d-106">عندما تحذف عنصرا أو موقعا من Sharepoint ، فلن تتم ازالته علي الفور.</span><span class="sxs-lookup"><span data-stu-id="f801d-106">When you delete an item or site from Sharepoint, it isn't immediately removed.</span></span> <span data-ttu-id="f801d-107">تنتقل العناصر المحذوفة إلى "سله المحذوفات" لفترة زمنية.</span><span class="sxs-lookup"><span data-stu-id="f801d-107">Deleted items go into the recycle bin for a period of time.</span></span> <span data-ttu-id="f801d-108">خلال ذلك الوقت، يمكنك استعادة العناصر التي حذفتها إلى موقعها الأصلي.</span><span class="sxs-lookup"><span data-stu-id="f801d-108">During that time, you can restore the items you deleted to their original location.</span></span> <span data-ttu-id="f801d-109">للحصول على مزيد من المعلومات، الرجاء زيارة الارتباطات الموجودة أدناه.</span><span class="sxs-lookup"><span data-stu-id="f801d-109">For more information, please visit the links below.</span></span>

<span data-ttu-id="f801d-110">[استعاده العناصر الموجودة في سله المحذوفات لموقع SharePoint](https://support.office.com/article/restore-deleted-items-from-the-site-collection-recycle-bin-5fa924ee-16d7-487b-9a0a-021b9062d14b).</span><span class="sxs-lookup"><span data-stu-id="f801d-110">[Restore items in the Recycle Bin of a SharePoint site](https://support.office.com/article/restore-deleted-items-from-the-site-collection-recycle-bin-5fa924ee-16d7-487b-9a0a-021b9062d14b).</span></span>

[<span data-ttu-id="f801d-111">استعاده الملفات أو المجلدات المحذوفة في OneDrive</span><span class="sxs-lookup"><span data-stu-id="f801d-111">Restore deleted files or folders in OneDrive</span></span>](https://support.office.com/article/Restore-deleted-files-or-folders-in-OneDrive-949ada80-0026-4db3-a953-c99083e6a84f)

[<span data-ttu-id="f801d-112">استعاده مجموعه مواقع مشتركه محذوفة (بما في ذلك المجموعة والاتصال والمواقع الأخرى)</span><span class="sxs-lookup"><span data-stu-id="f801d-112">Restore a deleted site collection (Including group, communication and other sites)</span></span>](https://docs.microsoft.com/sharepoint/restore-deleted-site-collection)

[<span data-ttu-id="f801d-113">استعاده موقع OneDrive محذوف</span><span class="sxs-lookup"><span data-stu-id="f801d-113">Restore a deleted OneDrive site</span></span>](https://docs.microsoft.com/onedrive/restore-deleted-onedrive)

<span data-ttu-id="f801d-114">بالنسبة إلى إجراءات سله المحذوفات المجمعة ، يمكن للمسؤولين استخدام [Sharepoint ONLINE PNP](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps).</span><span class="sxs-lookup"><span data-stu-id="f801d-114">For bulk recycle bin actions, admins may consider using [Sharepoint Online PNP](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps).</span></span>

<span data-ttu-id="f801d-115">**ميزة استعادة الملفات**</span><span class="sxs-lookup"><span data-stu-id="f801d-115">**Files Restore feature**</span></span>

<span data-ttu-id="f801d-116">إذا كانت هناك الكثير من ملفات OneDrive أو SharePoint التي قمت بحذفها ، أو الكتابة فوقها ، أو تلفها ، أو المصابة بالبرامج الضارة ، فيمكنك استعاده OneDrive أو مكتبه SharePoint بالبالكامل إلى وقت سابق باستخدام ميزه استعاده الملفات.</span><span class="sxs-lookup"><span data-stu-id="f801d-116">If lots of your OneDrive or SharePoint files get deleted, overwritten, corrupted, or infected by malware, you can restore your entire OneDrive or SharePoint library to a previous time using the files restore feature.</span></span>

[<span data-ttu-id="f801d-117">استعادة مكتبة OneDrive</span><span class="sxs-lookup"><span data-stu-id="f801d-117">Restore a OneDrive library</span></span>](https://support.office.com/article/restore-your-onedrive-fa231298-759d-41cf-bcd0-25ac53eb8a15)

[<span data-ttu-id="f801d-118">استعادة مكتبة مستندات</span><span class="sxs-lookup"><span data-stu-id="f801d-118">Restore a Document library</span></span>](https://support.office.com/article/restore-a-document-library-317791c3-8bd0-4dfd-8254-3ca90883d39a)

