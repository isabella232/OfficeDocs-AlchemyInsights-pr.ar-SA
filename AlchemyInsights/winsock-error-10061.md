---
title: 1554 Winsock خطأ 10061
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: e8f62d97efc937518ef766b45e1747e83b7f99c3
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766156"
---
# <a name="winsock-error-10061"></a>Winsock خطأ 10061

رمز الخطأ هذا يعني أن Microsoft لم تتمكن من إنشاء مأخذ توصيل TCP (اتصال) مع المضيف الهدف. السبب الأكثر احتمالاً لهذا الخطأ هو مشكلة في تكوين جدار الحماية الخاص بك. لإصلاح المشكلة، تحقق من هذه الإعدادات:

- التحقق من تكوين جدار الحماية الخاص بك مع المعلومات الموجودة في [عناوين URL Microsoft 365 ونطاقات عناوين IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

- إذا كان الخطأ خاصًا بـ Exchange Online Protection (EOP)، فيجب أن يكون قد تم إعلامك مسبقًا بتغيير [عناوين IP الخاصة بحماية Exchange عبر الإنترنت](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

- تحقق من أن موفر خدمة الإنترنت (ISP) لا يقوم بحظر المنفذ.

- تحقق من إعدادات المضيف والخادم المستهدف الذكية في الموصلات.

لاحظ أن Microsoft 365 لا يمنع الاتصالات *الواردة* بهذه الطريقة.
