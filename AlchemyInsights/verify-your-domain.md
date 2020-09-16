---
title: التحقق من المجال
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: d30f9b51c0164acd126f214a581ad6cec5eec04e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47734293"
---
# <a name="verify-your-domain"></a><span data-ttu-id="4da45-102">التحقق من المجال</span><span class="sxs-lookup"><span data-stu-id="4da45-102">Verify your domain</span></span>

 <span data-ttu-id="4da45-103">**من المحتمل عدم تحديث السجل عبر الإنترنت.**</span><span class="sxs-lookup"><span data-stu-id="4da45-103">**The record probably hasn't updated across the Internet.**</span></span>
  
<span data-ttu-id="4da45-104">عاده ما يستغرق الأمر بضع دقائق فقط لكي يتمكنوا من رؤية السجل الجديد ، ولكن قد يستغرق الأمر بضع ساعات.</span><span class="sxs-lookup"><span data-stu-id="4da45-104">It typically only takes a few minutes for us to be able to see the new record, but occasionally it can take as long as a few hours.</span></span> 
  
- <span data-ttu-id="4da45-105">إذا قمت بالانتهاء من هذا الوقت بالفعل ، فتاكد من انك قمت بنسخ القيمة الصحيحة ولصقها في سجل التحقق من الصحة TXT لدي مضيف DNS.</span><span class="sxs-lookup"><span data-stu-id="4da45-105">If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host.</span></span> <span data-ttu-id="4da45-106">هناك مشكله واحده شائعه لا تتضمن الجزء "MS =" من السجل.</span><span class="sxs-lookup"><span data-stu-id="4da45-106">One common issue is not including the "MS=" part of the record.</span></span> <span data-ttu-id="4da45-107">نحتاج أيضا إلى ذلك!</span><span class="sxs-lookup"><span data-stu-id="4da45-107">We need that too!</span></span>

- <span data-ttu-id="4da45-108">في بعض مضيفي DNS ، يجب اجراء خطوه اضافيه لحفظ ملف المنطقة (حيث يتم تخزين سجل DNS) بحيث يتم تحديثه عبر الإنترنت.</span><span class="sxs-lookup"><span data-stu-id="4da45-108">At some DNS hosts, you have to take an extra step to save the zone file (where the DNS record is stored) so that it will update across the Internet.</span></span> <span data-ttu-id="4da45-109">تاكد من انك قمت بحفظ التغييرات التي أجريتها لكي تتمكن Microsoft من رؤية السجل والتحقق منه.</span><span class="sxs-lookup"><span data-stu-id="4da45-109">Make sure you've saved your changes so Microsoft can see and verify the record.</span></span>
