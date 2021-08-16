---
title: قد تحتاج DLP إلى نوع مخصص
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
ms.openlocfilehash: 1b0beb89eaf8a4105659a1faa7cc723174a73940ef46bd2355bdddfee7b94adb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54030781"
---
# <a name="dlp-might-need-a-custom-type"></a>قد تحتاج DLP إلى نوع مخصص

**هام**: خلال هذه الأوقات غير المسبوقة، نقوم باتخاذ الخطوات اللازمة لضمان توفر خدمات SharePoint Online و OneDrive بشكل كبير – الرجاء زيارة [تعديلات الميزات المؤقتة لـ SharePoint Online](https://aka.ms/ODSPAdjustments) للحصول على مزيد من المعلومات.

**قد تتطلب DLP نوع معلومات مخصص**

باستخدام نهج منع فقدان البيانات (DLP)، يمكنك تحديد البيانات الحساسة وحمايتها في مؤسستك. في بعض السيناريوهات، قد تحتاج  إلى إنشاء نوع المعلومات الحساسة المخصص لحماية بيانات مؤسستك.

على سبيل المثال، قد تحتاج مؤسستك إلى تحديد هوية الموظفين أو البيانات الأخرى وحمايتها بتنسيق خاص بالم مؤسستك. إذا كان الأمر كذلك، راجع المقالات التالية للحصول على مزيد من المعلومات.
  
 **تخصيص نوع معلومات حساسة مضمن**
  
إذا كان نوع المعلومات الحساسة المضمن يلبي احتياجاتك من خلال بعض التعديلات فقط، يمكنك تخصيص نوع معلومات حساسة [مضمن.](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type) على سبيل المثال، يمكنك إضافة كلمات أساسية أو إزالتها، أو إضافة أدلة دعم أو إزالتها مثل تاريخ أو عنوان.
  
 **إنشاء نوع معلومات حساسة مخصصة**
  
ولكن إذا كنت بحاجة إلى تحديد نوع مختلف من المعلومات [](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) الحساسة وحمايتها تماما، يمكنك إنشاء نوع معلومات مخصص حساس في واجهة مستخدم مركز التوافق & الأمان.
  
**إنشاء نوع معلومات حساسة مخصصة في مركز & التوافق PowerShell**

وأخيرا، إذا لم توفر واجهة المستخدم كل الخيارات التي تحتاج إليها، يمكنك إنشاء نوع معلومات مخصص حساس في أمان & [مركز التوافق PowerShell](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell). من خلال البدء بملف XML، يمكنك استخدام كل خيار متوفر.
