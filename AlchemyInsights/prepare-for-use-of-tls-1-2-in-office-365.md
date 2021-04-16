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

اعتباراً من 31 أكتوبر 2018، سيستمر Microsoft 365 في الانتقال إلى TLS 1.2. بدءا من 15 أكتوبر 2020، سيبدأ O365 في إهمال TLS 1.0 و1.1 عبر الخدمة. سيستمر طرح هذا التغيير على مدار الأسابيع والأشهر القليلة القادمة، ولكن يجب على العملاء افتراض عدم عمل مكالمات TLS 1.0/1.1 عند استخدام O365 بدءا من 15 أكتوبر 2020. كما تم الاتصال مسبقا (MC126199 في ديسمبر 2017، إن MC128929 في فبراير 2018 و MC186827 في يوليو 2019 و MC218794 في يوليو 2020)، نقوم بنقل كل خدماتنا عبر الإنترنت إلى 1.2+ أمان طبقة النقل لتوفير التشفير الأفضل في الفئة وضمان أن تكون خدمتنا أكثر أمانا بشكل افتراضي. لا يزال يمكن للعملاء اختيار الحصول على TLS 1.0/1.1 على خوادمهم ومواردهم، ولكن يجب أن يفترضوا أن TLS 1.2 أو أعلى فقط ستعمل عند التفاعل مع موارد O365.
  
لمعرفة المزيد حول هذه التغييرات، الرجاء الاطلاع [على هنا](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365?view=o365-worldwide) [وهنا](https://docs.microsoft.com/microsoft-365/compliance/tls-1.0-and-1.1-deprecation-for-office-365?view=o365-worldwide).

  