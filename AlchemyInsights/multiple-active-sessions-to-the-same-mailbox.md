---
title: العديد من الجلسات النشطة إلى علبه البريد نفسها
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1836"
- "9000248"
ms.openlocfilehash: f4ae5c5afef9972ad4ffe74144d702ed58b2f437
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47769710"
---
# <a name="multiple-active-sessions-to-the-same-mailbox"></a><span data-ttu-id="f3b07-102">العديد من الجلسات النشطة إلى علبه البريد نفسها</span><span class="sxs-lookup"><span data-stu-id="f3b07-102">Multiple active sessions to the same mailbox</span></span>

<span data-ttu-id="f3b07-103">للتحكم في استخدام موارد Exchange ، تحتوي علبه البريد علي "الموازنة".</span><span class="sxs-lookup"><span data-stu-id="f3b07-103">To control usage of Exchange resources, a mailbox has a "budget."</span></span>

<span data-ttu-id="f3b07-104">يمكن تشغيل استثناء الموازنة بواسطة ، ولكنه غير محدود بالظروف التالية:</span><span class="sxs-lookup"><span data-stu-id="f3b07-104">The over-budget exception can be triggered by, but is not limited to, the following circumstances:</span></span>

- <span data-ttu-id="f3b07-105">يتم فتح بعض علامات تبويب المستعرض داخل جلسة عمل Outlook Web App نفسها.</span><span class="sxs-lookup"><span data-stu-id="f3b07-105">A few browser tabs are opened within the same Outlook Web App session.</span></span>

- <span data-ttu-id="f3b07-106">بعض جلسات عمل Outlook Web App النشطة إلى علبه البريد نفسها.</span><span class="sxs-lookup"><span data-stu-id="f3b07-106">A few active Outlook Web App sessions to the same mailbox.</span></span>

- <span data-ttu-id="f3b07-107">يقوم بعض تطبيقات العملاء الأخرى (Outlook ، Outlook Mobile ، تطبيق عميل تابع لجهة خارجيه) بالوصول إلى علبه البريد في الوقت نفسه.</span><span class="sxs-lookup"><span data-stu-id="f3b07-107">A few other client applications (Outlook, Outlook Mobile, a third party client app) access the mailbox at the same time.</span></span>

- <span data-ttu-id="f3b07-108">يتم تنفيذ عمليات التشغيل الطويلة ، مثل تنفيذ طلبات البحث ، من جلسة أخرى نشطه في علبه البريد.</span><span class="sxs-lookup"><span data-stu-id="f3b07-108">Long running operations, such as executing search requests, are performed from another active mailbox session.</span></span>

