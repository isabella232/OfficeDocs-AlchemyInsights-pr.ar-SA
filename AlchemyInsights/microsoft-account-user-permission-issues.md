---
title: استكشاف أخطاء المشكلة-لم يتم العثور علي المستخدم في الدليل
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 0f1e427801107109e31486a4d300f53084880caf
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/15/2019
ms.locfileid: "40054797"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>استكشاف أخطاء المشكلة-لم يتم العثور علي المستخدم في الدليل

إذا كان المستخدمون يتلقون رسالة خطا "لا يمكن العثور علي المستخدم" في الدليل ، الرجاء المحاولة مره أخرى حيث "نوع المشكلة" المستخدم غير موجود في الدليل.

يمكن إكمال الخطوات التالية لاستكشاف المشكلة وإصلاحها.

- تاكد من ان الحساب الذي قبل دعوه البريد الكتروني هو نفس الحساب الذي يتم استخدامه لتسجيل الدخول لاحقا. تاكد من ان المستخدم يستخدم نفس الحساب لقبول الدعوة وتسجيل الدخول إلى الموقع. 

لمزيد من المعلومات ، راجع [كيفيه أداره الأسماء المستعارة لحساب</a> Microsoft الخاص بك لأداره المكتب 365 تسجيل الدخول](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases). 

- استعرض لكل موقع (مواقع) حيث يتلقى المستخدم الخطا. 

أضافه "/_layouts/15/sys\sscsx/mcershipgrid = 0" (ضمن علامات الاقتباس المزدوجة) إلى نهاية URL الموقع. 

علي سبيل المثال: https://< "contoso" >. sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.

- حدد المستخدم من القائمة.

- انقر فوق **أزاله أذونات المستخدم** من "الشريط". 
-  أضافه المستخدم وأعاده إرسال الدعوة إلى المستخدم.

