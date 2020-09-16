---
title: يتعذر علي المالك إنشاء مجلد فرعي باستخدام Outlook
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 9590f780cffeaf644733752c763e04d748b1b39e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47665705"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a><span data-ttu-id="2d7d5-102">يتعذر علي المالك إنشاء مجلد فرعي باستخدام Outlook</span><span class="sxs-lookup"><span data-stu-id="2d7d5-102">Owner cannot create sub-folder using Outlook</span></span>

<span data-ttu-id="2d7d5-103">**توجد مشكله مستمرة في مالكي المجلدات العامة لإنشاء مجلدات فرعيه باستخدام Outlook. سيتم تصحيح المشكلة قريبا.**</span><span class="sxs-lookup"><span data-stu-id="2d7d5-103">**There's an ongoing issue with public folder owners creating subfolders using Outlook. The issue will be fixed soon.**</span></span>

<span data-ttu-id="2d7d5-104">اثناء ، استخدم أحد الحلول البديلة التالية:</span><span class="sxs-lookup"><span data-stu-id="2d7d5-104">Meanwhile, use one of the following workarounds:</span></span>

1. <span data-ttu-id="2d7d5-105">استخدام Outlook for MAC لإنشاء المجلد الفرعي لان المشكلة تؤثر فقط علي Outlook لسطح المكتب من windows (كل الإصدارات)</span><span class="sxs-lookup"><span data-stu-id="2d7d5-105">Use Outlook for MAC to create the subfolder as the issue impacts only Outlook for desktop windows (all versions)</span></span>
2. <span data-ttu-id="2d7d5-106">جعل المسؤول ينشئ المجلد الفرعي باستخدام أكسو Shell أو EAC</span><span class="sxs-lookup"><span data-stu-id="2d7d5-106">Have admin create the subfolder using EXO Shell or EAC</span></span>
3. <span data-ttu-id="2d7d5-107">تغيير ديفاولتبوبليكفولديرميلبوكس/افيكتيفيبوبليكفولديرمايلبوكس علي المستخدم إلى علبه بريد أخرى بخلاف علبه بريد المحتوي للمجلد الذي يسبب المشكلة</span><span class="sxs-lookup"><span data-stu-id="2d7d5-107">Change the DefaultPublicFolderMailbox/EffectivePublicFolderMailbox on the user to other mailbox than the Content Mailbox for the folder causing issue</span></span>  
    - <span data-ttu-id="2d7d5-108">*تعيين-علبه البريد User1 ديفاولتبوبليكفولديرميلبوكس PubMBX3*</span><span class="sxs-lookup"><span data-stu-id="2d7d5-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span></span>
4. <span data-ttu-id="2d7d5-109">انتظر لمده ساعة ، أعد تشغيل عميل outlook</span><span class="sxs-lookup"><span data-stu-id="2d7d5-109">Wait for an hour, restart outlook client</span></span>