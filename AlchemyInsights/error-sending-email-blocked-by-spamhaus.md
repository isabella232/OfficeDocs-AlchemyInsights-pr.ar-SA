---
title: خطا في إرسال البريد الكتروني المحظور بواسطة SpamHaus
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
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: a0c2f4be0b2d8ba6fd3dadbdf306e6ce623ad380
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47783754"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>خطا في إرسال البريد الكتروني: تم حظر مضيف العميل باستخدام Spamhaus

يكون عنوان IP الذي أرسل الرسالة في قائمه حظر مملوكه ل [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245). تشمل الأسباب التي يتم حظرها بواسطة Spamhaus الحسابات التي تم اختراقها ومشاركه عناوين IP العامة ونهج موفر خدمه الإنترنت (ISP). التصحيحات المحتملة هي:
  
- بالنسبة إلى الرسائل الواردة المحظورة حيث تتحكم في خادم البريد الكتروني المصدر ، يجب تحديد السبب وأزاله الحظر من موقع Spamhaus علي ويب.

- بالنسبة إلى الرسائل الواردة المحظورة التي ينتمي اليها عنوان IP المصدر لشخص آخر ، يحتاج مالك العنوان إلى أزاله الحظر من موقع ويب Spamhaus. إذا كان عنوان IP في قائمه حظر النهج (ببل) ، فبامكان المالك تعيين عنوان IP ثابت مختلف أو أزاله العنوان من ببل.

- بالنسبة إلى الرسائل الصادرة المحظورة من المجال المتصل ب Microsoft ، يمكنك تلقي هذا الخطا إذا كانت الرسائل موجهه عبر خدمه الطرف الخارجي. يمكنك استخدام أداه البحث في WHOIS للعثور علي مالك عنوان IP المحظور.
