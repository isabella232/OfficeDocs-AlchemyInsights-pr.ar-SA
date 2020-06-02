---
title: قد يحتاج DLP إلى نوع مخصص
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 1ec8959a479f1a8f7bfcffb55f440e8c4ab435fb
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507501"
---
# <a name="dlp-might-need-a-custom-type"></a>قد يحتاج DLP إلى نوع مخصص

**هام**: خلال هذه الأوقات غير المسبوقة، نقوم باتخاذ الخطوات اللازمة لضمان توفر خدمات SharePoint Online و OneDrive بشكل كبير – الرجاء زيارة [تعديلات الميزات المؤقتة لـ SharePoint Online](https://aka.ms/ODSPAdjustments) للحصول على مزيد من المعلومات.

**قد يتطلب DLP نوع معلومات مخصصة**

باستخدام سياسة منع فقدان البيانات (DLP) ، يمكنك تحديد البيانات الحساسة وحمايتها في مؤسستك. في بعض السيناريوهات، قد تحتاج إلى إنشاء نوع معلومات حساسة **مخصصة** لحماية بيانات مؤسستك.

على سبيل المثال، قد تحتاج مؤسستك إلى تحديد وحماية هوية الموظفين أو البيانات الأخرى بتنسيق معين لمؤسستك. إذا كان الأمر كذلك، راجع المقالات التالية لمزيد من المعلومات.
  
 **تخصيص نوع معلومات حساسة مدمج**
  
إذا كان نوع المعلومات الحساسة المدمج يلبي احتياجاتك مع بعض التعديلات فقط، يمكنك [تخصيص نوع معلومات حساسة مضمنة.](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type) على سبيل المثال، يمكنك إضافة كلمات رئيسية أو إزالتها، أو إضافة أو إزالة أدلة داعمة مثل تاريخ أو عنوان.
  
 **إنشاء نوع معلومات حساسة مخصصة**
  
ولكن إذا كنت بحاجة إلى تحديد وحماية نوع مختلف من المعلومات الحساسة تمامًا، يمكنك [إنشاء نوع معلومات حساسة مخصصة](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) في واجهة المستخدم لمركز التوافق & الأمان.
  
**إنشاء نوع معلومات حساسة مخصصة في مركز التوافق & الأمان PowerShell**

أخيرًا، إذا لم توفر واجهة المستخدم جميع الخيارات التي تحتاجها، يمكنك [إنشاء نوع معلومات حساسة مخصصة في مركز الأمان & الامتثال PowerShell](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell). من خلال البدء بملف XML، يمكنك استخدام كل خيار متاح.
