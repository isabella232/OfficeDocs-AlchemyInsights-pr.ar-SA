---
title: مشكله استكشاف الأخطاء وإصلاحها-تعذر العثور علي المستخدم في الدليل
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 512494a69ab274af00962cb9777a3479b4200fd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47725394"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>مشكله استكشاف الأخطاء وإصلاحها-تعذر العثور علي المستخدم في الدليل

إذا قام المستخدمون بتلقي رسالة خطا "تعذر العثور علي المستخدم" في الدليل ، يرجى المحاولة مره أخرى حيث يكون نوع المشكلة مستخدما ليس في الدليل.

يمكن إكمال الخطوات التالية لاستكشاف المشكلة وإصلاحها.

- تاكد من ان الحساب الذي وافق علي دعوه البريد الكتروني هي نفس الحساب الذي يتم استخدامه لتسجيل الدخول لاحقا. تاكد من ان المستخدم يستخدم الحساب نفسه لقبول الدعوة وتسجيل الدخول إلى الموقع. 

لمزيد من المعلومات ، راجع [كيفيه أداره الأسماء المستعارة لحساب microsoft الخاص بك </a> لأداره تسجيل الدخول إلى microsoft 365](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases). 

- استعرض وصولا إلى الموقع (المواقع) الذي يتلقى فيه المستخدم الخطا. 

أضف "/_layouts/15/people.aspx/membershipgroupid = 0" (ضمن علامات الاقتباس المزدوجة) إلى نهاية عنوان URL الخاص بالموقع. 

مثال: https://< "contoso" >. sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.

- حدد المستخدم من القائمة.

- انقر فوق **أزاله أذونات المستخدمين** من الشريط. 
-  أضف المستخدم وأرسل الدعوة إلى المستخدم.

