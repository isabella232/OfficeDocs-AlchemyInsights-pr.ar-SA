---
title: إهمال 1065 نطاقات عناوين IP الصادرة ل EOPMC146155
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: 214abc57a99c70a02a7d159441713e007f6ad980f67e373780d4ca297f69f764
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54031249"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>إهمال نطاقات عناوين IP الصادرة ل EOP

لقد اكتشفنا مشكلة محتملة في مؤسستك قد تكسر تدفق البريد إلى الوجهات المحلية أو الخارجية (إذا لم يتم تصحيحها بحلول 26 أكتوبر 2018). كما تم الاتصال مسبقا، لتبسيط إدارة نطاقات عناوين IP، نقوم بدمج نطاقات عناوين IP Exchange Online Protection (EOP) المستخدمة لإرسال البريد الإلكتروني وتلقيه خارج Microsoft 365. يشير تحليلنا إلى أن واحدة أو أكثر من مصادر البريد الإلكتروني الخارجية أو الوجهات التي قمت بتكوينها في موصلات تدفق البريد لا تقبل الاتصالات من نطاقات عناوين IP المعروضة [هنا](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

التصرف قبل 26 أكتوبر لضمان قبول هذه المصادر والوجهات للاتصالات من ونهاية عناوين [IP ل EOP المنشورة.](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)

لمزيد من المعلومات حول هذا التغيير، الرجاء الاطلاع على منشورات مركز الرسائل [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155)أو [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)أو [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).

**ملاحظة:** إذا سبق لك استخدام نشر عناوين IP أو URL عبر HTML وXML وRSS لتحديثات نقاط النهاية، يجب أيضا الترحيل إلى خدمات الويب الجديدة لأتمتة هذه الأنواع من التحديثات. لمزيد من المعلومات، راجع Microsoft 365 نقاط النهاية Microsoft 365 IP وخدمة [URL على الويب](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).
