---
title: قد يحتاج DLP إلى نوع مخصص
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 72b16d437f97de27cbdc364f022c3e2059b31ef0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47712171"
---
# <a name="dlp-might-need-a-custom-type"></a>قد يحتاج DLP إلى نوع مخصص

**هام**: خلال هذه الأوقات غير المسبوقة، نقوم باتخاذ الخطوات اللازمة لضمان توفر خدمات SharePoint Online و OneDrive بشكل كبير – الرجاء زيارة [تعديلات الميزات المؤقتة لـ SharePoint Online](https://aka.ms/ODSPAdjustments) للحصول على مزيد من المعلومات.

**قد يتطلب DLP نوع معلومات مخصصا**

باستخدام نهج تفادي فقدان البيانات (DLP) ، يمكنك تحديد البيانات الحساسة وحمايتها في مؤسستك. في بعض السيناريوهات ، قد تحتاج إلى إنشاء نوع المعلومات **الحساسة المخصصة** لحماية بيانات المؤسسة.

علي سبيل المثال ، قد تحتاج مؤسستك إلى تحديد معرفات الموظفين أو البيانات الأخرى وحمايتها بتنسيق مخصص لمؤسسك. إذا كان الأمر كذلك ، فراجع المقالات التالية للحصول علي مزيد من المعلومات.
  
 **تخصيص نوع المعلومات الحساسة المضمن**
  
إذا كان نوع المعلومات الحساسة المضمن يفي باحتياجاتك باستخدام بضع نهائي فقط ، فيمكنك [تخصيص نوع معلومات مضمن](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type). علي سبيل المثال ، يمكنك أضافه الكلمات الاساسيه أو ازالتها ، أو أضافه أو أزاله الادله المعتمدة مثل التاريخ أو العنوان.
  
 **إنشاء نوع معلومات حساس مخصص**
  
ولكن إذا كنت بحاجه إلى تحديد نوع آخر من المعلومات الهامه وحمايته تماما ، فيمكنك [إنشاء نوع معلومات حساس مخصص](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) في واجهه المستخدم الخاصة بمركز توافق & الأمان.
  
**إنشاء نوع معلومات حساس مخصص في مركز توافق & الأمان PowerShell**

وأخيرا ، إذا لم توفر واجهه المستخدم كل الخيارات التي تحتاج اليها ، فيمكنك [إنشاء نوع معلومات حساس مخصص في "مركز توافق ال& الأمان"](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell). بالبدء باستخدام ملف XML ، يمكنك استخدام كل خيار متوفر.
