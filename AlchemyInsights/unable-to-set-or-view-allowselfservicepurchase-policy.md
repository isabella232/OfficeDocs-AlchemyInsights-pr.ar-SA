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
ms.openlocfilehash: 255dbe35b808b3fe6b5707779251bf3f4a7e1c269c8b6f0ac2cb43ca03c469e9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54020179"
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

