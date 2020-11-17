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
ms.openlocfilehash: c5b055989014b464d3136895702c8ea40e8eb701
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 11/17/2020
ms.locfileid: "49086143"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a><span data-ttu-id="ab986-102">اسئله حول كيفيه استخدام أداه نشر Office (ODT)</span><span class="sxs-lookup"><span data-stu-id="ab986-102">Questions about how to use the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="ab986-103">قم بتنزيل أداه نشر Office من [مركز التنزيل ل Microsoft](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="ab986-103">Download the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
  
<span data-ttu-id="ab986-104">بعد تنزيل الملف ، قم بتشغيل الملف القابل للتنفيذ والاستخراج الذاتي ، الذي يحتوي علي أداه نشر Office القابلة للتنفيذ (setupodt.exe) وملف تكوين نموذجي (configuration.xml).</span><span class="sxs-lookup"><span data-stu-id="ab986-104">After downloading the file, run the self-extracting executable file, which contains the Office Deployment Tool executable (setupodt.exe) and a sample configuration file (configuration.xml).</span></span>
  
 <span data-ttu-id="ab986-105">**لاستبعاد تطبيقات Microsoft 365 لمنتجات المؤسسة من أجهزه الكمبيوتر العميلة أو ازالتها:**</span><span class="sxs-lookup"><span data-stu-id="ab986-105">**To exclude or remove Microsoft 365 Apps for enterprise products from client computers:**</span></span>
  
<span data-ttu-id="ab986-106">عند تثبيت تطبيقات Microsoft 365 للمؤسسة ، يمكنك استبعاد منتجات معينه.</span><span class="sxs-lookup"><span data-stu-id="ab986-106">When installing Microsoft 365 Apps for enterprise, you can exclude specific products.</span></span> <span data-ttu-id="ab986-107">للقيام بذلك ، اتبع الخطوات المتعلقة بتثبيت Office مع ODT ، ولكن قم بتضمين عنصر اكسكلوديب في ملف التكوين.</span><span class="sxs-lookup"><span data-stu-id="ab986-107">To do so, follow the steps for installing Office with the ODT, but include the ExcludeApp element in your configuration file.</span></span> <span data-ttu-id="ab986-108">علي سبيل المثال ، يقوم ملف التكوين هذا بتثبيت كل تطبيقات Microsoft 365 لمنتجات enterprise باستثناء Publisher:</span><span class="sxs-lookup"><span data-stu-id="ab986-108">For example, this configuration file installs all the Microsoft 365 Apps for enterprise products except Publisher:</span></span>
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[<span data-ttu-id="ab986-109">نظره عامه حول أداه نشر Office</span><span class="sxs-lookup"><span data-stu-id="ab986-109">Overview of the Office Deployment Tool</span></span>](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

