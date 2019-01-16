---
title: خطأ Winsock 1554 10061
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 96a9cfd11941158ddf13655c74974e3eb800e570
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/15/2019
ms.locfileid: "28273131"
---
# <a name="winsock-error-10061"></a>خطأ Winsock 10061

رمز الخطأ هذا يعني أن Office 365 تعذر إنشاء مأخذ توصيل TCP (اتصال) مع المضيف الهدف. السبب المحتمل لهذا الخطأ مشكلة في تكوين جدار الحماية الخاص بك. لحل هذه المشكلة، تحقق من هذه الإعدادات:
  
- تحقق من تكوين جدار الحماية الخاص بك باستخدام المعلومات الموجودة في [Office 365 URLs ونطاقات عناوين IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)
    
- إذا كان الخطأ خاص إلى Exchange عبر إنترنت الحماية (البرنامج)، قد يجب أن تم مسبقاً إعلامك لتغيير [عناوين IP في حماية Exchange عبر إنترنت](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).
    
- تأكد من أن موفر خدمة إنترنت (ISP) لا يقوم بحظر المنفذ.
    
- تحقق من إعدادات الخادم المضيف والهدف الذكية في الموصلات.
    
لاحظ أن Office 365 لا منع الاتصالات *الواردة* على هذا النحو. 
  

