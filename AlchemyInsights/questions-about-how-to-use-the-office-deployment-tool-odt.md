---
title: أسئلة حول كيفية استخدام أداة نشر Office (ODT)
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: 96d3f70f554f71c43d6458ec8debc099cd9fb040
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43698045"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>أسئلة حول كيفية استخدام أداة نشر Office (ODT)

تحميل أداة نشر Office من [مركز تنزيل Microsoft](https://go.microsoft.com/fwlink/p/?LinkID=626065).
  
بعد تنزيل الملف، قم بتشغيل الملف القابل للتنفيذ ذاتي الاستخراج، والذي يحتوي على أداة نشر Office القابلة للتنفيذ (setup.exe) وملف تكوين عينة (configuration.xml).
  
 **لاستبعاد تطبيقات Microsoft 365 لمنتجات المؤسسات من أجهزة الكمبيوتر العميلة أو إزالتها:**
  
عند تثبيت تطبيقات Microsoft 365 للمؤسسات، يمكنك استبعاد منتجات معينة. للقيام بذلك، اتبع الخطوات لتثبيت Office مع ODT، ولكن قم بتضمين عنصر ExcludApp في ملف التكوين الخاص بك. على سبيل المثال، يعمل ملف التكوين هذا على تثبيت كافة تطبيقات Microsoft 365 لمنتجات المؤسسات باستثناء Publisher:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[نظرة عامة على أداة نشر Office](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)
  

