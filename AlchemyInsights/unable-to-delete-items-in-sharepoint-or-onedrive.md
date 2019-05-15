---
title: غير قادر على حذف عناصر SharePoint أو أونيدريفي
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 21d7b928fade48a6729c120e6ea33b16dafe799e
ms.sourcegitcommit: 22ce2315c8cf643137ab3420cdc1cda41433d44a
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/14/2019
ms.locfileid: "34057664"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="aac94-102">غير قادر على حذف العناصر</span><span class="sxs-lookup"><span data-stu-id="aac94-102">Unable to delete items</span></span>

<span data-ttu-id="aac94-103">تواجه مشكلات حذف العناصر؟</span><span class="sxs-lookup"><span data-stu-id="aac94-103">Having issues deleting items?</span></span>

- <span data-ttu-id="aac94-104">تأكد دائماً لديك [الأذونات المناسبة](https://docs.microsoft.com/en-us/sharepoint/default-sharepoint-groups) لحذف العنصر أو محاولة [مسؤول مجموعة الموقع](https://docs.microsoft.com/en-us/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) إزالة العنصر.</span><span class="sxs-lookup"><span data-stu-id="aac94-104">Always make sure you have the [appropriate permissions](https://docs.microsoft.com/en-us/sharepoint/default-sharepoint-groups) to delete the item or have a [site collection administrator](https://docs.microsoft.com/en-us/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) attempt remove the item.</span></span>

- <span data-ttu-id="aac94-105">تأكد من أنه لا يوجد إعداد [نهج الاستبقاء](https://docs.microsoft.com/en-us/office365/securitycompliance/retention-policies) على العنصر.</span><span class="sxs-lookup"><span data-stu-id="aac94-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/en-us/office365/securitycompliance/retention-policies) setup on the item.</span></span>

- <span data-ttu-id="aac94-106">تأكد من أن العنصر ليس [قيد السحب](https://support.office.com/en-us/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) إلى مستخدم آخر.</span><span class="sxs-lookup"><span data-stu-id="aac94-106">Ensure the item is not [checked out](https://support.office.com/en-us/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

- <span data-ttu-id="aac94-107">وأخيراً، يمكن للمسؤولين استخدام [أنماط SharePoint والممارسات](https://docs.microsoft.com/en-us/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) الذي يحتوي على مكتبة PowerShell الأوامر التي تسمح لك بتنفيذ إجراءات إدارة معقدة مثل فرض حذف العناصر العنيدة.</span><span class="sxs-lookup"><span data-stu-id="aac94-107">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/en-us/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span> 
- [<span data-ttu-id="aac94-108">إزالة ملف PNP</span><span class="sxs-lookup"><span data-stu-id="aac94-108">Remove PNP File</span></span>](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="aac94-109">إزالة المجلد PNP</span><span class="sxs-lookup"><span data-stu-id="aac94-109">Remove PNP Folder</span></span>](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="aac94-110">إزالة عنصر قائمة PNP</span><span class="sxs-lookup"><span data-stu-id="aac94-110">Remove PNP List Item</span></span>](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="aac94-111">إزالة قائمة PNP</span><span class="sxs-lookup"><span data-stu-id="aac94-111">Remove PNP List</span></span>](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="aac94-112">إزالة PNP حقل (عمود)</span><span class="sxs-lookup"><span data-stu-id="aac94-112">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)