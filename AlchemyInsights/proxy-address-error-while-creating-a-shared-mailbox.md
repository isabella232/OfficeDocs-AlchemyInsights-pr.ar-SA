---
title: خطأ في عنوان الوكيل أثناء إنشاء علبة بريد مشتركة
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
ms.openlocfilehash: ab491e883ab294f08d0b5d2e686dc059b468d29f
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/09/2021
ms.locfileid: "50568277"
---
# <a name="proxy-address-error-while-creating-a-mailbox-or-other-email-enabled-object"></a><span data-ttu-id="fd71e-102">خطأ في عنوان الوكيل أثناء إنشاء علبة بريد أو كائن آخر تم تمكين البريد الإلكتروني له</span><span class="sxs-lookup"><span data-stu-id="fd71e-102">Proxy address error while creating a mailbox or other email enabled object</span></span>

<span data-ttu-id="fd71e-103">إذا حاولت إنشاء كائن تم تمكينه للبريد الإلكتروني (علبة البريد، علبة البريد المشتركة وما إلى ذلك) تلقيت رسالة الخطأ "عنوان الوكيل "SMTP:alias@domain.com" مستخدم بالفعل..."، يتم بالفعل استخدام عنوان البريد الإلكتروني الذي اخترته بواسطة كائن آخر تم تمكين البريد الإلكتروني له في مؤسستك.</span><span class="sxs-lookup"><span data-stu-id="fd71e-103">If you tried to create an email-enabled object (mailbox, shared mailbox etc.) and received the error "The proxy address "SMTP:alias@domain.com" is already being used…", the email address you chose is already taken by another email-enabled object in your organization.</span></span>
  
<span data-ttu-id="fd71e-104">ستحتاج إلى البحث عن المستخدم أو المجموعة أو علبة البريد المشتركة أو المجلد العمومي الذي يحتوي على عنوان البريد الإلكتروني هذا وحذفه أو تغيير عنوان البريد الإلكتروني الخاص به.</span><span class="sxs-lookup"><span data-stu-id="fd71e-104">You need to find the user, group, shared mailbox or public folder that has this email address and delete it or change its email address.</span></span> <span data-ttu-id="fd71e-105">بعد ذلك، يمكنك إنشاء كائن جديد لتمكين البريد الإلكتروني باستخدام عنوان البريد الإلكتروني الذي تم تحريره.</span><span class="sxs-lookup"><span data-stu-id="fd71e-105">Then you can create a new email-enabled object with the freed email address.</span></span> <span data-ttu-id="fd71e-106">استخدم "البحث" على الصفحة الرئيسية للعثور عليه.</span><span class="sxs-lookup"><span data-stu-id="fd71e-106">Use Search on the Home page to find it.</span></span> <span data-ttu-id="fd71e-107">يمكنك أيضا استخدام الأمر التالي في Exchange Online PowerShell للبحث عنه:</span><span class="sxs-lookup"><span data-stu-id="fd71e-107">You can also use the following Exchange Online PowerShell command to search for it:</span></span>

`
    Get-EXORecipient -Filter "EmailAddresses -eq 'email@contoso.onmicrosoft.com'"
`
  
<span data-ttu-id="fd71e-108">إذا كنت لا تريد حذف عنوان البريد الإلكتروني الموجود، فاختر عنوان بريد إلكتروني جديد للكائن الجديد الذي تقوم بإنشاءه.</span><span class="sxs-lookup"><span data-stu-id="fd71e-108">If you don't want to delete the existing email address, choose a new email address for the new object you are creating.</span></span>
  