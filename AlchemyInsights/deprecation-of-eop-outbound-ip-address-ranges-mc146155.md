---
title: 1065 الإهمال من EOP الصادرة عنوان IP rangesMC146155
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: f4854c32d970d84f3a0664a9e384dc6e3cd0bfa7
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704584"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>إهمال نطاقات عنوان IP الصادرة EOP

لقد اكتشفنا مشكلة محتملة مع مؤسستك قد تكسر تدفق البريد إلى وجهاتك الداخلية أو الخارجية (إذا لم يتم تصحيحها بحلول 26 أكتوبر 2018). كما تم إرساله مسبقًا ، لتبسيط إدارة نطاق عنوان IP ، نقوم بدمج نطاقات عنوان IP لحماية Exchange عبر الإنترنت (EOP) المستخدمة لإرسال واستقبال البريد الإلكتروني خارج Microsoft 365. يشير تحليلنا إلى أن واحدًا أو أكثر من مصادر البريد الإلكتروني الخارجية أو الوجهات التي قمت بتكوينها في موصلات تدفق البريد لا تقبل الاتصالات من نطاقات عنوان IP الموضحة [هنا](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

العمل قبل 26 أكتوبر لضمان قبول هذه المصادر والوجهات الاتصالات من وإلى جميع [عناوين IP EOP المنشورة](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

لمزيد من المعلومات حول هذا التغيير، يرجى الاطلاع على منشورات مركز الرسائل [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155)أو [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)أو [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).

**ملاحظة:** إذا كنت تستخدم مسبقاً نشر IP أو URL عبر HTML و XML و RSS لتحديثات نقطة النهاية، فيجب عليك أيضًا الترحيل إلى خدمات الويب الجديدة لأتمتة هذه الأنواع من التحديثات. لمزيد من المعلومات، راجع [فئات نقطة نهاية Microsoft 365 وعنوان IP Microsoft 365 وخدمة ويب URL](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).
