---
title: تعذر تعيين نهج AllowSelfServicePurchase أو عرضه
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 8dac2bdc20905cf37fc30317d9b371bfd755f452
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826078"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a>تعذر تعيين نهج AllowSelfServicePurchase أو عرضه

عند محاولة تعيين نهج AllowSelfServicePurchase أو عرضه، ستتلقى رسالة الخطأ التالية:

*معالج : فشل استرداد نهج المنتج باستخدام PolicyId 'AllowSelfServicePurchase', ErrorMessage - تم إغلاق الاتصال الأساسي: حدث خطأ غير متوقع في عملية إرسال.*

قد يعود سبب ذلك إلى إصدار أقدم من "أمان طبقة النقل" (TLS). لتوصيل خدمة MSCommerce، تحتاج إلى استخدام TLS 1.2 أو أكبر.  

جرب الخطوات التالية لتمكين/تعيين بروتوكول TLS إلى 1.2 والتحقق من الصحة والمحاولة مرة أخرى.
 1. في موجه الأوامر PowerShell (PS C: أدخل الأمر التالي لتعيين \) بروتوكول TLS إلى الإصدار 1.2:

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. تحقق من بروتوكول (بروتوكولات) TLS (بروتوكولات) TLS المستخدم، باستخدام الأمر التالي:

    `[Net.ServicePointManager]::SecurityProtocol` 

3. إعادة محاولة الأمرين الحصول أو التحديث حسب الحاجة.

