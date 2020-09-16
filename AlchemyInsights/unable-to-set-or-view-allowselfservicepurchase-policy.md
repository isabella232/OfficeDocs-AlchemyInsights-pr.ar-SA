---
title: تعذر تعيين نهج اللووسيلفسيرفيسيبوركهاسي أو عرضه
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 5ec16b3071f95ef52af2771e95137116222a3c5b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47735186"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a>تعذر تعيين نهج اللووسيلفسيرفيسيبوركهاسي أو عرضه

عند محاولة تعيين النهج اللووسيلفسيرفيسيبوركهاسي أو عرضه ، تتلقي رسالة الخطا التالية:

*هاندليرور: فشل استرداد نهج المنتج باستخدام بوليسييد ' اللووسيلفسيرفيسيبوركهاسي ' ، ارورميساجي-تم إغلاق الاتصال الأساسي: حدث خطا غير متوقع في الإرسال.*

قد يعود ذلك إلى إصدار سابق من أمان طبقه النقل (TLS). للاتصال بخدمه مسكوميرسي ، يجب استخدام TLS 1.2 أو الأحدث.  

جرب الخطوات التالية لتمكين/تعيين بروتوكول TLS إلى 1.2 والتحقق منه وأعاده المحاولة.
 1. في موجه الأوامر PowerShell (PS C: \) ادخل الأمر التالي لتعيين بروتوكول TLS إلى الإصدار 1.2:

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. تاكد من استخدام الأمر (بروتوكولات) TLS ، وذلك بالأوامر التالية:

    `[Net.ServicePointManager]::SecurityProtocol` 

3. أعد محاولة تنفيذ الأمرين Get أو Update كما تقتضي الحاجة.

