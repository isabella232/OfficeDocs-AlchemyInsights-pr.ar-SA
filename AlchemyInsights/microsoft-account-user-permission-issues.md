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
ms.openlocfilehash: 1825cfd0a78a29734d0a5128e19acbfba9115d32
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/04/2019
ms.locfileid: "34717334"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>حل المشكلة-المستخدم غير موجود في الدليل

<p>إذا كان المستخدمون تتلقى رسالة الإعلام بالخطأ <strong> &ldquo; &hellip;يمكن للمستخدم&rsquo;t يكون موجود في الدليل. الرجاء المحاولة مرة أخرى&hellip; </strong> حيث "نوع المشكلة" <strong> &ldquo;مستخدم غير موجود في الدليل.&rdquo;</strong>، يمكنك إكمال الخطوات التالية استكشاف المشكلة وإصلاحها.</p> <ol> <li>تأكد من الحساب الذي قبلت دعوة البريد الإلكتروني هو نفسه الحساب الذي يتم استخدامه لتسجيل الدخول لاحقاً. تأكد من أن المستخدم يستخدم نفس الحساب لقبول الدعوة وتسجيل الدخول إلى الموقع. <br /><br />لمزيد من المعلومات، راجع <a href="https://support.microsoft.com/en-us/help/12407/microsoft-account-how-to-manage-aliases">كيفية إدارة الأسماء المستعارة لحساب Microsoft</a> لإدارة تسجيل الدخول Office 365. <br /><br /></li> <li>استعرض للوصول إلى كل المواقع التي يتلقى المستخدم الخطأ. <br /><br />أ. إضافة <strong> &ldquo;/_layouts/15/people.aspx/membershipgroupid=0&rdquo; </strong> (داخل علامات اقتباس المزدوجة) إلى نهاية url الخاص بالموقع. <br /><br />على سبيل المثال: https://&lt;شركة "التعمير"&gt;.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0 <br /><br />(ب). حدد المستخدم من القائمة. <br /><br />(ج). انقر فوق <strong>إزالة أذونات المستخدم من "الشريط"</strong>. <br /><br />(د). إضافة المستخدم مرة أخرى وإعادة إرسال الدعوة إلى المستخدم.</li> </ol>

