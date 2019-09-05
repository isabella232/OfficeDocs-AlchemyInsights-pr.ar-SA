---
title: استكشاف الأخطاء وإصلاحها - لم يتم العثور على المستخدم في الدليل
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 81b9dafe8e27e5f73fe232c51ff56fed3fec29b4
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/04/2019
ms.locfileid: "36754179"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>استكشاف الأخطاء وإصلاحها - لم يتم العثور على المستخدم في الدليل

إذا كان المستخدمون يتلقون رسالة خطأ "لا يمكن العثور على المستخدم" في الدليل. الرجاء المحاولة مرة أخرى حيث يكون "نوع المشكلة" المستخدم غير موجود في الدليل.

يمكن إكمال الخطوات التالية لاستكشاف المشكلة وإصلاحها.

- تأكد من أن الحساب الذي قبل دعوة البريد الإلكتروني هو نفس الحساب الذي يتم استخدامه لتسجيل الدخول لاحقًا. تأكد من أن المستخدم يستخدم نفس الحساب لقبول الدعوة والتسجيل في الموقع. 

لمزيد من المعلومات، راجع [كيفية إدارة</a> الأسماء المستعارة لحساب Microsoft الخاص بك لإدارة تسجيل دخول Office 365](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases). 

- استعرض للوصول إلى كل موقع (مواقع) يتلقى المستخدم الخطأ. 

إضافة "/_layouts/15/people.aspx/membershipgroupid =0" (ضمن علامات الاقتباس المزدوجة) إلى نهاية URL الموقع. 

على سبيل المثال: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.

- حدد المستخدم من القائمة.

- انقر فوق **إزالة أذونات المستخدم** من الشريط. 
-  إضافة المستخدم مرة أخرى وإعادة إرسال الدعوة إلى المستخدم.

