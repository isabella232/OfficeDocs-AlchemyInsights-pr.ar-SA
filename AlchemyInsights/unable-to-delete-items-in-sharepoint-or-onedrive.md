---
title: تعذر حذف العناصر في SharePoint أو OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: fd12115214cc28b822cf7fa57fe9b86f76f7beb1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806098"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="9dfae-102">تعذر حذف العناصر</span><span class="sxs-lookup"><span data-stu-id="9dfae-102">Unable to delete items</span></span>

<span data-ttu-id="9dfae-103">يمكن ان تتسبب نهج الاستبقاء بهذا الأمر ، ستحتاج إلى تعطيل التعليق أو استبعاده الذي يسبب هذه المشكلة.</span><span class="sxs-lookup"><span data-stu-id="9dfae-103">Retention policies can cause this, you need to either disable or exclude respective hold that's causing this issue.</span></span> <span data-ttu-id="9dfae-104">بعد أزاله نهج الاستبقاء أو التعليق ، قد تستغرق التغييرات حيز التنفيذ حتى 24 ساعة.</span><span class="sxs-lookup"><span data-stu-id="9dfae-104">After a retention policy or hold is removed, it may take up to 24 hours for the change to take effect.</span></span> <span data-ttu-id="9dfae-105">تاكد من عدم وجود اعداد [نهج استبقاء](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) علي العنصر.</span><span class="sxs-lookup"><span data-stu-id="9dfae-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) setup on the item.</span></span>

<span data-ttu-id="9dfae-106">ربما تجاوز الموقع حد مساحة التخزين ، ويزيد [الحصة النسبية للموقع](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) ويحذف العنصر.</span><span class="sxs-lookup"><span data-stu-id="9dfae-106">The site might have exceeded storage limit, increase the [site quota](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) and delete the item.</span></span>

<span data-ttu-id="9dfae-107">تاكد من [عدم سحب العنصر إلى مستخدم](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) آخر.</span><span class="sxs-lookup"><span data-stu-id="9dfae-107">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

<span data-ttu-id="9dfae-108">في النهاية ، يمكن للمسؤولين استخدام [أنماط وممارسات SharePoint](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) التي تحتوي علي مكتبه لأوامر PowerShell التي تسمح لك بتنفيذ إجراءات الاداره المعقدة مثل فرض حذف العناصر الستوبورنه.</span><span class="sxs-lookup"><span data-stu-id="9dfae-108">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span>
- [<span data-ttu-id="9dfae-109">أزاله ملف PNP</span><span class="sxs-lookup"><span data-stu-id="9dfae-109">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="9dfae-110">أزاله مجلد PNP</span><span class="sxs-lookup"><span data-stu-id="9dfae-110">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="9dfae-111">أزاله عنصر قائمه PNP</span><span class="sxs-lookup"><span data-stu-id="9dfae-111">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="9dfae-112">أزاله قائمه PNP</span><span class="sxs-lookup"><span data-stu-id="9dfae-112">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="9dfae-113">أزاله حقل PNP (عمود)</span><span class="sxs-lookup"><span data-stu-id="9dfae-113">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)