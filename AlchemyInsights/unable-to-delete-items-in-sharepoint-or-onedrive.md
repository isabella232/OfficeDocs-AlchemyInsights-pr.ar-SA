---
title: غير قادر على حذف العناصر في SharePoint أو OneDrive
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
ms.openlocfilehash: abfcb91c6040aeed759d697ca63546ccea8ede97
ms.sourcegitcommit: c5e800313a6f211386a384716e5fa18e7fcc8c1c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/28/2020
ms.locfileid: "41571212"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="bd97c-102">غير قادر على حذف العناصر</span><span class="sxs-lookup"><span data-stu-id="bd97c-102">Unable to delete items</span></span>

<span data-ttu-id="bd97c-103">يمكن أن تتسبب نُهج الاحتفاظ في حدوث ذلك، تحتاج إما إلى تعطيل أو استبعاد احتجاز كل منهما الذي يسبب هذه المشكلة.</span><span class="sxs-lookup"><span data-stu-id="bd97c-103">Retention policies can cause this, you need to either disable or exclude respective hold that's causing this issue.</span></span> <span data-ttu-id="bd97c-104">بعد إزالة نهج الاحتفاظ أو الانتظار، قد يستغرق الأمر ما يصل إلى 24 ساعة حتى يسري التغيير.</span><span class="sxs-lookup"><span data-stu-id="bd97c-104">After a retention policy or hold is removed, it may take up to 24 hours for the change to take effect.</span></span> <span data-ttu-id="bd97c-105">تأكد من عدم وجود إعداد [نهج الاحتفاظ](https://docs.microsoft.com/office365/securitycompliance/retention-policies) على العنصر.</span><span class="sxs-lookup"><span data-stu-id="bd97c-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/office365/securitycompliance/retention-policies) setup on the item.</span></span>

<span data-ttu-id="bd97c-106">قد يكون الموقع قد تجاوز حد التخزين وزيادة [حصة الموقع وحذف](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) العنصر.</span><span class="sxs-lookup"><span data-stu-id="bd97c-106">The site might have exceeded storage limit, increase the [site quota](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) and delete the item.</span></span>

<span data-ttu-id="bd97c-107">تأكد من عدم [سحب](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) العنصر إلى مستخدم آخر.</span><span class="sxs-lookup"><span data-stu-id="bd97c-107">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

<span data-ttu-id="bd97c-108">وأخيراً، يمكن للمسؤولين استخدام [أنماط وممارسات SharePoint](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) التي تحتوي على مكتبة من أوامر PowerShell التي تسمح لك بتنفيذ إجراءات إدارة معقدة مثل فرض حذف العناصر العنيدة.</span><span class="sxs-lookup"><span data-stu-id="bd97c-108">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span>
- [<span data-ttu-id="bd97c-109">إزالة ملف PNP</span><span class="sxs-lookup"><span data-stu-id="bd97c-109">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="bd97c-110">إزالة مجلد PNP</span><span class="sxs-lookup"><span data-stu-id="bd97c-110">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="bd97c-111">إزالة عنصر قائمة PNP</span><span class="sxs-lookup"><span data-stu-id="bd97c-111">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="bd97c-112">إزالة قائمة PNP</span><span class="sxs-lookup"><span data-stu-id="bd97c-112">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="bd97c-113">إزالة حقل PNP (عمود)</span><span class="sxs-lookup"><span data-stu-id="bd97c-113">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)