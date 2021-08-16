---
title: تملك كائنات متعددة عنوان البريد الإلكتروني نفسه كالهوية
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1834"
- "9000247"
ms.openlocfilehash: 5866d182cb2e97e37bc6df87e05fb6ef55bfed1d36f9daa95b7b8993a509e2dd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54011899"
---
# <a name="multiple-objects-have-the-same-email-address-as-identity"></a>تملك كائنات متعددة عنوان البريد الإلكتروني نفسه كالهوية

**كائنات متعددة**

أحد الأسباب الشائعة لهذا الخطأ هو عدم القدرة على توجيه Outlook ويب Access بشكل صحيح في حالة وجود عدة كائنات لها عنوان البريد الإلكتروني نفسه كالهوية. للعثور على هذه الكائنات، يمكنك تشغيل الأوامر التالية:

· Get-Recipient <email address>

· Get-User <email address>

· Get-User <email address> -SoftDeletedUser

· Get-Contact <email address>

· Get-Mailbox <email address> -PublicFolder

· Get-Mailbox <email address> -IncludeSoftDeletedMailbox

· Get-Mailbox <email address> -InactiveMailboxOnly

لحل هذه المشكلة، قم بإزالة كائنات متعددة بنفس هوية البريد الإلكتروني وتأكد من وجود كائن واحد له هوية بريد إلكتروني محددة ومن أن نوع المستلم الخاص به هو UserMailbox.

**يتم استخدام العنوان نفسه لعلب بريد الأعمال والمستهلكين**

هناك سبب آخر وهو استخدام العنوان نفسه لعلب بريد الأعمال والمستهلكين. في هذه الحالة، يجب على المستخدم تغيير الاسم المستعار للمستهلك الأساسي حتى يدعم مقهى هذا السيناريو. هذا خطأ دائم لا يزول بدون تدخل.

للحصول على التفاصيل، راجع [تغيير عنوان البريد الإلكتروني أو رقم الهاتف لحساب Microsoft](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account)الخاص بك .