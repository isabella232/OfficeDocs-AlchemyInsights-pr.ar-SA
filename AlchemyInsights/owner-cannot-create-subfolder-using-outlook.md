---
title: يتعذر على المالك إنشاء مجلد فرعي باستخدام Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5884"
- "3500007"
ms.openlocfilehash: b2ab7b60bc521fd28d68333bb963528f7b9e05f2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836122"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a><span data-ttu-id="c4e3f-102">يتعذر على المالك إنشاء مجلد فرعي باستخدام Outlook</span><span class="sxs-lookup"><span data-stu-id="c4e3f-102">Owner cannot create sub-folder using Outlook</span></span>

<span data-ttu-id="c4e3f-103">**هناك مشكلة مستمرة في إنشاء مالكي المجلدات العمومية للمجلدات الفرعية باستخدام Outlook. سيتم إصلاح المشكلة قريبا.**</span><span class="sxs-lookup"><span data-stu-id="c4e3f-103">**There's an ongoing issue with public folder owners creating subfolders using Outlook. The issue will be fixed soon.**</span></span>

<span data-ttu-id="c4e3f-104">وفي هذه الأثناء، استخدم أحد الحلول التالية:</span><span class="sxs-lookup"><span data-stu-id="c4e3f-104">Meanwhile, use one of the following workarounds:</span></span>

1. <span data-ttu-id="c4e3f-105">استخدم Outlook for MAC لإنشاء الملف الفرعي حيث تؤثر المشكلة على Outlook فقط على نوافذ سطح المكتب (كل الإصدارات)</span><span class="sxs-lookup"><span data-stu-id="c4e3f-105">Use Outlook for MAC to create the subfolder as the issue impacts only Outlook for desktop windows (all versions)</span></span>
2. <span data-ttu-id="c4e3f-106">هل يجب على المسؤول إنشاء المدوّن الفرعي باستخدام EXO Shell أو EAC</span><span class="sxs-lookup"><span data-stu-id="c4e3f-106">Have admin create the subfolder using EXO Shell or EAC</span></span>
3. <span data-ttu-id="c4e3f-107">تغيير DefaultPublicFolderMailbox/EffectivePublicFolderMailbox على المستخدم إلى علبة بريد أخرى غير علبة بريد المحتوى للمجلد الذي تسبب المشكلة</span><span class="sxs-lookup"><span data-stu-id="c4e3f-107">Change the DefaultPublicFolderMailbox/EffectivePublicFolderMailbox on the user to other mailbox than the Content Mailbox for the folder causing issue</span></span>  
    - <span data-ttu-id="c4e3f-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span><span class="sxs-lookup"><span data-stu-id="c4e3f-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span></span>
4. <span data-ttu-id="c4e3f-109">انتظر لمدة ساعة، أعد تشغيل عميل outlook</span><span class="sxs-lookup"><span data-stu-id="c4e3f-109">Wait for an hour, restart outlook client</span></span>