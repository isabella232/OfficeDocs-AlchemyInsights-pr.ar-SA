---
title: 1554 خطا Winsock 10061
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 4f8007bd8ccb4666260c75fdca15dd0b14eb4e96
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47698849"
---
# <a name="winsock-error-10061"></a>خطا Winsock 10061

يشير رمز الخطا هذا إلى تعذر علي Microsoft إنشاء ماخذ توصيل TCP (اتصال) مع المضيف الهدف. السبب المحتمل هو وجود مشكله في تكوين جدار الحماية. لإصلاح المشكلة ، تحقق من الإعدادات التالية:

- التحقق من تكوين جدار الحماية باستخدام المعلومات الموجودة في [نطاقات عناوين url و Microsoft 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

- إذا كان الخطا خاصا ب Exchange Online Protection (EOP) ، فمن المفترض ان تكون قد تم اعلامك مسبقا بتغيير في [عناوين IP ل Exchange Online Protection](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

- تاكد من ان موفر خدمه الإنترنت (ISP) لا يقوم بحظر المنفذ.

- تحقق من إعدادات خادم المضيف الذكي والهدف في الموصلات.

لاحظ ان Microsoft 365 لا يقوم بحظر الاتصالات *الواردة* بهذه الطريقة.
