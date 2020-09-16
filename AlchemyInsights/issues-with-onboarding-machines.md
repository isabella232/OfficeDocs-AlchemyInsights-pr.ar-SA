---
title: المشاكل المتعلقة باجهزه إلحاق
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6023"
- "9002913"
ms.openlocfilehash: c3203ed68eb19d5f6d75eb2269094bb0422b14cc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47676869"
---
# <a name="issues-with-onboarding-machines"></a><span data-ttu-id="87cd7-102">المشاكل المتعلقة باجهزه إلحاق</span><span class="sxs-lookup"><span data-stu-id="87cd7-102">Issues with onboarding machines</span></span>

<span data-ttu-id="87cd7-103">قد تواجه مشاكل تتعلق بإلحاق الاجهزه بخدمه مداتب.</span><span class="sxs-lookup"><span data-stu-id="87cd7-103">You might have issues with onboarding machines to MDATP service.</span></span> <span data-ttu-id="87cd7-104">إذا كان بإمكانك الوصول إلى جهاز المستخدم النهائي ، فاتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="87cd7-104">If you can access the end-user machine, follow these steps:</span></span>

1. <span data-ttu-id="87cd7-105">قم بتنزيل أداه تشخيص " [محلل اتصالات العملاء](https://aka.ms/mdatpanalyzer) ".</span><span class="sxs-lookup"><span data-stu-id="87cd7-105">Download the [Client Connectivity Analyzer](https://aka.ms/mdatpanalyzer) diagnostic tool.</span></span>
2. <span data-ttu-id="87cd7-106">استخراج وتشغيل مداتباناليزير.</span><span class="sxs-lookup"><span data-stu-id="87cd7-106">Extract and run MDATPAnalyzer.cmd.</span></span>
3. <span data-ttu-id="87cd7-107">حدد موقع السجل التشخيصي في المجلد الذي يسمي مداتبكلينتاناليزيريسولت ، والمجلد نفسه الذي يتم فيه تنزيل أداه المحلل.</span><span class="sxs-lookup"><span data-stu-id="87cd7-107">Locate the diagnostic log in the folder called MDATPClientAnalyzerResult, the same folder where the Analyzer tool is downloaded.</span></span>
4. <span data-ttu-id="87cd7-108">راجع ملف السجل ، MDATPClientAnalyzer.txt ، للبحث عن مشاكل تتعلق بإعدادات وكيل الإنترنت أو الاتصال به.</span><span class="sxs-lookup"><span data-stu-id="87cd7-108">Review the log file, MDATPClientAnalyzer.txt, to find connectivity or internet proxy settings issues.</span></span>