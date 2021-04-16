---
title: أسئلة حول كيفية استخدام أداة نشر Office (ODT)
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: 20e0b6aa3c298ee0a4291c3da6ae46978177e81f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51790319"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>أسئلة حول كيفية استخدام أداة نشر Office (ODT)

قم بتنزيل أداة نشر Office من [مركز التنزيل ل Microsoft](https://go.microsoft.com/fwlink/p/?LinkID=626065).
  
بعد تنزيل الملف، قم بتشغيل الملف القابل للتنفيذ الذي يحتوي على أداة نشر Office القابلة للتنفيذ (setup.exe) وملف تكوين العينة (configuration.xml).
  
 **لاستبعاد تطبيقات Microsoft 365 لمنتجات المؤسسة أو إزالتها من أجهزة الكمبيوتر العميلة:**
  
عند تثبيت تطبيقات Microsoft 365 للمؤسسات، يمكنك استبعاد منتجات معينة. للقيام بذلك، اتبع الخطوات لتثبيت Office باستخدام ODT، ولكن قم بتضمين العنصر ExcludeApp في ملف التكوين. على سبيل المثال، يثبت ملف التكوين هذا جميع تطبيقات Microsoft 365 لمنتجات المؤسسات باستثناء Publisher:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[نظرة عامة على أداة نشر Office](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

