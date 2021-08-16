---
title: استكشاف الأخطاء وإصلاحها - لم يتم العثور على المستخدم في الدليل
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 79429f8e9523ad6b08cd2cd2b19dd221bac797d00de142cbb18826b86fb5ae4e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54098157"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>استكشاف الأخطاء وإصلاحها - لم يتم العثور على المستخدم في الدليل

إذا كان المستخدمون يتلقون رسالة خطأ "لا يمكن العثور على المستخدم" في الدليل، فيرجى المحاولة مرة أخرى حيث نوع المشكلة هو المستخدم غير في الدليل.

يمكن إكمال الخطوات التالية لا استكشاف المشكلة وإصلاحها.

- تأكد من أن الحساب الذي قبل دعوة البريد الإلكتروني هو نفس الحساب الذي يتم استخدامه في تسجيل الدخول لاحقا. تأكد من أن المستخدم يستخدم الحساب نفسه لقبول الدعوة ثم تسجيل الدخول إلى الموقع. 

لمزيد من المعلومات، راجع كيفية إدارة الأسماء المستعارة لحساب Microsoft الخاص بك لإدارة Microsoft 365 [ </a> تسجيل الدخول.](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases) 

- استعرض بحثا عن كل موقع (مواقع) يتلقى المستخدم الخطأ فيه. 

أضف "/_layouts/15/people.aspx/membershipgroupid=0" (ضمن علامات الاقتباس المزدوجة) إلى نهاية عنوان URL للموقع. 

مثال: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.

- حدد المستخدم من القائمة.

- انقر **فوق إزالة أذونات المستخدم** من الشريط. 
-  قم بإضافة المستخدم مرة أخرى ثم إعادة إرسال الدعوة إلى المستخدم.

