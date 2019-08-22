---
title: تحقق من المجال الخاص بك
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/5/2018
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
ms.openlocfilehash: 3dd96a9731cfd75882dd3bb397005b19d471c882
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/22/2019
ms.locfileid: "36531346"
---
# <a name="verify-your-domain"></a><span data-ttu-id="a1fb7-102">تحقق من المجال الخاص بك</span><span class="sxs-lookup"><span data-stu-id="a1fb7-102">Verify your domain</span></span>

 <span data-ttu-id="a1fb7-103">**ربما لم تحديث السجل عبر الإنترنت.**</span><span class="sxs-lookup"><span data-stu-id="a1fb7-103">**The record probably hasn't updated across the Internet.**</span></span>
  
<span data-ttu-id="a1fb7-104">عادة ما يستغرق سوى بضع دقائق لكي نستطيع أن نرى السجل الجديد، ولكن أحياناً قد يستغرق ما دام بضع ساعات.</span><span class="sxs-lookup"><span data-stu-id="a1fb7-104">It typically only takes a few minutes for us to be able to see the new record, but occasionally it can take as long as a few hours.</span></span> 
  
- <span data-ttu-id="a1fb7-105">إذا كنت قد انتظرت طويلة مسبقاً، تأكد من أنه تم نسخ ولصق القيمة في السجل التحقق TXT في مضيف DNS الخاص بك.</span><span class="sxs-lookup"><span data-stu-id="a1fb7-105">If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host.</span></span> <span data-ttu-id="a1fb7-106">مسألة عامة لا يتضمن "MS =" جزءا من السجل.</span><span class="sxs-lookup"><span data-stu-id="a1fb7-106">One common issue is not including the "MS=" part of the record.</span></span> <span data-ttu-id="a1fb7-107">نحن بحاجة أن جداً!</span><span class="sxs-lookup"><span data-stu-id="a1fb7-107">We need that too!</span></span>

- <span data-ttu-id="a1fb7-108">في بعض مضيفي DNS, يجب عليك إجراء خطوة إضافية لحفظ ملف المنطقة (حيث يتم تخزين سجل DNS) حيث أنه سيتم تحديث عبر الإنترنت.</span><span class="sxs-lookup"><span data-stu-id="a1fb7-108">At some DNS hosts, you have to take an extra step to save the zone file (where the DNS record is stored) so that it will update across the Internet.</span></span> <span data-ttu-id="a1fb7-109">تأكد من أن يتم حفظ التغييرات الخاصة بك حيث يمكنك مشاهدة Office 365 والتحقق من السجل.</span><span class="sxs-lookup"><span data-stu-id="a1fb7-109">Make sure you've saved your changes so Office 365 can see and verify the record.</span></span>
