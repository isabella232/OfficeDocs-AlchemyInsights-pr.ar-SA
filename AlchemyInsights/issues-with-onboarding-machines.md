---
title: مشاكل في أجهزة الboard إلى Microsoft Defender لنقاط النهاية
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
ms.openlocfilehash: 7ccec69f8ab43f277978176519a7f8f8df443846
ms.sourcegitcommit: 1d73771d147325cfd8578e6816becd8331913890
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/19/2021
ms.locfileid: "50901554"
---
# <a name="issues-with-onboarding-machines-to-microsoft-defender-for-endpoints"></a><span data-ttu-id="cb1be-102">مشاكل في أجهزة الboard إلى Microsoft Defender لنقاط النهاية</span><span class="sxs-lookup"><span data-stu-id="cb1be-102">Issues with onboarding machines to Microsoft Defender for Endpoints</span></span>

<span data-ttu-id="cb1be-103">قد تكون لديك مشاكل في أجهزة التكهين لخدمة MDE.</span><span class="sxs-lookup"><span data-stu-id="cb1be-103">You might have issues with onboarding machines to MDE service.</span></span> <span data-ttu-id="cb1be-104">إذا كان بإمكانك الوصول إلى جهاز المستخدم النهائي، فاتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="cb1be-104">If you can access the end-user machine, follow these steps:</span></span>

1. <span data-ttu-id="cb1be-105">قم بتنزيل أحدث إصدار معاينة من أداة [تشخيص MDE Client Analyzer.](https://aka.ms/betamdeanalyzer)</span><span class="sxs-lookup"><span data-stu-id="cb1be-105">Download the latest preview version of the [MDE Client Analyzer](https://aka.ms/betamdeanalyzer) diagnostic tool.</span></span>
2. <span data-ttu-id="cb1be-106">انقر بزر **الماوس الأيمن فوق MDEClientAnalyzer.cmd** وحدد "تشغيل كمسؤول".</span><span class="sxs-lookup"><span data-stu-id="cb1be-106">Right click **MDEClientAnalyzer.cmd** and select ‘Run as administrator’.</span></span>
3. <span data-ttu-id="cb1be-107">اتبع أي إرشادات تم اقتراحها في **MDEClientAnalyzer.htm**.</span><span class="sxs-lookup"><span data-stu-id="cb1be-107">Follow any guidance suggested in **MDEClientAnalyzer.htm**.</span></span>
4. <span data-ttu-id="cb1be-108">لمزيد من السجلات المطوبة، راجع المجلد الفرعي الذي تم إنشاؤه المسمى **MDEClientAnalyzerResult**.</span><span class="sxs-lookup"><span data-stu-id="cb1be-108">For more verbose logs, review the created sub-folder named **MDEClientAnalyzerResult**.</span></span>
5. <span data-ttu-id="cb1be-109">إذا كانت هناك حاجة إلى إرشادات إضافية، فاتصل بدعم نقطة النهاية [ل Microsoft Defender](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/contact-support) واوفر الملف الناتج MDEClientAnalyzerResult.zip لتحليله.</span><span class="sxs-lookup"><span data-stu-id="cb1be-109">If additional guidance is needed, contact [Microsoft Defender for Endpoint support](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/contact-support) and provide the resulting MDEClientAnalyzerResult.zip file for analysis.</span></span>
