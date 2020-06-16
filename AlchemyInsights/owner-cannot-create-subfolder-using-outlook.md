---
title: لا يمكن للمالك إنشاء مجلد فرعي باستخدام Outlook
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5884"
- "3500007"
ms.openlocfilehash: 2116bb837e4378ea29d7882df1d3010b3a4e0b1c
ms.sourcegitcommit: 936330b11fec49f6174eadea6c765bdf9e6ba784
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/12/2020
ms.locfileid: "44748701"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a><span data-ttu-id="3dd83-102">لا يمكن للمالك إنشاء مجلد فرعي باستخدام Outlook</span><span class="sxs-lookup"><span data-stu-id="3dd83-102">Owner cannot create sub-folder using Outlook</span></span>

<span data-ttu-id="3dd83-103">**هناك مشكلة مستمرة مع مالكي المجلدات العمومية إنشاء مجلدات فرعية باستخدام Outlook. سيتم إصلاح المشكلة قريبا.**</span><span class="sxs-lookup"><span data-stu-id="3dd83-103">**There's an ongoing issue with public folder owners creating subfolders using Outlook. The issue will be fixed soon.**</span></span>

<span data-ttu-id="3dd83-104">وفي الوقت نفسه، استخدم أحد الحلول التالية:</span><span class="sxs-lookup"><span data-stu-id="3dd83-104">Meanwhile, use one of the following workarounds:</span></span>

1. <span data-ttu-id="3dd83-105">استخدام Outlook لـ MAC لإنشاء المجلد الفرعي كما تؤثر المشكلة فقط Outlook يندوز سطح المكتب (كافة الإصدارات)</span><span class="sxs-lookup"><span data-stu-id="3dd83-105">Use Outlook for MAC to create the subfolder as the issue impacts only Outlook for desktop windows (all versions)</span></span>
2. <span data-ttu-id="3dd83-106">يكون المسؤول إنشاء المجلد الفرعي باستخدام EXO شل أو EAC</span><span class="sxs-lookup"><span data-stu-id="3dd83-106">Have admin create the subfolder using EXO Shell or EAC</span></span>
3. <span data-ttu-id="3dd83-107">تغيير الافتراضيمجديفبوبولديديرميلبوإكس/فعالةPublicFolderMailbox على المستخدم إلى علبة بريد أخرى من علبة بريد المحتوى للمجلد تسبب المشكلة</span><span class="sxs-lookup"><span data-stu-id="3dd83-107">Change the DefaultPublicFolderMailbox/EffectivePublicFolderMailbox on the user to other mailbox than the Content Mailbox for the folder causing issue</span></span>  
    - <span data-ttu-id="3dd83-108">*تعيين علبة البريد User1 DefaultPublicFolderMailbox PubMBX3*</span><span class="sxs-lookup"><span data-stu-id="3dd83-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span></span>
4. <span data-ttu-id="3dd83-109">انتظر لمدة ساعة، أعد تشغيل عميل Outlook</span><span class="sxs-lookup"><span data-stu-id="3dd83-109">Wait for an hour, restart outlook client</span></span>