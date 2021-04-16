---
title: شراء الخدمة الذاتية من PowerShell
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
- "3516"
ms.openlocfilehash: 48b5b0a1be1bc03d45a531a1093f18a3f750c37d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51797708"
---
# <a name="self-service-purchase-of-powershell"></a>شراء الخدمة الذاتية من PowerShell

لاستخدام وحدة MSCommerce PowerShell النمطية، تحتاج إلى تثبيتها على جهاز يعمل بنظام التشغيل Windows 10 باستخدام TLS 1.2 (أذونات المسؤول المحلي مطلوبة).  استيراد وحدة MSCommerce النمطية والاتصال بها.  عند مطالبتك بتسجيل الدخول، ستحتاج إلى استخدام بيانات اعتماد دور مسؤول الفوترة أو العام.  

إذا لم يكن لديك TLS 1.2، فقد تتلقى الخطأ التالي عند محاولة الحصول على النهج أو تحديثه:

*ErrorMessage -تم إغلاق* الاتصال الأساسي: حدث خطأ غير متوقع في عملية إرسال .



