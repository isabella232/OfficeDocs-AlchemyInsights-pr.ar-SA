---
title: خطأ في إرسال بريد إلكتروني تم حظره بواسطة SpamHaus
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
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 8372032e19bd2ebaf3ba8cc8e87f19ef3e2edf1e607b1739a919f6dcc443cd97
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53946680"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>خطأ في إرسال البريد الإلكتروني: تم حظر مضيف العميل باستخدام Spamhaus

يوجد عنوان IP الذي أرسل الرسالة في قائمة الحظر التي يملكها [Spamhaus.](https://go.microsoft.com/fwlink/p/?linkid=123245) تتضمن أسباب حظر البريد العشوائي الحسابات الم اختراق الأجهزة التي تشارك عنوان IP عام ونهج موفر خدمة الإنترنت (ISP). الإصلاحات المحتملة هي:
  
- بالنسبة للرسائل الواردة المحظورة حيث تتحكم في خادم البريد الإلكتروني المصدر، ستحتاج إلى تحديد السبب وإزالة الحظر من موقع Spamhaus على الويب.

- بالنسبة للرسائل الواردة المحظورة التي ينتمي فيها عنوان IP المصدر إلى شخص آخر، يحتاج مالك العنوان إلى إزالة الحظر من موقع Spamhaus على الويب. إذا كان عنوان IP في قائمة حظر النهج (PBL)، يمكن للمالك تعيين عنوان IP ثابت مختلف أو إزالة العنوان من PBL.

- بالنسبة للرسائل الصادرة المحظورة من مجالك المتصل ب Microsoft، يمكنك تلقي هذا الخطأ إذا تم توجيه الرسائل عبر خدمة جهة خارجية. يمكنك استخدام أداة البحث WHOIS للعثور على مالك عنوان IP المحظور.
