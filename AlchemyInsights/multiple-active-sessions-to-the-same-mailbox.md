---
title: جلسات عمل نشطة متعددة إلى نفس علبة البريد
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1836"
- "9000248"
ms.openlocfilehash: d2fd3f20346012baed21efd4900ca4cf73391d91
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 07/28/2020
ms.locfileid: "45438674"
---
# <a name="multiple-active-sessions-to-the-same-mailbox"></a><span data-ttu-id="77b24-102">جلسات عمل نشطة متعددة إلى نفس علبة البريد</span><span class="sxs-lookup"><span data-stu-id="77b24-102">Multiple active sessions to the same mailbox</span></span>

<span data-ttu-id="77b24-103">للتحكم في استخدام موارد Exchange، علبة بريد لها "ميزانية".</span><span class="sxs-lookup"><span data-stu-id="77b24-103">To control usage of Exchange resources, a mailbox has a "budget."</span></span>

<span data-ttu-id="77b24-104">يمكن تشغيل استثناء الموازنة المفرطة، ولكن لا يقتصر على، الظروف التالية:</span><span class="sxs-lookup"><span data-stu-id="77b24-104">The over-budget exception can be triggered by, but is not limited to, the following circumstances:</span></span>

- <span data-ttu-id="77b24-105">يتم فتح بعض علامات التبويب المستعرض داخل نفس جلسة عمل Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="77b24-105">A few browser tabs are opened within the same Outlook Web App session.</span></span>

- <span data-ttu-id="77b24-106">بعض جلسات عمل Outlook Web App النشطة إلى نفس علبة البريد.</span><span class="sxs-lookup"><span data-stu-id="77b24-106">A few active Outlook Web App sessions to the same mailbox.</span></span>

- <span data-ttu-id="77b24-107">عدد قليل من التطبيقات العميل الأخرى (Outlook، أوتلوك موبايل، تطبيق عميل جهة خارجية) الوصول إلى علبة البريد في نفس الوقت.</span><span class="sxs-lookup"><span data-stu-id="77b24-107">A few other client applications (Outlook, Outlook Mobile, a third party client app) access the mailbox at the same time.</span></span>

- <span data-ttu-id="77b24-108">يتم تنفيذ عمليات التشغيل الطويلة، مثل تنفيذ طلبات البحث، من جلسة عمل أخرى نشطة لعلبة البريد.</span><span class="sxs-lookup"><span data-stu-id="77b24-108">Long running operations, such as executing search requests, are performed from another active mailbox session.</span></span>

