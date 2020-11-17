---
title: التحضير لاستخدام أمان طبقة النقل TLS 1.2 في Microsoft 365
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Critical
ms.custom:
- "1266"
- "1600052"
ms.assetid: d5c84f5c-a3ca-4abd-8633-7e9ff01328a9
ms.openlocfilehash: 1ec40ba36c69296298e24dca64a873d53682833a
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 11/17/2020
ms.locfileid: "49085891"
---
# <a name="prepare-for-use-of-tls-12-in-microsoft-365"></a>التحضير لاستخدام أمان طبقة النقل TLS 1.2 في Microsoft 365

اعتباراً من 31 أكتوبر 2018، سيستمر Microsoft 365 في الانتقال إلى TLS 1.2. بدءا من 15 أكتوبر 2020 ، O365 سيبدا الإهمال الخاص ب TLS 1.0 و 1.1 عبر الخدمة. ستستمر عمليه تقديم هذا التغيير في الأسابيع القليلة والأشهر القادمة ، ولكن يجب ان يفترض العملاء عدم عمل مكالمات TLS 1.0/1.1 عند التعامل مع O365 بدءا من الأول من أكتوبر ، 2020. بمجرد ان يتم الاتصال مسبقا (MC126199 في ديسمبر 2017 ، MC128929 في فبراير 2018 ، MC186827 في يوليو 2019 ، و MC218794 في يوليو 2020) ، فاننا نقوم بنقل كل خدماتنا الموجودة عبر الإنترنت إلى أمان طبقه النقل (TLS) 1.2 + لتوفير التشفير الأفضل للفئة ، ولضمان أمان خدمتنا بشكل افتراضي. لا يزال بإمكان العملاء اختيار الحصول علي الإصدارين TLS 1.0/1.1 علي خوادمهم ومواردهم ، ولكن من المفترض ان يفترض عمل TLS 1.2 أو ما بعده فقط عند التفاعل مع موارد O365.
  
للحصول علي مزيد من المعلومات حول هذه التغييرات ، الرجاء الاطلاع علي [هنا](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365?view=o365-worldwide) [وهنا](https://docs.microsoft.com/microsoft-365/compliance/tls-1.0-and-1.1-deprecation-for-office-365?view=o365-worldwide).

  