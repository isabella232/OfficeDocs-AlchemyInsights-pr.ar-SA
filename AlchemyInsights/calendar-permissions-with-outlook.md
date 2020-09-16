---
title: أذونات التقويم
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800009"
- "611"
ms.openlocfilehash: cfee520e26587c0a649c08084853c31232d027f8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47748780"
---
# <a name="calendar-permissions"></a><span data-ttu-id="2821c-102">أذونات التقويم</span><span class="sxs-lookup"><span data-stu-id="2821c-102">Calendar Permissions</span></span>

<span data-ttu-id="2821c-103">يمكن للمستخدمين تغيير أذونات التقويم الخاصة بهم باستخدام Outlook علي الويب أو العملاء الآخرين ، ولكن كمسؤول قد تحتاج إلى التحقق منه أيضا.</span><span class="sxs-lookup"><span data-stu-id="2821c-103">Users can change their own Calendar Permissions with Outlook on the Web or other clients, but as an admin you may need to investigate as well.</span></span>  
<span data-ttu-id="2821c-104">باستخدام Exchange PowerShell cmdlet سيعرض لك الاذن في تقويم المستخدم:</span><span class="sxs-lookup"><span data-stu-id="2821c-104">With Exchange PowerShell cmdlet will show you the permission on a user’s calendar:</span></span>

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

<span data-ttu-id="2821c-105">للاطلاع علي مزيد من المعلومات ، راجع ما يلي:</span><span class="sxs-lookup"><span data-stu-id="2821c-105">To see more information see the following:</span></span>

- [<span data-ttu-id="2821c-106">مايلبوكسفولديربيرميسيون</span><span class="sxs-lookup"><span data-stu-id="2821c-106">Get-MailboxFolderPermission</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [<span data-ttu-id="2821c-107">ميلبوكسفولديربيرميشن</span><span class="sxs-lookup"><span data-stu-id="2821c-107">Set-MailboxFolderPermission</span></span>](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [<span data-ttu-id="2821c-108">الوظائف الاضافيه ميلبوكسفولديربيرميشن</span><span class="sxs-lookup"><span data-stu-id="2821c-108">Add-MailboxFolderPermission</span></span>](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

<span data-ttu-id="2821c-109">يتم استخدام أذونات التقويم في مشاركه التقويمات ، للاطلاع علي مزيد من المعلومات حول مشاركه تقويم Outlook ، راجع المقالات التالية:</span><span class="sxs-lookup"><span data-stu-id="2821c-109">Calendar Permissions are used in the sharing of calendars, to see more information about sharing an Outlook calendar, see these articles:</span></span>

- [<span data-ttu-id="2821c-110">مشاركة تقويم Outlook مع أشخاص آخرين</span><span class="sxs-lookup"><span data-stu-id="2821c-110">Share an Outlook calendar with other people</span></span>](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [<span data-ttu-id="2821c-111">مشاركه التقويم في Outlook علي الويب للاعمال</span><span class="sxs-lookup"><span data-stu-id="2821c-111">Share your calendar in Outlook on the web for business</span></span>](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

<span data-ttu-id="2821c-112">لاستكشاف أخطاء التقويم وإصلاحها ، يمكنك استخدام أداه [مساعد الإصلاح والدعم](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) .</span><span class="sxs-lookup"><span data-stu-id="2821c-112">To troubleshoot Calendar Permission you can use the [Support and Recovery Assistant](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) tool.</span></span>