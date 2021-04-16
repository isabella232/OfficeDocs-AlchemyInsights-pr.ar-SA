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
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a><span data-ttu-id="6d5c9-102">أسئلة حول كيفية استخدام أداة نشر Office (ODT)</span><span class="sxs-lookup"><span data-stu-id="6d5c9-102">Questions about how to use the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="6d5c9-103">قم بتنزيل أداة نشر Office من [مركز التنزيل ل Microsoft](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="6d5c9-103">Download the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
  
<span data-ttu-id="6d5c9-104">بعد تنزيل الملف، قم بتشغيل الملف القابل للتنفيذ الذي يحتوي على أداة نشر Office القابلة للتنفيذ (setup.exe) وملف تكوين العينة (configuration.xml).</span><span class="sxs-lookup"><span data-stu-id="6d5c9-104">After downloading the file, run the self-extracting executable file, which contains the Office Deployment Tool executable (setup.exe) and a sample configuration file (configuration.xml).</span></span>
  
 <span data-ttu-id="6d5c9-105">**لاستبعاد تطبيقات Microsoft 365 لمنتجات المؤسسة أو إزالتها من أجهزة الكمبيوتر العميلة:**</span><span class="sxs-lookup"><span data-stu-id="6d5c9-105">**To exclude or remove Microsoft 365 Apps for enterprise products from client computers:**</span></span>
  
<span data-ttu-id="6d5c9-106">عند تثبيت تطبيقات Microsoft 365 للمؤسسات، يمكنك استبعاد منتجات معينة.</span><span class="sxs-lookup"><span data-stu-id="6d5c9-106">When installing Microsoft 365 Apps for enterprise, you can exclude specific products.</span></span> <span data-ttu-id="6d5c9-107">للقيام بذلك، اتبع الخطوات لتثبيت Office باستخدام ODT، ولكن قم بتضمين العنصر ExcludeApp في ملف التكوين.</span><span class="sxs-lookup"><span data-stu-id="6d5c9-107">To do so, follow the steps for installing Office with the ODT, but include the ExcludeApp element in your configuration file.</span></span> <span data-ttu-id="6d5c9-108">على سبيل المثال، يثبت ملف التكوين هذا جميع تطبيقات Microsoft 365 لمنتجات المؤسسات باستثناء Publisher:</span><span class="sxs-lookup"><span data-stu-id="6d5c9-108">For example, this configuration file installs all the Microsoft 365 Apps for enterprise products except Publisher:</span></span>
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[<span data-ttu-id="6d5c9-109">نظرة عامة على أداة نشر Office</span><span class="sxs-lookup"><span data-stu-id="6d5c9-109">Overview of the Office Deployment Tool</span></span>](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

