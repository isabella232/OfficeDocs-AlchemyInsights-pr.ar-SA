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
ms.openlocfilehash: 5a383bdd17c5fa055c35a923ca36e0e0f6d429e4
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/28/2019
ms.locfileid: "35380492"
---
# <a name="unable-to-set-primary-email-address-or-change-user-attributes"></a>غير قادر على تعيين عنوان البريد الإلكتروني الأساسي أو تغيير خصائص المستخدم

إذا تم تمكين مزامنة الدليل للبيئة الخاصة بك لا تغيير بعض خصائص المستخدم أو الكائن استخدام مركز الإدارة.
لإدارة المستخدمين المتزامنة والسمات الخاصة بها بشكل كامل، استخدم الدليل النشط المحلي مستخدمين ومجموعات إدارة وحدة التحكم (adsiedit.msc).  

بدلاً من ذلك، يمكنك تغيير المستخدمين الفرديين أو سمات للمستخدمين متزامنة باستخدام powershell مثل المعروضة في هذه الأمثلة الشائعة: 
- مجموعة مسولوسير user2@yourvanitydomain.onmicrosoft.com-التيرناتيمايلادريسيس user@yourdomain.onmicrosoft.com-UserPrincipalName
- مجموعة مسولوسير-UserPrincipalName "user@yourdomain.onmicrosoft.com"-اسم العرض "اختبار المستخدم"-"اسم العائلة" "المستخدم"-العنوان "مدير"-قسم "الموارد البشرية"
- إزالة مسولوسير-UserPrincipalName "user@yourdomain.onmicrosoft.com