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
# <a name="diagnostic-to-enable-basic-authentication-for-exchange-online-protocols"></a>تشخيص لتمكين المصادقة الأساسية لبروتوكولات Exchange Online الأساسية

باستخدام هذا التشخيص، يمكنك تمكين المصادقة الأساسية لبروتوكولات Exchange Online مثل POP3 و IMAP4 و Exchange ActiveSync و Exchange Web Services و دفتر العنوان غير المتصل و MAPI و RPC و Remote PowerShell، والتي ربما قامت Microsoft بتعطيلها مؤخرا لم المؤسسة. 

نحن نرسل اتصالات مباشرة عبر مركز الرسائل لنعلم المستأجرين بمكان جاهزيتهم إيقاف تشغيل المصادقة الأساسية في بيئتهم بسبب عدم الاستخدام، مما سيساعد في حماية بيئتهم من مخاطر الأمان ذات الصلة.