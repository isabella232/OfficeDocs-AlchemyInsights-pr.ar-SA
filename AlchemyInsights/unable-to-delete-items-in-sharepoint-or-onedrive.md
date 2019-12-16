---
title: غير قادر علي حذف العناصر في SharePoint أو اندريف
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: cc19fcb6603160032dac52b1ec9e194a90b7891f
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/15/2019
ms.locfileid: "40049504"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="6aeb1-102">غير قادر علي حذف العناصر</span><span class="sxs-lookup"><span data-stu-id="6aeb1-102">Unable to delete items</span></span>

<span data-ttu-id="6aeb1-103">هل تواجه مشكلات في حذف عناصر SharePoint ؟</span><span class="sxs-lookup"><span data-stu-id="6aeb1-103">Having issues deleting SharePoint items?</span></span>

- <span data-ttu-id="6aeb1-104">تاكد دائما من ان لديك [الأذونات المناسبة](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) لحذف العنصر أو محاولة [مسؤول مجموعه موقع](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) أزاله العنصر.</span><span class="sxs-lookup"><span data-stu-id="6aeb1-104">Always make sure you have the [appropriate permissions](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) to delete the item or have a [site collection administrator](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) attempt remove the item.</span></span>

- <span data-ttu-id="6aeb1-105">تاكد من عدم وجود اعداد [نهج استبقاء](https://docs.microsoft.com/office365/securitycompliance/retention-policies) علي العنصر.</span><span class="sxs-lookup"><span data-stu-id="6aeb1-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/office365/securitycompliance/retention-policies) setup on the item.</span></span>

- <span data-ttu-id="6aeb1-106">تاكد من عدم [سحب](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) العنصر إلى مستخدم آخر.</span><span class="sxs-lookup"><span data-stu-id="6aeb1-106">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

- <span data-ttu-id="6aeb1-107">وأخيرا ، يمكن للمسؤولين استخدام [أنماط SharePoint والممارسات](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) الذي يحتوي علي مكتبه من الأوامر PowerShell التي تسمح لك بتنفيذ إجراءات أداره معقده مثل فرض حذف العناصر العنيدة.</span><span class="sxs-lookup"><span data-stu-id="6aeb1-107">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span>
- [<span data-ttu-id="6aeb1-108">أزاله ملف PNP</span><span class="sxs-lookup"><span data-stu-id="6aeb1-108">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="6aeb1-109">أزاله مجلد PNP</span><span class="sxs-lookup"><span data-stu-id="6aeb1-109">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="6aeb1-110">أزاله عنصر قائمه PNP</span><span class="sxs-lookup"><span data-stu-id="6aeb1-110">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="6aeb1-111">أزاله قائمه PNP</span><span class="sxs-lookup"><span data-stu-id="6aeb1-111">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="6aeb1-112">أزاله حقل PNP (عمود)</span><span class="sxs-lookup"><span data-stu-id="6aeb1-112">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)