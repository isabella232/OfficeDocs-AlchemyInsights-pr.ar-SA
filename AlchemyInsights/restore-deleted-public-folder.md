---
title: استعادة مجلد عام محذوف
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3488"
ms.openlocfilehash: 7b04612daca61650d162c1dde240e25c1b185b04
ms.sourcegitcommit: 8ba12eff67e405f5922ea4cc35155e3036447859
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/15/2020
ms.locfileid: "42063580"
---
# <a name="restore-a-deleted-public-folder"></a>استعادة مجلد عام محذوف

**لاستعادة العناصر المحذوفة من مجلد عام:**

- راجع [لا يمكنك استرداد العناصر المحذوفة من مجلد عام غير بريد في Outlook 2016](https://aka.ms/pfrec).
 
**لاستعادة مجلد عام محذوف (من أي نوع):** 

- الرجاء استخدام الأمر EXO PowerShell التالي:

    بناء الجمله:

    >$pf = الحصول على PublicFolder \NON_IPM_SUBTREE \DUMPSTER_ROOT -recurse | ؟ {$_. اسم -eq\<"name_of_deleted_public_Folder"}؛ Set-PublicFolder $pf.identity-مسار \<حيث سيتم استعادة المجلد>

    مثال: سيقوم الأمر التالي باستعادة المجلد الفرعي1 ووضعه تحت \Parent1:

    >$pf = الحصول على PublicFolder \NON_IPM_SUBTREE \DUMPSTER_ROOT -recurse | ؟ {$_. اسم -eq "subfolder1"}; تعيين-PublicFolder $pf.الهوية -مسار \Parent1

راجع [استعادة مجلد عام محذوف](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) لمزيد من التفاصيل.
