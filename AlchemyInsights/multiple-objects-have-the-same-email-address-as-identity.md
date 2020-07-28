---
title: تحتوي الكائنات المتعددة على نفس عنوان البريد الإلكتروني كـ الهوية
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1834"
- "9000247"
ms.openlocfilehash: cc932aa7ecbd1e338c409a7a6525e2c4e673b232
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 07/28/2020
ms.locfileid: "45438673"
---
# <a name="multiple-objects-have-the-same-email-address-as-identity"></a>تحتوي الكائنات المتعددة على نفس عنوان البريد الإلكتروني كـ الهوية

**كائنات متعددة**

أحد الأسباب الشائعة لهذا الخطأ هو عدم القدرة على توجيه طلب Outlook Web Access بشكل صحيح في وجود كائنات متعددة لها نفس عنوان البريد الإلكتروني كهوية. للبحث عن هذه الكائنات، قم بتشغيل الأوامر التالية:

· الحصول على مستلم<email address>

· الحصول على المستخدم<email address>

· الحصول على المستخدم <email address> -SoftDeletedUser

· الحصول على الاتصال<email address>

· الحصول على علبة البريد <email address> -PublicFolder

· الحصول على علبة البريد <email address> -IncludeSoftDeletedميلبوك

· الحصول على علبة البريد <email address> -غير نشطالبريد الإلكتروني فقط

لحل هذه المشكلة، إزالة كائنات متعددة بنفس هوية البريد الإلكتروني وتأكد من وجود كائن واحد مع هوية البريد الإلكتروني المحدد وأن نوع المستلم الخاص به هو UserMailbox.

**يستخدم نفس العنوان لصناديق البريد الخاصة بالعمل والمستهلك**

سبب آخر هو عند استخدام نفس العنوان لصناديق البريد الأعمال والمستهلك. في هذه الحالة، يجب على المستخدم تغيير الاسم المستعار المستهلك الأساسي حتى يدعم Cafe هذا السيناريو. هذا خطأ دائم لا يذهب بعيدا دون تدخل.

للحصول على التفاصيل، راجع [تغيير عنوان البريد الإلكتروني أو رقم الهاتف لحساب Microsoft الخاص بك](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account).