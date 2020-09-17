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
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a><span data-ttu-id="601df-102">اسئله حول كيفيه استخدام أداه نشر Office (ODT)</span><span class="sxs-lookup"><span data-stu-id="601df-102">Questions about how to use the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="601df-103">قم بتنزيل أداه نشر Office من [مركز التنزيل ل Microsoft](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="601df-103">Download the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
  
<span data-ttu-id="601df-104">بعد تنزيل الملف ، قم بتشغيل الملف القابل للتنفيذ والاستخراج الذاتي ، الذي يحتوي علي أداه نشر Office القابلة للتنفيذ (setup.exe) وملف تكوين نموذجي (configuration.xml).</span><span class="sxs-lookup"><span data-stu-id="601df-104">After downloading the file, run the self-extracting executable file, which contains the Office Deployment Tool executable (setup.exe) and a sample configuration file (configuration.xml).</span></span>
  
 <span data-ttu-id="601df-105">**لاستبعاد تطبيقات Microsoft 365 لمنتجات المؤسسة من أجهزه الكمبيوتر العميلة أو ازالتها:**</span><span class="sxs-lookup"><span data-stu-id="601df-105">**To exclude or remove Microsoft 365 Apps for enterprise products from client computers:**</span></span>
  
<span data-ttu-id="601df-106">عند تثبيت تطبيقات Microsoft 365 للمؤسسة ، يمكنك استبعاد منتجات معينه.</span><span class="sxs-lookup"><span data-stu-id="601df-106">When installing Microsoft 365 Apps for enterprise, you can exclude specific products.</span></span> <span data-ttu-id="601df-107">للقيام بذلك ، اتبع الخطوات المتعلقة بتثبيت Office مع ODT ، ولكن قم بتضمين عنصر اكسكلوديب في ملف التكوين.</span><span class="sxs-lookup"><span data-stu-id="601df-107">To do so, follow the steps for installing Office with the ODT, but include the ExcludeApp element in your configuration file.</span></span> <span data-ttu-id="601df-108">علي سبيل المثال ، يقوم ملف التكوين هذا بتثبيت كل تطبيقات Microsoft 365 لمنتجات enterprise باستثناء Publisher:</span><span class="sxs-lookup"><span data-stu-id="601df-108">For example, this configuration file installs all the Microsoft 365 Apps for enterprise products except Publisher:</span></span>
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[<span data-ttu-id="601df-109">نظره عامه حول أداه نشر Office</span><span class="sxs-lookup"><span data-stu-id="601df-109">Overview of the Office Deployment Tool</span></span>](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

