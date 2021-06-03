---
title: تشخيص لتمكين المصادقة الأساسية لبروتوكولات Exchange Online الأساسية
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/27/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11392"
- "9006699"
ms.openlocfilehash: 8952aba3dc6b5abcf56776d81eddd9b50db33c7f
ms.sourcegitcommit: d3a739b75d521837660ce151190a7e232e4eeadb
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/27/2021
ms.locfileid: "52731236"
---
# <a name="diagnostic-to-enable-basic-authentication-for-exchange-online-protocols"></a><span data-ttu-id="bdf17-102">تشخيص لتمكين المصادقة الأساسية لبروتوكولات Exchange Online الأساسية</span><span class="sxs-lookup"><span data-stu-id="bdf17-102">Diagnostic to enable Basic authentication for Exchange Online protocols</span></span>

<span data-ttu-id="bdf17-103">باستخدام هذا التشخيص، يمكنك تمكين المصادقة الأساسية لبروتوكولات Exchange Online مثل POP3 و IMAP4 و Exchange ActiveSync و Exchange Web Services و دفتر العنوان غير المتصل و MAPI و RPC و Remote PowerShell، والتي ربما قامت Microsoft بتعطيلها مؤخرا لم المؤسسة.</span><span class="sxs-lookup"><span data-stu-id="bdf17-103">By using this diagnostic, you can enable Basic authentication for Exchange Online protocols such as POP3, IMAP4, Exchange ActiveSync, Exchange Web Services, Offline Address Book, MAPI, RPC and Remote PowerShell, which Microsoft might have disabled recently for your organization.</span></span> 

<span data-ttu-id="bdf17-104">نحن نرسل اتصالات مباشرة عبر مركز الرسائل لنعلم المستأجرين بمكان جاهزيتهم إيقاف تشغيل المصادقة الأساسية في بيئتهم بسبب عدم الاستخدام، مما سيساعد في حماية بيئتهم من مخاطر الأمان ذات الصلة.</span><span class="sxs-lookup"><span data-stu-id="bdf17-104">We are sending direct communications through Message Center to let tenants know where they're ready to turn off Basic authentication in their environment due to no use, which will help protect their environments from related security risks.</span></span>