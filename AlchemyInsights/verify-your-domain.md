---
title: التحقق من مجالك
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "47"
- "48"
- "8"
ms.assetid: 81fd176b-3d67-4e52-9ab8-d36602412734
ms.openlocfilehash: 4a34de7fa2aaaae365cf4562d31590d4b5fb7544
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51770978"
---
# <a name="verify-your-domain"></a><span data-ttu-id="23c69-102">التحقق من مجالك</span><span class="sxs-lookup"><span data-stu-id="23c69-102">Verify your domain</span></span>

 <span data-ttu-id="23c69-103">**على الأرجح لم يتم تحديث السجل عبر الإنترنت.**</span><span class="sxs-lookup"><span data-stu-id="23c69-103">**The record probably hasn't updated across the Internet.**</span></span>
  
<span data-ttu-id="23c69-104">يستغرق الأمر عادة بضع دقائق لكي نتمكن من رؤية السجل الجديد، ولكن قد يستغرق ذلك أحيانا بضع ساعات.</span><span class="sxs-lookup"><span data-stu-id="23c69-104">It typically only takes a few minutes for us to be able to see the new record, but occasionally it can take as long as a few hours.</span></span> 
  
- <span data-ttu-id="23c69-105">إذا انتظرت هذه المدة، فتحقق مرة أخرى من أنك نسخت القيمة الدقيقة ولصقتها في سجل التحقق من صحة TXT لدى مضيف DNS.</span><span class="sxs-lookup"><span data-stu-id="23c69-105">If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host.</span></span> <span data-ttu-id="23c69-106">إحدى المشاكل الشائعة هي عدم بما في ذلك الجزء "MS=" من السجل.</span><span class="sxs-lookup"><span data-stu-id="23c69-106">One common issue is not including the "MS=" part of the record.</span></span> <span data-ttu-id="23c69-107">نحتاج إلى ذلك أيضا!</span><span class="sxs-lookup"><span data-stu-id="23c69-107">We need that too!</span></span>

- <span data-ttu-id="23c69-108">في بعض مضيفي DNS، يجب عليك اتخاذ خطوة إضافية لحفظ ملف المنطقة (حيث يتم تخزين سجل DNS) بحيث يتم تحديثه عبر الإنترنت.</span><span class="sxs-lookup"><span data-stu-id="23c69-108">At some DNS hosts, you have to take an extra step to save the zone file (where the DNS record is stored) so that it will update across the Internet.</span></span> <span data-ttu-id="23c69-109">تأكد من حفظ التغييرات حتى تتمكن Microsoft من رؤية السجل والتحقق منه.</span><span class="sxs-lookup"><span data-stu-id="23c69-109">Make sure you've saved your changes so Microsoft can see and verify the record.</span></span>
