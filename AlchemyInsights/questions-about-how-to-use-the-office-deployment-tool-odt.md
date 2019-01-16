---
title: أسئلة حول كيفية استخدام أداة نشر Office (ODT)
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/26/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: c16b7ac7d79794307fa33ed1039305ed5b842cf6
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/15/2019
ms.locfileid: "28272828"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>أسئلة حول كيفية استخدام أداة نشر Office (ODT)

تنزيل أداة نشر Office من ["مركز تحميل microsoft"](http://go.microsoft.com/fwlink/p/?LinkID=626065).
  
بعد تنزيل الملف، تشغيل الملف القابل للتنفيذ يتم استخراجه ذاتيا، الذي يحتوي على Office نشر الأداة القابل للتنفيذ (setup.exe) ونموذج لملف تكوين (configuration.xml).
  
 **لاستبعاد أو إزالة منتجات Office 365 ProPlus من أجهزة الكمبيوتر العميلة:**
  
عند تثبيت Office 365 ProPlus، يمكنك استبعاد منتجات معينة. للقيام بذلك، اتبع الخطوات لتثبيت Office مع ODT، بل تتضمن عنصر اكسكلوديب في ملف التكوين الخاص بك. على سبيل المثال، ملف التكوين هذا بتثبيت كافة منتجات Office 365 ProPlus استثناء الناشر:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[نظرة عامة حول أداة نشر Office](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)
  

