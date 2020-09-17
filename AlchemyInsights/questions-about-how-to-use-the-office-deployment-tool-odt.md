---
title: اسئله حول كيفيه استخدام أداه نشر Office (ODT)
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: e9f7581fd21cf5ca2d712038c4b73b67d08f3a76
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47774878"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>اسئله حول كيفيه استخدام أداه نشر Office (ODT)

قم بتنزيل أداه نشر Office من [مركز التنزيل ل Microsoft](https://go.microsoft.com/fwlink/p/?LinkID=626065).
  
بعد تنزيل الملف ، قم بتشغيل الملف القابل للتنفيذ والاستخراج الذاتي ، الذي يحتوي علي أداه نشر Office القابلة للتنفيذ (setup.exe) وملف تكوين نموذجي (configuration.xml).
  
 **لاستبعاد تطبيقات Microsoft 365 لمنتجات المؤسسة من أجهزه الكمبيوتر العميلة أو ازالتها:**
  
عند تثبيت تطبيقات Microsoft 365 للمؤسسة ، يمكنك استبعاد منتجات معينه. للقيام بذلك ، اتبع الخطوات المتعلقة بتثبيت Office مع ODT ، ولكن قم بتضمين عنصر اكسكلوديب في ملف التكوين. علي سبيل المثال ، يقوم ملف التكوين هذا بتثبيت كل تطبيقات Microsoft 365 لمنتجات enterprise باستثناء Publisher:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[نظره عامه حول أداه نشر Office](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

