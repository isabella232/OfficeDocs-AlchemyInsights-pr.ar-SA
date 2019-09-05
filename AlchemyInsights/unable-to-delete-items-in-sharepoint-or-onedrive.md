---
title: غير قادر على حذف العناصر في SharePoint أو أندريف
ms.author: pebaum
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: 3cc168846999c6880b95edfaedb2df8cf6e843a6
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/04/2019
ms.locfileid: "36748511"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="a5f97-102">غير قادر على حذف العناصر</span><span class="sxs-lookup"><span data-stu-id="a5f97-102">Unable to delete items</span></span>

<span data-ttu-id="a5f97-103">هل تحتاج إلى مشاكل في حذف عناصر SharePoint؟</span><span class="sxs-lookup"><span data-stu-id="a5f97-103">Having issues deleting SharePoint items?</span></span>

- <span data-ttu-id="a5f97-104">تأكد دائمًا من أن لديك [الأذونات](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) المناسبة لحذف العنصر أو أن يكون مسؤول [مجموعة الموقع](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) يحاول إزالة العنصر.</span><span class="sxs-lookup"><span data-stu-id="a5f97-104">Always make sure you have the [appropriate permissions](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) to delete the item or have a [site collection administrator](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) attempt remove the item.</span></span>

- <span data-ttu-id="a5f97-105">تأكد من عدم وجود إعداد [نهج استبقاء](https://docs.microsoft.com/office365/securitycompliance/retention-policies) على العنصر.</span><span class="sxs-lookup"><span data-stu-id="a5f97-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/office365/securitycompliance/retention-policies) setup on the item.</span></span>

- <span data-ttu-id="a5f97-106">تأكد من عدم [سحب](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) العنصر إلى مستخدم آخر.</span><span class="sxs-lookup"><span data-stu-id="a5f97-106">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

- <span data-ttu-id="a5f97-107">وأخيراً، يمكن للمسؤولين استخدام [أنماط وممارسات SharePoint](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) التي تحتوي على مكتبة أوامر PowerShell التي تسمح لك بتنفيذ إجراءات إدارة معقدة مثل فرض حذف العناصر العنيدة.</span><span class="sxs-lookup"><span data-stu-id="a5f97-107">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span>
- [<span data-ttu-id="a5f97-108">إزالة ملف PNP</span><span class="sxs-lookup"><span data-stu-id="a5f97-108">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="a5f97-109">إزالة مجلد PNP</span><span class="sxs-lookup"><span data-stu-id="a5f97-109">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="a5f97-110">إزالة عنصر قائمة PNP</span><span class="sxs-lookup"><span data-stu-id="a5f97-110">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="a5f97-111">إزالة قائمة PNP</span><span class="sxs-lookup"><span data-stu-id="a5f97-111">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="a5f97-112">إزالة حقل PNP (عمود)</span><span class="sxs-lookup"><span data-stu-id="a5f97-112">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)