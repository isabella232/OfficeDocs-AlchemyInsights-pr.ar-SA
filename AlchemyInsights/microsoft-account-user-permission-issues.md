---
title: إنشاء واستخدام علبة بريد المشتركة
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 81bf8082198de1c44037291f23c434d06a77f02a
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/07/2019
ms.locfileid: "34762388"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>حل المشكلة-المستخدم غير موجود في الدليل

إذا كان المستخدمون تتلقى خطأ رسالة "لا يمكن العثور على المستخدم" في الدليل. الرجاء المحاولة مرة أخرى حيث "نوع المشكلة" غير المستخدم في الدليل.

يمكن إكمال الخطوات التالية استكشاف المشكلة وإصلاحها.

- تأكد من الحساب الذي قبلت دعوة البريد الإلكتروني هو نفسه الحساب الذي يتم استخدامه لتسجيل الدخول لاحقاً. تأكد من أن المستخدم يستخدم نفس الحساب لقبول الدعوة وتسجيل الدخول إلى الموقع. 

لمزيد من المعلومات، راجع [كيفية إدارة الأسماء المستعارة لحساب Microsoft</a> لإدارة تسجيل الدخول Office 365](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases). 

- استعرض للوصول إلى كل المواقع التي يتلقى المستخدم الخطأ. 

إضافة "/_layouts/15/people.aspx/membershipgroupid=0" (داخل علامات اقتباس المزدوجة) إلى نهاية url الخاص بالموقع. 

على سبيل المثال: https://_lT _"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.

- حدد المستخدم من القائمة.

- انقر فوق **إزالة أذونات المستخدم** من "الشريط". 
-  إضافة المستخدم مرة أخرى وإعادة إرسال الدعوة إلى المستخدم.

