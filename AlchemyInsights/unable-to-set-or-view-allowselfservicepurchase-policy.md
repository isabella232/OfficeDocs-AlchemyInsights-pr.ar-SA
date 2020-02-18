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
ms.openlocfilehash: a9b6e36e8034e71b3e72c49e3cc68a126ef97aca
ms.sourcegitcommit: cb9505f9eca032af3a4194c68d18c91789365690
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/16/2020
ms.locfileid: "42091654"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a>غير قادر على تعيين أو عرض نهج AllowSelfServicePurchase

عند محاولة تعيين أو عرض نهج AllowSelfServicePurchase، تتلقى رسالة الخطأ التالية:

*مؤشر الخطأ: فشل في استرداد نهج المنتج باستخدام PolicyId "AllowSelfServicePurchase"، خطأرسالة - تم إغلاق الاتصال الأساسي: حدث خطأ غير متوقع على إرسال.*

قد يكون هذا بسبب إصدار أقدم من أمان طبقة النقل (TLS). لتوصيل خدمة MSCommerce ، تحتاج إلى استخدام TLS 1.2 أو أكبر.  

حاول الخطوات التالية لتمكين/تعيين بروتوكول TLS إلى 1.2، تحقق، وإعادة المحاولة.
 1. في موجه الأمر PowerShell (PS C:\) أدخل الأمر التالي لتعيين بروتوكول TLS إلى الإصدار 1.2:

    \[Net.ServicePointManager]::بروتوكول الأمن \[= Net.SecurityProtocolType]::Tls12

2. تحقق من بروتوكول TLS (البروتوكولات) في الاستخدام، مع الأمر التالي:

    \[Net.ServicePointManager]::بروتوكول الأمن 

3. إعادة محاولة أوامر الحصول على أو تحديث حسب الحاجة.

