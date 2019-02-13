---
title: 1065 "الإهمال من البرنامج" الخارجي IP عنوان rangesMC146155
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 9/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: 2b4b2e2341f45e2d37713d72a2e0d34fa1a9a7cc
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/12/2019
ms.locfileid: "29934871"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>الإهمال التنظيمي نطاقات عناوين IP الصادرة

لقد اكتشفنا مشكلة محتملة مع المؤسسة الخاصة بك (إذا لم يتم تصحيحها بتاريخ 26 تشرين الأول/أكتوبر 2018) قد قطع تدفق البريد الداخلي أو وجهات خارجية. كما أبلغ عنها سابقا، لتبسيط إدارة نطاق عناوين IP، ونحن تقوم بالدمج نطاقات عناوين IP حماية Exchange عبر إنترنت (التنظيمي) التي يتم استخدامها لإرسال وتلقى البريد خارج Office 365. يشير تحليلنا إلى أن واحد أو أكثر من المصادر الخارجية البريد الإلكتروني أو الوجهات التي قمت بتكوينها في الروابط تدفق البريد لا يتم قبول الاتصالات من على IP عنوان نطاقات عرضها [هنا](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).
  
تعمل قبل 26 تشرين الأول/أكتوبر لضمان قبول هذه المصادر ووجهات الاتصالات ومن كافة [عناوين IP البرنامج نشر](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).
  
لمزيد من المعلومات حول هذا التغيير، الرجاء مراجعة وظائف مركز الرسائل [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155)أو [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)أو [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).
  
 **ملاحظة**: إذا استخدمت مسبقاً IP أو عنوان URL النشر عبر HTML و XML و RSS للتحديثات نقطة النهاية، كما يجب ترحيل لخدمات الويب الجديدة لهذه الأنواع من التحديثات بشكل تلقائي. لمزيد من المعلومات، راجع [Office 365 نقطة النهاية فئات وعنوان IP Office 365 وخدمه ويب URL](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).
  

