---
title: شراء الخدمة الذاتية من PowerShell
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
- "3516"
ms.openlocfilehash: 5e47e08e3309b3d58908e10ee06021da00f230bb
ms.sourcegitcommit: cb9505f9eca032af3a4194c68d18c91789365690
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/16/2020
ms.locfileid: "42091653"
---
# <a name="self-service-purchase-of-powershell"></a>شراء الخدمة الذاتية من PowerShell

لاستخدام وحدة MSCommerce PowerShell، تحتاج إلى تثبيتها على جهاز Windows 10 مع TLS 1.2 (أذونات المسؤول المحلي المطلوبة).  استيراد وحدة MSCommerce والاتصال بها.  عند المطالبة بتسجيل الدخول، ستحتاج إلى استخدام بيانات اعتماد دور مسؤول الفوترة أو العمومية.  

إذا لم يكن لديك TLS 1.2، قد تتلقى الخطأ التالي عند محاولة الحصول على النهج أو تحديثه:

*خطأرسالة -تم إغلاق الاتصال الأساسي: حدث خطأ غير متوقع على إرسال*.



