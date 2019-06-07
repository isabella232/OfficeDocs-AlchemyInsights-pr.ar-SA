---
title: استعادة حذف ملف أو مجلد
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: ba1573a5-9f44-482b-8082-6f648f169449
ms.openlocfilehash: 1672f425719597b93b8ef05865797714c3b19e42
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/07/2019
ms.locfileid: "34758893"
---
# <a name="restore-a-deleted-file-or-folder"></a><span data-ttu-id="a8067-102">استعادة حذف ملف أو مجلد</span><span class="sxs-lookup"><span data-stu-id="a8067-102">Restore a deleted file or folder</span></span>

<span data-ttu-id="a8067-103">SharePoint على الإنترنت يحتفظ بنسخ احتياطية لكافة المحتويات لمدة 14 يوما إضافية بعد الحذف الفعلي.</span><span class="sxs-lookup"><span data-stu-id="a8067-103">SharePoint Online retains backups of all content for 14 additional days beyond actual deletion.</span></span> <span data-ttu-id="a8067-104">إذا لا يمكن استعادة المحتوى عن طريق سلة المحذوفات أو استعادة الملفات، مسؤول الاتصال بدعم Microsoft لطلب استعادة أي وقت داخل إطار يوم 14.</span><span class="sxs-lookup"><span data-stu-id="a8067-104">If content cannot be restored via the Recycle Bin or Files Restore, an administrator can contact Microsoft Support to request a restore any time inside the 14 day window.</span></span> <span data-ttu-id="a8067-105">يتم إكمال عمليات الاستعادة من النسخ الاحتياطية فقط لمجموعات الموقع أو المواقع الفرعية، ليس للملفات المحددة أو القوائم أو المكتبات.</span><span class="sxs-lookup"><span data-stu-id="a8067-105">Restorations from backups can only be completed for site collections or sub-sites, not for specific files, lists, or libraries.</span></span>

<span data-ttu-id="a8067-106">عند حذف عنصر أو موقع من Sharepoint، لم يكن إزالته فورا.</span><span class="sxs-lookup"><span data-stu-id="a8067-106">When you delete an item or site from Sharepoint, it isn't immediately removed.</span></span> <span data-ttu-id="a8067-107">انتقل العناصر المحذوفة في سلة المحذوفات لفترة من الوقت.</span><span class="sxs-lookup"><span data-stu-id="a8067-107">Deleted items go into the recycle bin for a period of time.</span></span> <span data-ttu-id="a8067-108">خلال هذا الوقت، يمكنك استعادة العناصر التي قمت بحذفها إلى مواقعها الأصلية.</span><span class="sxs-lookup"><span data-stu-id="a8067-108">During that time, you can restore the items you deleted to their original location.</span></span> <span data-ttu-id="a8067-109">لمزيد من المعلومات، يرجى زيارة الارتباطات أدناه.</span><span class="sxs-lookup"><span data-stu-id="a8067-109">For more information, please visit the links below.</span></span>

<span data-ttu-id="a8067-110">[استعادة العناصر الموجودة في "سلة المحذوفات" لموقع SharePoint](https://support.office.com/article/restore-deleted-items-from-the-site-collection-recycle-bin-5fa924ee-16d7-487b-9a0a-021b9062d14b?ui=en-US&amp;rs=en-US&amp;ad=US).</span><span class="sxs-lookup"><span data-stu-id="a8067-110">[Restore items in the Recycle Bin of a SharePoint site](https://support.office.com/article/restore-deleted-items-from-the-site-collection-recycle-bin-5fa924ee-16d7-487b-9a0a-021b9062d14b?ui=en-US&amp;rs=en-US&amp;ad=US).</span></span>

[<span data-ttu-id="a8067-111">استعادة حذف الملفات أو المجلدات في أندريف</span><span class="sxs-lookup"><span data-stu-id="a8067-111">Restore deleted files or folders in OneDrive</span></span>](https://support.office.com/article/Restore-deleted-files-or-folders-in-OneDrive-949ada80-0026-4db3-a953-c99083e6a84f)

[<span data-ttu-id="a8067-112">استعادة مجموعة موقع حذف (بما في ذلك فريق الاتصال ومواقع أخرى)</span><span class="sxs-lookup"><span data-stu-id="a8067-112">Restore a deleted site collection (Including group, communication and other sites)</span></span>](https://docs.microsoft.com/sharepoint/restore-deleted-site-collection)

[<span data-ttu-id="a8067-113">استعادة موقع أندريف المحذوفة</span><span class="sxs-lookup"><span data-stu-id="a8067-113">Restore a deleted OneDrive site</span></span>](https://docs.microsoft.com/onedrive/restore-deleted-onedrive)

<span data-ttu-id="a8067-114">إجراءات سلة المحذوفات جملة المسؤولين قد الأخذ في الاعتبار استخدام [Sharepoint على الإنترنت PNP](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps).</span><span class="sxs-lookup"><span data-stu-id="a8067-114">For bulk recycle bin actions, admins may consider using [Sharepoint Online PNP](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps).</span></span>

<span data-ttu-id="a8067-115">**ميزة "استعادة الملفات"**</span><span class="sxs-lookup"><span data-stu-id="a8067-115">**Files Restore feature**</span></span>

<span data-ttu-id="a8067-116">إذا كان الكثير من الملفات SharePoint أو أندريف الحصول على حذف أو استبدال، تالفة أو الإصابة بالبرامج الضارة، يمكنك استعادة مكتبة SharePoint أو أندريف بالكامل إلى استخدام ميزة "استعادة الملفات" في وقت سابق.</span><span class="sxs-lookup"><span data-stu-id="a8067-116">If lots of your OneDrive or SharePoint files get deleted, overwritten, corrupted, or infected by malware, you can restore your entire OneDrive or SharePoint library to a previous time using the files restore feature.</span></span>

[<span data-ttu-id="a8067-117">استعادة مكتبة أندريف</span><span class="sxs-lookup"><span data-stu-id="a8067-117">Restore a OneDrive library</span></span>](https://support.office.com/article/restore-your-onedrive-fa231298-759d-41cf-bcd0-25ac53eb8a15)

[<span data-ttu-id="a8067-118">استعادة مكتبة مستندات</span><span class="sxs-lookup"><span data-stu-id="a8067-118">Restore a Document library</span></span>](https://support.office.com/article/restore-a-document-library-317791c3-8bd0-4dfd-8254-3ca90883d39a?ui=en-US&amp;rs=en-US&amp;ad=US.)

