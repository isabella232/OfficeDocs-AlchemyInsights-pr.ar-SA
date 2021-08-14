---
title: أسئلة حول كيفية استخدام أداة Office (ODT)
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
ms.openlocfilehash: d38866647c7bf286b5b5b21e7fdcc94af72ea1850bc40391af077aa230b8b4fd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53959670"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>أسئلة حول كيفية استخدام أداة Office (ODT)

قم بتنزيل Office النشر من [مركز تنزيل Microsoft](https://go.microsoft.com/fwlink/p/?LinkID=626065).
  
بعد تنزيل الملف، قم بتشغيل ملف قابل للتنفيذ لاستخراجه ذاتيا، الذي يحتوي على أداة النشر Office القابلة للتنفيذ (setup.exe) وملف تكوين العينة (configuration.xml).
  
 **لاستبعاد منتجات Microsoft 365 Apps for enterprise من أجهزة الكمبيوتر العميلة أو إزالتها:**
  
عند تثبيت Microsoft 365 Apps for enterprise، يمكنك استبعاد منتجات معينة. للقيام بذلك، اتبع الخطوات اللازمة لتثبيت Office ODT، ولكن قم بتضمين العنصر ExcludeApp في ملف التكوين. على سبيل المثال، يثبت ملف التكوين هذا جميع Microsoft 365 Apps for enterprise باستثناء Publisher:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[نظرة عامة على أداة Office النشر](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

