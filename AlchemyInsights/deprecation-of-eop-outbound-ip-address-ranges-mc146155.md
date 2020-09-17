---
title: 1065 إهمال عناوين IP الصادرة ل EOP rangesMC146155
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
ms.openlocfilehash: afd725668f906339f4b7d769bb67a4d2ee5a6ac6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806782"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>نطاقات عناوين IP الصادرة ل EOP

لقد اكتشفنا مشكله محتمله في مؤسستك (إذا لم يتم تصحيحها بواسطة شهر أكتوبر 26th 2018) قد تقطع تدفق البريد إلى الوجات المحلية أو الخارجية. بمجرد ان يتم الاتصال مسبقا ، لتبسيط أداره نطاق عناوين IP ، سنقوم بدمج نطاقات عناوين IP ل Exchange Online Protection (EOP) التي يتم استخدامها لإرسال البريد الكتروني وتلقيه خارج Microsoft 365. يشير التحليل الخاص بنا إلى ان واحد أو أكثر من مصادر البريد الكتروني الخارجية أو الوجات التي قمت بتكوينها في موصلات تدفق البريد لا تقبل الاتصالات من نطاقات عناوين IP التي تظهر [هنا](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

Act قبل أكتوبر 26th تاكد من ان هذه المصادر والوجات ستقبل الاتصالات بكل [عناوين IP المنشورة](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)والتي تم نشرها.

للحصول علي مزيد من المعلومات حول هذا التغيير ، يرجى مراجعه نشرات مركز الرسائل [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155)أو [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)أو [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).

**ملاحظه**: إذا قمت مسبقا باستخدام IP أو URL للنشر عبر HTML و XML و RSS لتحديثات نقاط النهاية ، فيجب أيضا الترحيل إلى خدمات الويب الجديدة لاتمته أنواع التحديثات هذه. لمزيد من المعلومات ، راجع [فئات نقاط النهاية ل microsoft 365 وعنوان IP ل microsoft 365 وخدمه ويب URL](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).
