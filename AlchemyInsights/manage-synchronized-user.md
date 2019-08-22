---
title: إدارة مستخدم متزامن
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000609"
- "2444"
ms.openlocfilehash: a943c59d67c512e6326856dacd0053db121f6aa3
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/22/2019
ms.locfileid: "36541968"
---
# <a name="unable-to-set-primary-email-address-or-change-user-attributes"></a>غير قادر على تعيين عنوان البريد الإلكتروني الأساسي أو تغيير خصائص المستخدم

إذا تم تمكين مزامنة الدليل للبيئة الخاصة بك، يتعذر تغيير بعض خصائص المستخدم أو الكائن استخدام مركز مسؤول Microsoft 365.

لإدارة المستخدمين المتزامنة والسمات الخاصة بها بشكل كامل، استخدم الدليل النشط المحلي مستخدمين ومجموعات إدارة وحدة التحكم (adsiedit.msc).  

بدلاً من ذلك، يمكنك تغيير المستخدمين الفرديين أو سمات للمستخدمين متزامنة باستخدام powershell مثل المعروضة في هذه الأمثلة الشائعة: 
- مجموعة مسولوسير user2@yourvanitydomain.onmicrosoft.com-التيرناتيمايلادريسيس user@yourdomain.onmicrosoft.com-UserPrincipalName
- مجموعة مسولوسير-UserPrincipalName "user@yourdomain.onmicrosoft.com"-اسم العرض "اختبار المستخدم"-"اسم العائلة" "المستخدم"-العنوان "مدير"-قسم "الموارد البشرية"
- إزالة مسولوسير-UserPrincipalName "user@yourdomain.onmicrosoft.com