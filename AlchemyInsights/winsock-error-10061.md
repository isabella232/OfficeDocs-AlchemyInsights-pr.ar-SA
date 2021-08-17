---
title: الخطأ 1554 وينكوك 10061
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
ms.openlocfilehash: 7991f83a0b4791eaa7eb3246f7e61f781e4c7430931fbf920d7fd9e44c018d13
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54083217"
---
# <a name="winsock-error-10061"></a>خطأ وينكوك 10061

يعني رمز الخطأ هذا أنه لم تتمكن Microsoft من إنشاء مأخذ توصيل TCP (اتصال) مع المضيف الهدف. السبب المرجح لهذا الخطأ هو مشكلة في تكوين جدار الحماية. لإصلاح المشكلة، تحقق من هذه الإعدادات:

- التحقق من تكوين جدار الحماية الخاص بك باستخدام المعلومات في نطاقات عناوين [IP Microsoft 365 URL](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

- إذا كان الخطأ خاص Exchange Online Protection (EOP)، فمن المفترض أن يتم إعلامك مسبقا بتغيير في عناوين IP Exchange Online Protection [IP.](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)

- تحقق من أن موفر خدمة الإنترنت (ISP) لا يمنع المنفذ.

- تحقق من إعدادات الخادم الهدف والمضيف الذكي في الموصلات.

لاحظ أن Microsoft 365 لا يمنع الاتصالات *الواردة* بهذه الطريقة.
