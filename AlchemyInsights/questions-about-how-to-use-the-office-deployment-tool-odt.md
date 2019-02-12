---
title: أسئلة حول كيفية استخدام أداة نشر Office (ODT)
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/26/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: e91d40f872dd401ee210ac05eb39d64b6fb88027
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/12/2019
ms.locfileid: "29925331"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a><span data-ttu-id="6375e-102">أسئلة حول كيفية استخدام أداة نشر Office (ODT)</span><span class="sxs-lookup"><span data-stu-id="6375e-102">Questions about how to use the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="6375e-103">تنزيل أداة نشر Office من ["مركز تحميل microsoft"](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="6375e-103">Download the Office Deployment Tool from the [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
  
<span data-ttu-id="6375e-104">بعد تنزيل الملف، تشغيل الملف القابل للتنفيذ يتم استخراجه ذاتيا، الذي يحتوي على Office نشر الأداة القابل للتنفيذ (setup.exe) ونموذج لملف تكوين (configuration.xml).</span><span class="sxs-lookup"><span data-stu-id="6375e-104">After downloading the file, run the self-extracting executable file, which contains the Office Deployment Tool executable (setup.exe) and a sample configuration file (configuration.xml).</span></span>
  
 <span data-ttu-id="6375e-105">**لاستبعاد أو إزالة منتجات Office 365 ProPlus من أجهزة الكمبيوتر العميلة:**</span><span class="sxs-lookup"><span data-stu-id="6375e-105">**To exclude or remove Office 365 ProPlus products from client computers:**</span></span>
  
<span data-ttu-id="6375e-p101">عند تثبيت Office 365 ProPlus، يمكنك استبعاد منتجات معينة. للقيام بذلك، اتبع الخطوات لتثبيت Office مع ODT، بل تتضمن عنصر اكسكلوديب في ملف التكوين الخاص بك. على سبيل المثال، ملف التكوين هذا بتثبيت كافة منتجات Office 365 ProPlus استثناء الناشر:</span><span class="sxs-lookup"><span data-stu-id="6375e-p101">When installing Office 365 ProPlus, you can exclude specific products. To do so, follow the steps for installing Office with the ODT, but include the ExcludeApp element in your configuration file. For example, this configuration file installs all the Office 365 ProPlus products except Publisher:</span></span>
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[<span data-ttu-id="6375e-109">نظرة عامة حول أداة نشر Office</span><span class="sxs-lookup"><span data-stu-id="6375e-109">Overview of the Office Deployment Tool</span></span>](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)
  

