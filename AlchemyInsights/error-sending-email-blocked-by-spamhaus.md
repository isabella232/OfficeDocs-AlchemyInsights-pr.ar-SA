---
title: خطأ في إرسال رسالة بريد إلكتروني يتم حظره بواسطة SpamHaus
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 2/23/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 52a5c20d59a2eac4c4bf465edaa888952d47f39f
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/28/2019
ms.locfileid: "35387836"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>خطأ في إرسال البريد الإلكتروني: حظر استخدام Spamhaus المضيف العميل

عنوان IP الذي يرسل الرسالة موجودة على قائمة حظر المملوكة [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245). حسابات المكسور، من بين أسباب منع قبل Spamhaus اختراق أجهزة مشاركة عنوان IP عمومي، ونهج موفر خدمة إنترنت (ISP). الإصلاحات الممكنة:
  
- مع الرسائل الواردة الممنوعة بحيث يمكنك التحكم خادم البريد الإلكتروني مصدر Office 365، تحتاج لتحديد السبب وإزالة الكتلة من موقع Spamhaus.

- المحظورة مع الرسائل الواردة إلى Office 365 حيث ينتمي عنوان IP المصدر لشخص آخر مالك عنوان يحتاج إلى إزالة الحظر من موقع Spamhaus. إذا كان عنوان IP على قائمة الحظر نهج (PBL)، يمكن تعيين عنوان IP ثابت آخر المالك أو إزالة العنوان من PBL.

- الرسائل الصادرة الممنوعة من المجال الخاص بك Office 365، يمكن تلقي هذا الخطأ إذا كان يتم توجيه الرسائل من خلال خدمة طرف ثالث. يمكنك استخدام أداة بحث WHOIS للبحث عن مالك عنوان IP المحظورة.
