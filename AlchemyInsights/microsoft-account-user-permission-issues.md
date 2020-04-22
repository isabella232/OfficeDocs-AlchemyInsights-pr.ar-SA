---
title: استكشاف المشكلة - لم يتم العثور على المستخدم في الدليل
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 3b863c5e9962dd29ca2ed41d113041d74830f615
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43702725"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>استكشاف المشكلة - لم يتم العثور على المستخدم في الدليل

إذا كان المستخدمون يتلقون رسالة خطأ "لا يمكن العثور على المستخدم" في الدليل، الرجاء المحاولة مرة أخرى حيث نوع المشكلة هو المستخدم غير موجود في الدليل.

يمكن إكمال الخطوات التالية لاستكشاف المشكلة.

- تأكد من أن الحساب الذي قبل دعوة البريد الإلكتروني هو نفس الحساب الذي يتم استخدامه لتسجيل الدخول لاحقًا. تأكد من أن المستخدم يستخدم نفس الحساب لقبول الدعوة وتسجيل الدخول إلى الموقع. 

لمزيد من المعلومات، راجع [كيفية إدارة الأسماء</a> المستعارة لحساب Microsoft لإدارة تسجيل الدخول Microsoft 365](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases). 

- استعراض إلى كل موقع (مواقع) يتلقى فيها المستخدم الخطأ. 

إضافة "/_layouts/15/people.aspx/membershipgroupid=0" (ضمن علامات الاقتباس المزدوجة) إلى نهاية عنوان URL للموقع. 

مثال: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.

- حدد المستخدم من القائمة.

- انقر فوق **إزالة أذونات المستخدم** من الشريط. 
-  إضافة المستخدم مرة أخرى وإعادة إرسال الدعوة إلى المستخدم.

