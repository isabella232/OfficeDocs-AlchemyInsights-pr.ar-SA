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
ms.openlocfilehash: c0996e0cc923c13b7de3752ac6534026e8627c51
ms.sourcegitcommit: dcd1c76ced1a0cec27f4cf8d383593760c198424
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/18/2021
ms.locfileid: "59446678"
---
# <a name="dlp-might-need-a-custom-type"></a>قد تحتاج DLP إلى نوع مخصص

**هام**: خلال هذه الأوقات غير المسبوقة، نقوم باتخاذ الخطوات اللازمة لضمان توفر خدمات SharePoint Online و OneDrive بشكل كبير – الرجاء زيارة [تعديلات الميزات المؤقتة لـ SharePoint Online](https://aka.ms/ODSPAdjustments) للحصول على مزيد من المعلومات.

**قد تتطلب DLP نوع معلومات مخصص**

باستخدام نهج منع فقدان البيانات (DLP)، يمكنك تحديد البيانات الحساسة وحمايتها في مؤسستك. في بعض السيناريوهات، قد تحتاج إلى إنشاء نوع المعلومات الحساسة المخصص لحماية بيانات مؤسستك. لمزيد من المعلومات، راجع [التعرف على أنواع المعلومات الحساسة](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-learn-about) وتعريفات كيان نوع المعلومات [الحساسة](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).

لمزيد من المعلومات حول كيفية إنشاء أنواع المعلومات المخصصة الحساسة ونهجها، راجع: 

**تخصيص نوع معلومات حساسة مضمن**

إذا كان نوع المعلومات الحساسة المضمن يلبي احتياجاتك من خلال بعض التعديلات فقط، فشاهد تخصيص نوع معلومات [حساسة مضمن](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type). على سبيل المثال، يمكنك إضافة كلمات أساسية أو إزالتها، أو إضافة أدلة دعم أو إزالتها مثل تاريخ أو عنوان.

**إنشاء نوع معلومات حساسة مخصصة**

ولكن إذا كنت بحاجة إلى تحديد نوع مختلف من المعلومات الحساسة وحمايتها تماما، يمكنك إنشاء نوع معلومات حساسة مخصص في مركز التوافق في Microsoft 365. لمزيد من المعلومات، راجع [بدء استخدام أنواع المعلومات الحساسة المخصصة](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type).

**إنشاء نوع معلومات حساسة مخصصة في مركز & التوافق PowerShell**

وأخيرا، إذا لم توفر واجهة المستخدم كل الخيارات التي تحتاج إليها، يمكنك إنشاء نوع معلومات مخصص حساس في مركز التوافق & PowerShell. من خلال البدء بملف XML، يمكنك استخدام كل خيار متوفر. لمزيد من المعلومات، راجع [إنشاء نوع معلومات حساسة مخصصة باستخدام PowerShell](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell).

لاختبار النهج في وضع الاختبار أولا، [راجع](https://docs.microsoft.com/microsoft-365/compliance/dlp-learn-about-dlp#implement-policy-in-test-mode) تنفيذ النهج في وضع الاختبار وإنشاء نهج [DLP واختباره وضبطه.](https://docs.microsoft.com/microsoft-365/compliance/create-test-tune-dlp-policy) 