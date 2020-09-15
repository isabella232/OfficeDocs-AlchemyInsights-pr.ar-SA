---
title: 1049 أنتيسبام 4.5.3 العديد من المستلمين (AS780090)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1049"
- "3100024"
ms.assetid: fa3d4be9-c90a-4926-9754-4b708b038bf6
ms.openlocfilehash: deb57e6e872ce5769a339c7d130a63a8e90ab4c8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717780"
---
# <a name="453-too-many-recipients-as780090"></a><span data-ttu-id="54b88-102">4.5.3 العديد من المستلمين (AS780090)</span><span class="sxs-lookup"><span data-stu-id="54b88-102">4.5.3 Too many recipients (AS780090)</span></span>

<span data-ttu-id="54b88-103">يحدث هذا الخطا عندما يتجاوز حجم نقل بيانات البريد الكتروني من عنوان IP المصدر الحد الذي يعتمد علي سمعه عنوان IP المصدر أو نقصه فيه.</span><span class="sxs-lookup"><span data-stu-id="54b88-103">This error occurs when the volume of email traffic from the source IP address exceeds the limit based on the reputation (or lack of reputation) of source IP address.</span></span>

<span data-ttu-id="54b88-104">ستنتهي صلاحيه حظر البريد الكتروني من عنوان IP المصدر في غضون ساعة.</span><span class="sxs-lookup"><span data-stu-id="54b88-104">Blocking email from the source IP address will expire within an hour.</span></span> <span data-ttu-id="54b88-105">إذا كان عنوان IP المصدر هو خادم البريد الكتروني المحلي الذي ينتمي اليك ، فتحقق من تكوين موصل تدفق البريد.</span><span class="sxs-lookup"><span data-stu-id="54b88-105">If the source IP address is an on-premises email server that belongs to you, verify the configuration of the mail flow connector.</span></span> <span data-ttu-id="54b88-106">إذا استمر السلوك لأكثر من ساعة ، فاتصل بقسم الدعم لطلب استثناء لعنوان IP المصدر.</span><span class="sxs-lookup"><span data-stu-id="54b88-106">If the behavior continues for more than an hour, contact support to request an exception for the source IP address.</span></span>
