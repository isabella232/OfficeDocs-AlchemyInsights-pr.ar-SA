---
title: تغيير إعدادات EWS
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000752"
- "5653"
- "5760"
ms.openlocfilehash: 16916d5f16f763d87ce0d5ef830e741279c9f4df
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51818023"
---
# <a name="changing-ews-throttling-settings"></a><span data-ttu-id="9bbb4-102">تغيير إعدادات EWS</span><span class="sxs-lookup"><span data-stu-id="9bbb4-102">Changing EWS throttling settings</span></span>

<span data-ttu-id="9bbb4-103">الرجاء تشغيل الاختبار التلقائي الذي سيسمح لك بتعديل نهج EWS للتقييل طوال مدة الترحيل.</span><span class="sxs-lookup"><span data-stu-id="9bbb4-103">Please run our automated test which will allow you to modify the EWS throttling policy for the duration of your migration.</span></span> <span data-ttu-id="9bbb4-104">تجدر الإشارة إلى أنه حتى بعد تشغيل هذا، ستقتصر عمليات استيراد EWS على 150mb لكل 5 دقائق لكل علبة بريد؛ لتحقيق سرعات نقل ترحيل أعلى، يرجى ترحيل المزيد من المستخدمين بشكل متزامن.</span><span class="sxs-lookup"><span data-stu-id="9bbb4-104">Note that even after this is run, EWS imports will still be limited to 150mb per 5 minutes per mailbox; to achieve higher migration throughput speeds, please migrate more users concurrently.</span></span>

<span data-ttu-id="9bbb4-105">تجدر الإشارة إلى أن تغييرات نهج التحكم في EWS لا يكون لها أي تأثير على أنواع الترحيل التالية (باستخدام أدوات Microsoft): المختلط أو كلي/مرحلي (RPC/HTTP) أو IMAP أو G Suite أو المجلد العام أو خدمة استيراد PST.</span><span class="sxs-lookup"><span data-stu-id="9bbb4-105">Please note that EWS throttling policy changes have no effect on the following migration types (using Microsoft tools): Hybrid, Cutover/Staged (RPC/HTTP), IMAP, G Suite, Public Folder or PST Import Service.</span></span>