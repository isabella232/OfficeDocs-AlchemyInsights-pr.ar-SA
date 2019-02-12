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
ms.custom: Adm_O365
ms.assetid: 81fd176b-3d67-4e52-9ab8-d36602412734
ms.openlocfilehash: 7332650d1763e2bbd13be48f406fb04b8849a6c1
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/12/2019
ms.locfileid: "29911219"
---
# <a name="verify-your-domain"></a><span data-ttu-id="68b5c-102">تحقق من المجال الخاص بك</span><span class="sxs-lookup"><span data-stu-id="68b5c-102">Verify your domain</span></span>

 <span data-ttu-id="68b5c-103">**ربما لم تحديث السجل عبر الإنترنت.**</span><span class="sxs-lookup"><span data-stu-id="68b5c-103">**The record probably hasn't updated across the Internet.**</span></span>
  
<span data-ttu-id="68b5c-104">عادة ما يستغرق سوى بضع دقائق لكي نستطيع أن نرى السجل الجديد، ولكن أحياناً قد يستغرق ما دام بضع ساعات.</span><span class="sxs-lookup"><span data-stu-id="68b5c-104">It typically only takes a few minutes for us to be able to see the new record, but occasionally it can take as long as a few hours.</span></span> 
  
- <span data-ttu-id="68b5c-p101">إذا كنت قد انتظرت طويلة مسبقاً، تأكد من أنه تم نسخ ولصق القيمة في السجل التحقق TXT في مضيف DNS الخاص بك. مسألة عامة لا يتضمن "MS =" جزءا من السجل. نحن بحاجة أن جداً!</span><span class="sxs-lookup"><span data-stu-id="68b5c-p101">If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host. One common issue is not including the "MS=" part of the record. We need that too!</span></span>
    
- <span data-ttu-id="68b5c-p102">في بعض مضيفي DNS, يجب عليك إجراء خطوة إضافية لحفظ ملف المنطقة (حيث يتم تخزين سجل DNS) حيث أنه سيتم تحديث عبر الإنترنت. تأكد من أن يتم حفظ التغييرات الخاصة بك حيث يمكنك مشاهدة Office 365 والتحقق من السجل.</span><span class="sxs-lookup"><span data-stu-id="68b5c-p102">At some DNS hosts, you have to take an extra step to save the zone file (where the DNS record is stored) so that it will update across the Internet. Make sure you've saved your changes so Office 365 can see and verify the record.</span></span>
    

