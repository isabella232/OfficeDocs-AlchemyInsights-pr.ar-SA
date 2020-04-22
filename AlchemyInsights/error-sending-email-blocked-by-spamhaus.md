---
title: خطأ في إرسال البريد الإلكتروني المحظور من قبل SpamHaus
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
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 3ff4f7a155fe74f5b42a1bd43e67ef0a751d7fbd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43714245"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>خطأ إرسال البريد الإلكتروني: تم حظر مضيف العميل باستخدام Spamhaus

عنوان IP الذي أرسل الرسالة موجود على قائمة حظر مملوكة من [قبل Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245). تتضمن أسباب حظرالبريد الإلكتروني غير المرغوب فيه الحسابات التي تم اختراقها، والآلات التي تم اختراقها التي تشارك عنوان IP عامًا، وسياسات موفر خدمة الإنترنت (ISP). الإصلاحات المحتملة هي:
  
- بالنسبة للرسائل الواردة المحظورة حيث تتحكم في خادم البريد الإلكتروني المصدر، تحتاج إلى تحديد السبب وإزالة الحظر من موقع Spamhaus.

- بالنسبة للرسائل الواردة المحظورة حيث ينتمي عنوان IP المصدر إلى شخص آخر ، يحتاج مالك العنوان إلى إزالة الحظر من موقع Spamhaus. إذا كان عنوان IP موجودًا في قائمة كتلة النهج (PBL)، يمكن للمالك تعيين عنوان IP ثابت مختلف أو إزالة العنوان من PBL.

- بالنسبة للرسائل الصادرة المحظورة من نطاقك المتصل بـ Microsoft، يمكنك تلقي هذا الخطأ إذا تم توجيه الرسائل من خلال خدمة جهة خارجية. يمكنك استخدام أداة بحث WHOIS للعثور على مالك عنوان IP المحظور.
