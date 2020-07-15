---
title: مشاكل مع آلات على متن الطائرة
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6023"
- "9002913"
ms.openlocfilehash: 19b516dc21472e2c80a8b9046f802b329d15e4d6
ms.sourcegitcommit: 45c2aaeee58c0be466b76c7f0cd71e796d3c8f76
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 07/15/2020
ms.locfileid: "45141284"
---
# <a name="issues-with-onboarding-machines"></a><span data-ttu-id="8d8e8-102">مشاكل مع آلات على متن الطائرة</span><span class="sxs-lookup"><span data-stu-id="8d8e8-102">Issues with onboarding machines</span></span>

<span data-ttu-id="8d8e8-103">قد يكون لديك مشاكل مع أجهزة تشغيل إلى خدمة MDATP.</span><span class="sxs-lookup"><span data-stu-id="8d8e8-103">You might have issues with onboarding machines to MDATP service.</span></span> <span data-ttu-id="8d8e8-104">إذا كان يمكنك الوصول إلى جهاز المستخدم النهائي، اتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="8d8e8-104">If you can access the end-user machine, follow these steps:</span></span>

1. <span data-ttu-id="8d8e8-105">قم بتنزيل أداة تشخيص [محلل اتصال العميل.](https://aka.ms/mdatpanalyzer)</span><span class="sxs-lookup"><span data-stu-id="8d8e8-105">Download the [Client Connectivity Analyzer](https://aka.ms/mdatpanalyzer) diagnostic tool.</span></span>
2. <span data-ttu-id="8d8e8-106">استخراج وتشغيل MDATPAnalyzer.cmd.</span><span class="sxs-lookup"><span data-stu-id="8d8e8-106">Extract and run MDATPAnalyzer.cmd.</span></span>
3. <span data-ttu-id="8d8e8-107">حدد موقع سجل التشخيص في المجلد يسمى MDATPClientAnalyzerResult، نفس المجلد حيث يتم تحميل أداة محلل.</span><span class="sxs-lookup"><span data-stu-id="8d8e8-107">Locate the diagnostic log in the folder called MDATPClientAnalyzerResult, the same folder where the Analyzer tool is downloaded.</span></span>
4. <span data-ttu-id="8d8e8-108">راجع ملف السجل، MDATPClientAnalyzer.txt، للعثور على مشكلات الاتصال أو إعدادات وكيل الإنترنت.</span><span class="sxs-lookup"><span data-stu-id="8d8e8-108">Review the log file, MDATPClientAnalyzer.txt, to find connectivity or internet proxy settings issues.</span></span>