---
title: اسئله حول كيفيه استخدام أداه نشر Office (ODT)
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/26/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: 604fc200517316de6e0194bd64e6eb3039cfa61b
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/18/2019
ms.locfileid: "36553527"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>اسئله حول كيفيه استخدام أداه نشر Office (ODT)

قم بتنزيل "أداه نشر Office" من " [مركز التنزيل ل Microsoft](http://go.microsoft.com/fwlink/p/?LinkID=626065)".
  
بعد تحميل الملف ، تشغيل الملف القابل للتنفيذ الاستخراج الذاتي الذي يحتوي علي أداه نشر Office القابل للتنفيذ (setup.exe) وملف تكوين نموذج (تكوين .xml).
  
 **لاستبعاد أو أزاله منتجات Office 365 ProPlus من أجهزه الكمبيوتر العميلة:**
  
عند تثبيت Office 365 ProPlus ، يمكنك استبعاد منتجات معينه. للقيام بذلك ، اتبع الخطوات التالية لتثبيت Office مع ODT ، ولكن تضمين العنصر الحصري في ملف التكوين الخاص بك. علي سبيل المثال ، يقوم ملف التكوين هذا بتثبيت كافة منتجات Office 365 ProPlus باستثناء Publisher:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[نظره عامه حول أداه نشر Office](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)
  

