---
title: غير قادر على تعيين أو عرض نهج AllowSelfServicePurchase
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 587a05cccbc71a970d4bd7723bff0df0c3b64ccc
ms.sourcegitcommit: 2a9d059262c07c33f9a740b3da4e6e3366b2f925
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/20/2020
ms.locfileid: "42158541"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a>غير قادر على تعيين أو عرض نهج AllowSelfServicePurchase

عند محاولة تعيين أو عرض نهج AllowSelfServicePurchase، تتلقى رسالة الخطأ التالية:

*مؤشر الخطأ: فشل في استرداد نهج المنتج باستخدام PolicyId "AllowSelfServicePurchase"، خطأرسالة - تم إغلاق الاتصال الأساسي: حدث خطأ غير متوقع على إرسال.*

قد يكون هذا بسبب إصدار أقدم من أمان طبقة النقل (TLS). لتوصيل خدمة MSCommerce ، تحتاج إلى استخدام TLS 1.2 أو أكبر.  

حاول الخطوات التالية لتمكين/تعيين بروتوكول TLS إلى 1.2، تحقق، وإعادة المحاولة.
 1. في موجه الأمر PowerShell (PS C:\) أدخل الأمر التالي لتعيين بروتوكول TLS إلى الإصدار 1.2:

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. تحقق من بروتوكول TLS (البروتوكولات) في الاستخدام، مع الأمر التالي:

    `[Net.ServicePointManager]::SecurityProtocol` 

3. إعادة محاولة أوامر الحصول على أو تحديث حسب الحاجة.

