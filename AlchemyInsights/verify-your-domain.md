---
title: التحقق من نطاقك
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "47"
- "48"
- "8"
ms.assetid: 81fd176b-3d67-4e52-9ab8-d36602412734
ms.openlocfilehash: 2c4d8e075d2cf7214b5ef005b856daf7fb0ed53c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43710430"
---
# <a name="verify-your-domain"></a><span data-ttu-id="f959e-102">التحقق من نطاقك</span><span class="sxs-lookup"><span data-stu-id="f959e-102">Verify your domain</span></span>

 <span data-ttu-id="f959e-103">**ربما لم يتم تحديث السجل عبر الإنترنت.**</span><span class="sxs-lookup"><span data-stu-id="f959e-103">**The record probably hasn't updated across the Internet.**</span></span>
  
<span data-ttu-id="f959e-104">عادة ما يستغرق الأمر بضع دقائق فقط حتى نتمكن من رؤية السجل الجديد ، ولكن في بعض الأحيان قد يستغرق الأمر بضع ساعات.</span><span class="sxs-lookup"><span data-stu-id="f959e-104">It typically only takes a few minutes for us to be able to see the new record, but occasionally it can take as long as a few hours.</span></span> 
  
- <span data-ttu-id="f959e-105">إذا انتظرت كل هذا الوقت، فتحقق مرة أخرى من أنك قمت بنسخ القيمة الدقيقة ولصقها في سجل التحقق من TXT في مضيف DNS.</span><span class="sxs-lookup"><span data-stu-id="f959e-105">If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host.</span></span> <span data-ttu-id="f959e-106">مشكلة واحدة مشتركة لا تتضمن "MS =" جزء من السجل.</span><span class="sxs-lookup"><span data-stu-id="f959e-106">One common issue is not including the "MS=" part of the record.</span></span> <span data-ttu-id="f959e-107">نحن بحاجة إلى ذلك أيضا!</span><span class="sxs-lookup"><span data-stu-id="f959e-107">We need that too!</span></span>

- <span data-ttu-id="f959e-108">في بعض مضيفي DNS، يجب عليك اتخاذ خطوة إضافية لحفظ ملف المنطقة (حيث يتم تخزين سجل DNS) بحيث سيتم تحديثه عبر الإنترنت.</span><span class="sxs-lookup"><span data-stu-id="f959e-108">At some DNS hosts, you have to take an extra step to save the zone file (where the DNS record is stored) so that it will update across the Internet.</span></span> <span data-ttu-id="f959e-109">تأكد من حفظ التغييرات حتى تتمكن Microsoft من رؤية السجل والتحقق منه.</span><span class="sxs-lookup"><span data-stu-id="f959e-109">Make sure you've saved your changes so Microsoft can see and verify the record.</span></span>
