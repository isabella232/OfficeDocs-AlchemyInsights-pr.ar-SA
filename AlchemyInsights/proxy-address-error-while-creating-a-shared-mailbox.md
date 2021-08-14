---
title: خطأ عنوان الوكيل أثناء إنشاء علبة بريد مشتركة
ms.author: pebaum
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ece4bcce-1053-4ed3-a194-9d0af8f73c6f
ms.custom:
- "19"
- "6"
ms.openlocfilehash: 7c15d5db5445fbe4c3ec22878f180f48d2da4f90369f2e6f223916646eb19c12
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54062895"
---
# <a name="proxy-address-error-while-creating-a-mailbox-or-other-email-enabled-object"></a>خطأ عنوان الوكيل أثناء إنشاء علبة بريد أو كائن آخر تم تمكين البريد الإلكتروني له

إذا حاولت إنشاء كائن تم تمكينه للبريد الإلكتروني (علبة البريد، علبة البريد المشتركة وما إلى ذلك) تلقيت رسالة الخطأ "عنوان الوكيل "SMTP:alias@domain.com" مستخدم بالفعل..."، يتم بالفعل أخذ عنوان البريد الإلكتروني الذي اخترته بواسطة كائن آخر تم تمكينه للبريد الإلكتروني في مؤسستك.
  
يجب البحث عن المستخدم أو المجموعة أو علبة البريد المشتركة أو المجلد العمومي الذي يحتوي على عنوان البريد الإلكتروني هذا وحذفه أو تغيير عنوان بريده الإلكتروني. بعد ذلك، يمكنك إنشاء كائن جديد لتمكين البريد الإلكتروني باستخدام عنوان البريد الإلكتروني الذي تم تحريره. استخدم البحث في الصفحة الرئيسية للعثور عليه. يمكنك أيضا استخدام Exchange Online PowerShell للبحث عنه:

`
    Get-EXORecipient -Filter "EmailAddresses -eq 'email@contoso.onmicrosoft.com'"
`
  
إذا كنت لا تريد حذف عنوان البريد الإلكتروني الموجود، فاختر عنوان بريد إلكتروني جديد للكائن الجديد الذي تقوم بإنشاءه.
  